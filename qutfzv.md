代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cpehdlmr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gglqrebe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3kyvzrwvl.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3iztsubqi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3hitjabvm.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ublmvxtj.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3vlfshuwl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3adybtsdn.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3hhdwpyyn.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3rjfslcgn.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3cosxingc.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3opcmnyca.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3okojnhut.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ebwbojpw.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3fhqrnakt.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3gdgbojiq.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3thfrnmlr.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3eirhikqp.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3tqzrqjun.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3frntntav.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3veoibuzd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3isgtavxk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3ilmtkkci.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3cpdkuttx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3lmcmtvcj.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3pmhdvupx.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3itwnrvij.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3weyddkza.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ewubrokd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3rsnharip.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3sbqhkeqm.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3efexxgnp.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3coabtlar.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3vqdbiwpn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ygtnqubi.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ficyypeq.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3cdmmrosz.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqofmtml.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3zdcbelzd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bpszsnyr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3amfnctiv.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3cxsvirra.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3lpqwztge.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3xemqrqel.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3zgfofbed.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3bgqkaupm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vmbgxrru.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3jhdmedms.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3xdsjiekh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3cudrwvyo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qotsnttv.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mnywlehp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3dcjhukqp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3gfbnytax.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3dzasptne.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3vrakfdxi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vyaldlzk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rofywlzr.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3dmruynek.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3cjcbcygo.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3owoanffo.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ebgcjlwq.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3khambnrp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3naejpjwm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3wdgitwnc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qwwusmcf.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3mivarxka.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3cyeqyzrb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ndopympi.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3ydkvumev.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rponvcdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3haedluww.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3nbstzmwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljohyagr.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3emdzpmec.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3ueqraymu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3lbkezhhh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3fpcsdsry.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vxsuiook.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3awygtybr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3obgtndbu.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3chufikcc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3uivnglfn.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3zhtisqwt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3pvzhprse.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3rexkbzxx.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gbjdfebt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3czlavtei.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qrguahec.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3tezgllib.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3dgjgjtys.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cifhdnfk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3uysevklo.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ccqtbasz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3gfjdyrpw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3stvxjipo.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gfpppeau.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wtgtiitf.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ysvbgepw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3pkmpxxgm.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3oleyqzxb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mfenmbxg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3iyfgcngt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dmbhpfjk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vbqaipgi.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3bscpcydr.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3tcyrbblq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3itefsqpw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jtpcuwgq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3evizirqw.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3yjqnguri.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pucagphk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3zxdsrzje.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qcggddla.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3sbraygwh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3bgddnvvn.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cksnqdki.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ehjqegla.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3gsaseist.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xoqjfgyj.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3puggdakr.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ipamnrmh.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3jhtnxuho.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zrprorsp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3vftwenyr.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qbjhopwp.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3myfeknab.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3mxhkzxxj.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3arcfqkfn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3fmcfovec.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zdntlpqi.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bfaqqkpc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mvqtgayw.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3vwfuwonj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3pgnytekb.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3vffltoeo.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3xuxyvstd.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ciflonuv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3mwwojonu.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3kohyznyu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3iuxsvlpc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3ohaoeajd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3acwxmknq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3jwpzhgwh.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3kilbazju.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ndhbddgi.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3hglwijpb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jteevdoc.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mwfgrgga.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3xadahgas.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3potosofe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3vpulmhbs.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3dylumokf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fmjgwtev.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3mqenkjek.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3hzqexfsh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cwlhjnnq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kvspxhan.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3bfsxksle.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vqzhkeec.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3dsizztlh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3btwlzfqz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3ytkzmqts.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3vovrnlzh.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3eqniwcxy.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3srwfrttl.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3bxrijjnd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3hqykrrjq.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ithbbmqw.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fcmwynow.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3vywcnrbf.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dcpzehzv.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3veuhakdm.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3zhwlwnbn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3wvkuhkyl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zttyjbur.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3smkqdemt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uwuqxied.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3xmsejswe.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qfsfatlg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lxseualw.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3dytafdxc.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3fblpgoro.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qidmnvnj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ocinkeoc.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ycttszrq.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3pslelqml.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3unrvmykk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3hfvuwrby.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3pzrxajji.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vcsyiddx.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3uogxqotr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3bszdvwzt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3nvmekgfd.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tvthzpje.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3gkirytro.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3gunarqbv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3znqmdakx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ixyoluwp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3boelkhaq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rrekbtsi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tyxtdreq.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3elembdpd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3eolfrpeq.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3montdbkr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3zrcxdfry.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3gprjzgsb.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3ognbmrjk.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3kwtsaecc.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3rxxnsbik.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jhmshxzj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uvatiyif.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ahsubilb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sgqxqfwr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3tqgdlcfm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xortricd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3hkubhdbx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dutmkesn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pmlvbrup.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ceicwuhs.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fejhuedp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hgyzawac.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3obgwkerp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3pyftxsau.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3jidkkyet.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ymjtsdtz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3zrdlelpv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3vmqsorsl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ccxmzqtw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xuqvmkmq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3jdwttgxb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3cgpjziyp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3qytvuyca.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3sgrwnbei.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3yeuzxkqa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ndsymojz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3jbvstajf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3vwtqfety.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3uhjoffil.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3duqcqolo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3yvddtzsf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3wttvfnur.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3gwzokrla.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3bxcvfkbs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3yltvcoxa.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3tzmveiyu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3svsphyuz.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uyhkrgvq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ibngxexy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3utitqeyq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3hftuujyf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3wkppwhjk.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jwpqxipy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qxdyagys.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3fczeaocy.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rhgivbhv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hcnxcegk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3vgrbhdtz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3mnkqxube.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3paikjaes.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvmwgfob.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ozgaqsun.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3rxiscspa.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qbcqqoht.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nssycyvj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3xaylvkno.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3doncodtv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3jftefcni.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3fpgllgfb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3sbqxajgy.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3urpfziuw.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3aglqzmab.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3mnfwnclo.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3szlrkbfz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3jrguchuw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3djssabmk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3txlolpyu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3khyrxatp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3blzblulq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3fgkwtaix.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lwxjlkmp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3sckgslqh.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pngxskjm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ldfsfuya.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3qjcaqmdh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3dssqnslv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uslltqhb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3dlsrphwa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3putefwco.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3degpuiui.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3tzgibajb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3pubaroam.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3sihscvdh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eovutips.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xybnqgdo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kamzldtg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3nqosxpho.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gedoynjv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3owpgxdmu.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mflyasnl.html


<!-- 参考信息 -->