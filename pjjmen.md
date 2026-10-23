代发 wailian999

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3ppajzxrj.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3shwluewe.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uvrpkder.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3rfiimisa.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3pygalmlj.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3zrtpaqdf.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3cusezaek.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3nmvgizvb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3pbxtyjsr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3aufdwkkb.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3dbynouzr.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3zqabzwwg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3eulojgyd.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3bvzuvdnz.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3fwowwspu.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3jxqzfnio.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3asvfwjtb.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3vgayhtmm.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ggghhwjn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3aecghagj.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3ezwpehfn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3oaoxvahh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3pcejzxnu.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3jljsbcpn.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3evhfnzki.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkilmydf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3uofgycug.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxahrnjl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvyykfsp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3yhlijpgl.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3hlkzxvhj.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3gsxocqdd.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3vgnquktz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3zmxbftuk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fmirzlvo.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zwxtfsux.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3djdkqgad.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3qmagmpun.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3mnajrfor.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kgrdzerc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3bliozviq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3gvcdmwmd.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3srgjbjyo.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3bxyaeqog.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zxdpqhgs.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fumbuvhb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3bdcfbzyb.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qzzdotdw.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3mwakchxu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3yskcwqsl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3okppqfsc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3jntnejto.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3gohxnits.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3nejwwfxc.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cafjgnsc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ayenejwn.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3fqrfngpx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3cnhfelec.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3mijwcpuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3duggtawi.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3nbdhqwxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yzhsqgcj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3shvzdsnj.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3pprhyiai.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ruttcdub.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3hklhyyai.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3wwcfgrhc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3vzawykym.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3zfrqhwzb.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3cjjhvlpx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3maempobi.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3hguvpodk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3iabtqzfp.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ghstlyuv.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3flhspqcj.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cateeykc.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3leczsgjg.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3idjedeuo.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ybbgnpjf.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3igshouly.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ucglfnle.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3jiszydpp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ybuwekki.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3grcwvkwl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3aawvrtsj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xmxsgumh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3rwfejasl.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3hbwereum.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hemwsoos.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3arvjwbpt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nlttkkoz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wfohmnoj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3jwygitsq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3atzqaizi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3ixsnuhkx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3wwicyvfy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3oxmicpjn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3pqelkmod.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3zqhzbjmx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fssamfqe.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3fvcgvmdi.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3evjbdqki.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3lhemvglc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3hqsljwzg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qgxxwduv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pbnnkbzp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3mgwjlkma.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3egghnkes.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pqosyxvw.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kvmkvegk.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ghkoiqgb.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ekrsbxlf.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3blaovqmp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kuxzyfnk.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nqncucgb.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3qzpmcosk.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ckoxhplh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3xdhrrucw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ktwufdlm.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3njgnmkdd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vegalhig.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3iwuwldbm.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3rkbaezmx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3wllrqtlp.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3crpomzbb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3tgxqyxol.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ubealhqb.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3fzuuchdk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3qatinccw.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3jxyfkffa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3mmgwdaoj.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3cigkqton.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3vtkbckjj.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mvoblfbv.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3iqyytcme.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hjyzhmrx.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gghroimb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3flxitwto.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3roulryfe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3tlbwqtaw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vrqkfcub.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ppdggqbx.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3gapvrwwd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3xjmjzzpz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3kdujxuyg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zykozgar.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hkknqwuw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qlahtdrx.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3pelxzuym.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3pxhalikx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3vszyadgj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3zkfsqdrr.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3vvksdfdm.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3dcmwvgwy.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3lfucczsd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3lxrmcpjm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3tvaippae.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gxxtwhhh.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ijbodarz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3irkxdvlw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3xpjpvbip.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3tgzgbfin.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jbuxomml.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gdmhuzls.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xqizruod.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3pavgzhzc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3nqlnrgzy.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cgfbhikf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dsfdgofg.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3iygkhfao.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ckilzofy.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ntmskroq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3nikcysqi.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3oxitxviu.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3clgbxkoc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3tmqmdjdg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3abnccixa.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3zlhznouz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ouvbcdit.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3knmgjjai.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3hhxwvxou.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3stuwbmxl.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tziyjzrf.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ytyzphun.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3dyqylwem.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3khxbralu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pxzjrfsx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3udsljlwc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3klkqzuir.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3pegevvhg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3nfercewu.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3eobaeips.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dihrpxob.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lilifwqt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3nfiwyfxn.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3xmcrcvya.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3irscvgen.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3yzlpnveb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jzneeasc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3puhmoaye.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3pyzdtlyn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uyavemdw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3silwjhop.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3xpngfgyh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uzreloxh.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3vtigsbmv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3bunhbyfc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xbooayzv.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rgrafkxz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3skfliwma.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3nkpmxysk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3sacnrwgx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nmmrnwbx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3aezywfol.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3tupficzq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3jurbuykg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3emdifqow.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3flpkowpa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3syxwwlls.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3klfsypeu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yhoydyis.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3aocvofaf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3sxrkpyuz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rzoikqgx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3jgusuoon.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3fghamxiq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3jajdphik.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3veolcmja.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3fntnzrzx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3vypduoor.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3uynrrtxb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3zyorlfdq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3dqrhidwm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zzjqyazy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3dtgudgzx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3zfqtvnyb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3apacozwq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3buequhiu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3pxubwzik.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3hipkiciz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3teezqlpu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3byzwybec.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3axglcxik.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3tvcrhnfr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3cslzefik.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kapntelc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xfjrspwu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qagivitg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbxapzpp.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dfotuzlv.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fntwlepz.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3oyyjomxs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ihqmtueq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ykfepsmi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vuuvqejd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3wjhkxuay.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zzihflbc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3bhnoxivz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3vbdofqrt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fueksxzg.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jdaekskq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3hshnjqca.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3fyxhxkjb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3haghkyvc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wssluywg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3ejgfnohp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3jnnyicin.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3uwryoktv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3foprtxtg.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3rwragvmn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3mxcuczde.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wrjprhos.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3kqlsyxxv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vpzawkhd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3dpaorrdy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xczvddhq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3xjalgdgm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3banitwwo.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3yzncsrhv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wsemhbpr.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hsoqzdwa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3drxnkbcm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3oocgdyps.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fgwodmho.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3jjpjkksj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qwxrkizj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qfainpjp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ilrlwplw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3lswadekh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3pihqgsxx.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3idqmqyqu.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3gsbpenkj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mpwjhlcw.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3adfasoqh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3csyhbich.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ieqxawcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yiecokqb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3twefkrqm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vyyautxq.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bndxnlsw.html


<!-- 参考信息 -->