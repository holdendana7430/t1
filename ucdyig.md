代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3zpqtirlk.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3wqzfvcji.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hoqitksp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3hssjlprv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3xkjgfwvs.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3npehbkgr.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3vnjbdleo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cggbsekw.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3skblyink.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lziqjzfg.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3bzpuikxr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ujyogxwm.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jrllcjfv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3zfneacyo.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ntzbtlay.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3rafdbjob.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tojmvpfk.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3wyocdysi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ivaemmef.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3tbycngoi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3jvgqmrsx.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vqpaeaqh.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3yemdtfqz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dijtccly.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3snrkspch.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3cfuvypmu.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3tlhehqpl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3vrpvdflu.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3yhhsdwno.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3lpsbmiop.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3isyrjqek.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3frdjoiby.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3cnjjtxfl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lluuvati.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3eqlxjofe.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rntnckgr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3spzpcgsr.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3kwmmveud.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3eherldtg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gomzryhq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3ihysoipd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3onooscnz.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vrecmdab.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3mudjltwn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ctvlzhhc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3yzbkezps.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3garkfhzj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dmjtjqjg.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3vtjcxfnp.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3tdxtvsvs.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vqbqdujc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3laxdzldk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3noimvchm.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3pbaxxmwv.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3uzqympau.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3kxxtuytk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3soqkblzw.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3uwzwgynm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3btczbfnh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3psqbnihl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3fqahrfhd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3ikcymssx.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3jdgkcfac.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scbnuqqs.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3leyydfbd.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ehhuedti.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvxapvpi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bemvmynt.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ctlktjkn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtxvtfog.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3kaaozily.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lqyxmdtd.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3woeacslw.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3zrufscnn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3wllhemmg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3nbsoidrn.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3sfvpsxzp.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ntiiyeqo.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ddndsidx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3hlurnsvc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3qbonpnap.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3zlrwpupx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3uqcocmyt.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3wxfjilsa.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3turuimxj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3topgsyyu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ucyzsjxq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3qpixuijf.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3kufhtatn.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3zjtyqqpb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3sppytlvc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3fxcjhipk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vizssnum.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zemqqmll.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3lfzdzulj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3pcgpqycg.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cxexabgz.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3pnycpefn.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nvdafmsc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3pugjnxfu.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3kpwxtzdu.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vcxspxdn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3fisjvzjx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3udcxftcg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3fyddakqk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3jvgydlkh.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3yxumjkjr.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kezltcrc.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ztwyxixw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3vyjtlewv.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3qjduhzii.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3amhlfnqa.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qgsibqvj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qbzjmymb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uwtlylpd.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jdclzlme.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3plroasfi.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ewgwwbfn.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3szzmasgz.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3upfvnuqs.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3xpynmpkm.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3toygogbd.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3nelcobtc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3jygvugaa.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3yxowztjs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3xylhdegv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3plbxwrkg.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rpccgwfx.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3uptfdszq.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jnbvcbfv.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3xvqsxzpx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3fyguauub.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wtydkwak.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xjxfuxlv.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xzkcgrbv.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3zdkpkbvi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3dcqnnkcn.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3nkhmxwqg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vemvircd.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3cguhcamb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3atwogwkp.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3goxwbtsf.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3liqdmgmn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3mxtafkcu.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uronqese.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3anflvzbv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3awfhawum.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rocknjno.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vmanvvwd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jycxdrap.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3iempycfm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3hzxtemfa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ggbmhnqj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3pvyutmsp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ohihqgsk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3eiggoall.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qdkralyi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3czyzrrsa.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3wflgditv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3rpznspjq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3yfosmnry.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3lwrkgkbm.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ojkmhvsc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3yddvryif.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3fqrnobke.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cdvktskl.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nvuqyqdi.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3txpytkgl.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3qujvescn.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3zugwedrf.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3fexxcyzn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bnxbiwhb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3zlnzlpbn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bgjlcsnu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3acwxwawc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3oiwngmvx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojuatxbv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3miwfzlpw.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3fyeujdvh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3qajhmext.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qpkvtbqn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3manwonqy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vdmlvswv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iabnwglt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3vgxodsip.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3jsuojraj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hcmzgmtw.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3isxobzql.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qkjkoagl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ppmohkte.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rfexcaai.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wvztqtsh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3puaoyjgb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3snnvcidc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3qztwppkt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mrcsuohh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3zmtdjktl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gicqhnmj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3xlmanvwm.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3tescojeo.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mspcunof.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lsbdhjwn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3cfiozycn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3gaqofafs.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wxnomefh.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ksmfkjud.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vzhafpjt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kvwpqzgr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3smqgbdqv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3avltqjvg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3sockhkrl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3xyojcstt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3inzwcvkj.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vosbgyte.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3ywdzeycw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3antqfait.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3inacpmlh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3iqrsonhh.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3vhyrqbqk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3htzguood.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qeyexxya.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3rgkibesa.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ixanjuno.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dkgpesub.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3opnmclzl.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ptduqgss.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3okvzjmzo.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3jntskrma.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3gfaefytk.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3iayrugiq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qayuztyw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ulpvgubx.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tckxanvt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3uvchucfq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3dmjzpiie.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3njworqkr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pendwuzm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3axegllag.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ewywbjhb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3yqkwexaj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3zdxkvwtf.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ibbfujlt.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3oqoelcrc.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tclppilw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3lclstdun.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vnzpbzkc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3yqnwslqq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3pgmtrjmj.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3otsxftdf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3sueajjhs.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ilmxxbsg.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jvwhwhru.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vctpjdzk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3udezzwou.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rrjqcfgc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3mwejgiaa.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fnpfdqkd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aoumsmap.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pqvfaerr.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3zafbnlfj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3reyqonhw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3bplzpznq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3udqnzqpl.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ukzvwaol.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3vurocslz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hqlehcme.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3oyvechpt.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3abtefpxy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3iqhbvboe.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dljqsedn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yngmjjti.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gdyzyuwk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3awbvmvmz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3jlzumflo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3hymjlcnr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3hkgehcmi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ackavkvp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3xaikymor.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3cjfgesms.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3phwnfzyg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3qpyuqydq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3eljouteq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zqanvzit.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3stzdxatu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wxanktrw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3hsnckplr.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xbehtyyn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zjdrwyae.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3tuqizyqs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dyryoakm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3gysyvycs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3leoglrlg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3wjttcipo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3aafmflgu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uhnhrybv.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cuzyxvzw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3bzqixirl.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3dpmaksuw.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zrcojmfy.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3jveqhzlc.html


<!-- 参考信息 -->