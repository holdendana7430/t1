代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3qseyfutw.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3xavzujpz.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3setwejjp.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3mspeklzt.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jwlqasli.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ulzoeucv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3yndrdgkr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3kqmxwthi.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gejkdfiu.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3iakrsrvm.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3okypeaba.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yhfwlvsq.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rlfpxrtq.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3llekbjau.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3wxipmofv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3ktzpexos.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3wsrpvtsy.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3efvwcdws.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3lpnquznz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3qiripnvk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3boprfldg.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3tbgcuvhq.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3dkypvxal.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3epiqvxoc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3spqomcba.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hcvsrtxo.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3jmmsergl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3zgrfkyvc.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3yoiabqkq.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3kplxyooi.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3aylkigoh.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3eifycskz.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3vvyzcxtn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qnjpbyeo.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3afdxwyfw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3pzwjkjbn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3vwcolgbm.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3jjjnlyqk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pkqqlqkd.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3smwlfemc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3tiepkxjj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhppibcr.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3zguaiuec.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3uaksptcb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqjrwfls.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vfsizrks.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3fcxprftp.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3etivltdb.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3omfwdwhj.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3siqtxtwt.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3sqrmwoiy.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jxlbcqyi.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qnbpfrwp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3djyjmruz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3agdelsvj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rnqhiqog.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3pujinikn.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3poqcpwxk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3cjawdfjr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3humqmkgt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzdzgsdt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3uamjfwjb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mnigtrml.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3mfycjtcp.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3czxpaqow.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3dxmuyxkt.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3hwsgpsri.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ljihuwdu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3jpzbutcn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3rlgqjltu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3hxzluvuh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3perfatel.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3bzyjnpkk.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3pidunhlu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ggavjbkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bcuqycfu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3vnzfboxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jiftnkhs.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ybxpyjux.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3wwjodcgk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3iolxfcra.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pgwelfgs.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3eontapco.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3agbctued.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3vypashkn.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3ejofdlcs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3otxjqimd.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3wscnryfy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3fbyfyesa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3pxfhrpqh.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3kgnppftt.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xyquncqe.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3rsscjwui.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3apamdhun.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3lcnajoor.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3jicqpuip.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3ilfahoou.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3ktkcotmp.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3msppzssw.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3yjtngptl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cidfrdzj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bsrpujiw.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3bwltuypb.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3rslzxeny.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uydbmegq.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3mnytpaco.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pddyntir.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dbyikvkc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3nhhrxkvs.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ogmzksts.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3undcertg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3xvfsszbd.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3qztrkwso.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3szzmmled.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3swrlzrjt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ywauvzcz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aggcfbxu.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3btlaxcoj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ihdmvsqz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3mxzshsmc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3fheztlld.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3apazvpzs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3bauixprx.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ccqsmohg.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3czfjzfbv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3aiklyxhm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3buwyuhdo.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tahecjxp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3vnxzodtm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nldurqpj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3stgdvvoh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3olrxxtfc.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3lnnkpuma.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ylfuajzh.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3bibxbdnr.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3lykgqcbb.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fguiwljt.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tumyazmg.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3scllqlev.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3xvuwjhjn.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3hnwppvgy.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3cogmmcfp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3mhwcceod.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3dmqtvlxd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ksbvxpay.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3xjronnef.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3jbhljphm.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3ichaqmnd.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3cfijzgxm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zjgqindo.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3xjunabwd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gihvpokd.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3onbyabyh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ycrdzsra.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ozwctdkb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3smmzpdek.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3axvtixea.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tszxgoqe.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3aitnazjm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3gxmuzvye.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xovxaiot.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qupxsilh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3cszynatd.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3brxgfisg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3sbjwgjio.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3midgzsek.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rlqnupqb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3bjwwiiua.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3fknkzbny.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3jimaztgd.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pduuldmk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3vwxgqhaf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3ffzivxlz.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3gkgzdczy.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3rsanmozs.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3sbypghqw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3vrcalodd.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3qqgwehbl.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3htmlscvn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3plgjogqh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jexmansv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ggbrmasn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3kzaywnxd.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lwmbtyas.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hkvjajgn.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nvxlvlko.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3jungemcs.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3yykjbliz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qqgbsqrj.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3iabwpbqh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3kqxndbwf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zguoxaak.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3tgsgbglc.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3yptcxqaf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ltdzalnm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3lbhpfmjq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3byipyivf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3mplaleae.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mijxheuf.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hagownpu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3zyjmarrj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ieyojbvt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ziqahiur.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zvwwhwrh.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3axuojtmf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3azvsjbck.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3pqjrbyni.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3lpmnorzw.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3mfxnxmss.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lxlwyiiq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3btrzmcqs.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3hooewqew.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3dqfkoalt.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3jncxjpxe.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3berxmsqo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3crpvrnpt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3lbvwisdi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gyhfbrxf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bbzsyrkz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3tltwlemn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3uoivtjst.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3qdmnxord.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3qvvbeozy.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jwtxurqy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xiuukkxw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3psshuvyy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ccpksidv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gihbtmjv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3tokcdhns.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3brcgsxxd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3fmxggpoh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qwjvhrbt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3fjfctlqx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3zxcyuyid.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mojivtsk.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3rmzhmzld.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bjozuccn.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zxnxgnzm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3iyobvrff.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3iwvgrtfa.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3fihtynwe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wvbqkmvt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3nurczidl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3wtoltiyo.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3uhoogmrx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3vagueijg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3vhqvdpni.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3eseqhfyc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vtpxauoc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3flhmiuzu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3yvbjumjd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qcvxnzjv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3epbxsmny.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ulabfggg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3onmvuvlt.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ibnvlrqa.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ghkdvmrc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3lqeqgndk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3doxzempd.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3tdzsjqxq.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tzjaflca.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3eilglzgw.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vraxyqiq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3skgbibip.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vvikhrym.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yjwxbaaz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3crbxcmuw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3egjwsnzq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3aobysunh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ffowijqs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zgrhpypw.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3xkwhqtjr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3cocbyfur.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3oksefuka.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fhzhryig.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tlugqytd.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3sjujsmzw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3vewuusvo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3avtwswkk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lexzevfv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3edwrelim.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ekfzkctd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3osaqarwz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3tlxdhhgu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3yfmqjgxb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3sjekgysg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3quqhgmhy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3cfqqxbbn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3umiykkng.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3azitrflv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3derrfboz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3bemzmxcd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gqrifgvl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gopkuqax.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3egvcjudu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gavzginm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bdcconuj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pitjtefl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3opbjdxqb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3eytsonrj.html


<!-- 参考信息 -->