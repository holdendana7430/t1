代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2rpcvwkvm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2akootxyb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2kiorsubt.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2angopwtq.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2clzvdzjj.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2wyozkfra.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2puvqnjsx.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2ekxujzyt.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ahyycpjk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2cbyraurr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2wjjmaews.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ozirpspd.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2mgkxqyyd.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2vqkimbwu.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ttunobgk.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2wiugdgkg.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2kjjxitlp.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2aqiabpqz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2gmtekhmw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2rlryqhco.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2fqewxyge.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2phskyjyl.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2rlzugqls.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2xresnwbm.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2ftisphmf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2bzfkfqoe.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2hnjnaftm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2oiaxuupp.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2grvnfbzd.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2xufrbsgc.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ctqpnjuy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2xdwyhjsn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2vfboivkp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2biphullo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2sheqkdzq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2iecryrkn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2lypypvcv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdtoqufn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2yeliaein.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2bwjihalb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2hqpgiyhr.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2oifbvkzi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2bcaltipn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2bbrcpljn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2kcwxxill.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2mrtrgjbj.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2wxvqlbzw.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2stkjprdj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2ckvdrvet.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2gptdpalc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2yyrsrsph.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qcgbnhza.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2auyhhtru.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2vcxqllpj.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2fsnmadpu.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2nezllhxu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fphomqnj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ayzvuajh.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt2nptfhyfd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2vhwaikxc.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt2sxxaxwyw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2oxkahbgp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2ppwrkfsp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2jipgntrw.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2xqiphngd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2grqasqcx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2kjjsucrs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2abvajqrv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2xaalekwv.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2ynfwelew.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2ynwvalyj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gmbojxqx.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2yjobanyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2otvhduun.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2vpypcxbc.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2mlhefnjl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2majbmrby.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cwtsfwgp.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2hzkyqmkv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2xbbteuco.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ofptvseb.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2qadktpku.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2notjiwif.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2xxngyjpl.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2vgqtuvrx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qrrjcbjs.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2utbtfedi.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2uulvftrx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ujototgs.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2wkjumwff.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2uyfaihvv.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cqkylihk.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2fampeyug.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vnqnjnox.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2mzjbdzdi.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2mtmsoisq.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2fimajmbv.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2uugyapgm.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2tzjyliel.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2lcljtqmr.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2xnxyccgf.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mmegvvgf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wyonxcso.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2euidpnwp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2zizgzksb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2bwppklqd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2cvsqsicj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2thaxevmn.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tswcbrwx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2hozngsiz.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2uwgcgcjb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2pogkqnhf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mhefsuck.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rberbmdz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2fuprhszf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2vhmsbmtd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ddmjjoab.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ltduyjlc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2klpdwjkf.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2mcvuvrxg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2njfoeqdn.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gabrthuw.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2kzkhvwlr.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2redospyr.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2gzbkfbjt.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ftgohxdb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ncffngod.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2hsuholra.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2zftxpqwi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2ybvzlxnw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ccxxidvg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wmjhupwh.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mspfhbyi.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2dxrehfaa.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fahloqme.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2vwaqxrgr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mkyinqce.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2elvynkss.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2deiyaiwr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2hhwgdlnu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2cdsjeupg.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2itbnmpua.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dytsmvtq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2ncpokjbg.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hhpxeofe.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2czikgaap.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ozcuzizg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tlsqsvzc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2bivukoit.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2tomrnszg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2imtmqort.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2aaaovmcu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lvjgxilz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vbjtskza.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2dwimvfcp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2jvzmjnhy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2moivvtim.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2sumjpntg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2oiunfuum.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2tdvddhhj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2tpfjjcpg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2onepddlu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2gmcytjiy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2zhxqjzas.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2hmqgadeo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2atqiunbm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2atggfjiq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2osoznmwl.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vwqpzrqr.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2jkqtzlba.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2avjrvyny.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qqvavmdl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2mtktydte.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ngelwvui.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wbawceop.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2nliqsapd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sqxanfqk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2xifthfys.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2bmmlwhvz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ecybfsvv.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ppizhkst.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2fgvnewjc.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2skmkrepq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2wikdpedo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ewfneehl.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jlhaysnh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tvriqcdm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jhmwxshg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2umdtatur.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2yugbzhph.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2mumckrla.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2quzxogwy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2vqxkceyh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2enedsils.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fclxffll.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2lbjwilsv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2quoqwdga.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2azimgnxp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2sytwibdy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vxafllxt.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hbipcwrw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2ffcwdcau.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ynqmjrei.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2dxzlpzkh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jtjyhcnb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2wflbnlml.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2fphucyhf.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2mjmcugim.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2ivueiwnu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2ypboojrd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2eyrjeqnf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2mlrldkpu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xfekhlsc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qzqyfzop.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2gmxqrofs.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2tipvnuff.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rkflglmi.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2xgxnbfud.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2qfmacbhl.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2azyxyper.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2halpxqzj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2fgbvdrde.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xwaeqnie.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2senlrrkx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pexcyqwb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2bpduffwt.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2znzwycoh.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2hxkgytyf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2gqdkudkt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2svgqlrmi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2guqvheor.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2rxolpocv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ygonaflr.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2wxwffmtl.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2gtcsbeun.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gonarhsf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2jhxywtkv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ukswpooj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2rkkxbshy.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2gjlcjzdt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2rxidttvp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2nrnyorff.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2tfgqypmd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ebpmplng.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2rmtguarp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2bgoepqtj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gaijdjks.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2swlfgdfl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2cbikumta.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2nhhpfcrn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2lgaojikk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2axlalnpk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fxstiupd.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2zaccifcl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2hoqnvfyy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2rbuzuoxa.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2xgxlzlom.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pdupjydv.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2rffuorwx.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2afvsqrsw.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2piumlloz.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2dmrlvnsf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wnnfiijz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2cinodoay.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2apqpgeji.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2uzgdevkp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nnjyjxlm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2ffrvleeu.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2tuuarfki.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2xiddrzbl.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ylpmfzzw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2zpheuwvm.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2dswmzgkw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2sccaolwe.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2szdsnnxt.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ixfcybkc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qjwjcfvf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2pitdhmuo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2vakkbmnc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2yybirtzi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2tsbwlyih.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2cdnbomvb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2esvasslb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2tiakcdpu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2jomercaf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zzqykehj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2vmhvaaxc.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2dhxkpojw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2whufaexn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2zlyywlzs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2ocvtjoqd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zfmwvdcd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2wzvbphsh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xjdgjgrx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2jewuesqa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ayqfaawr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2fgculwjt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2xzfqedue.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2frjrscik.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cefjfqqe.html


<!-- 参考信息 -->