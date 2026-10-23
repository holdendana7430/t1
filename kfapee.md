代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3levnypdv.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzorrxtn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nztojerd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3inmtwwao.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ttezoczk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3quztqluo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3dtmhvrrv.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3faxlhvfp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cmftjpoq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ykrikarw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3uiaoxggh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rtirdxgo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gbahnikp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3mbkairrk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fzlpsept.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3lxribsrw.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jnawnzso.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ozqlliqh.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3wcmibzbg.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3xjwwynvn.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3pwasxmdw.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vibogwet.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zthszwqr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3vofdafwj.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3uhvtbkhe.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3pbuzotkt.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3txxkahmi.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3bcqzvini.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3eqoudeqa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3ainpphcw.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3llqexaam.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3azimgqcx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ztykqxdi.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3vebulxbu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3veypesoe.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3mxtyqzuz.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3zwzrpswj.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3edoxoirq.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zgotadce.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3syhiybau.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3btruhrfl.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3ljwwtstc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xolqfkbq.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3wjqdnmbr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3phupjxky.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3opgpcgcb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3gidplsma.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qjkowqki.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3wywrtsrw.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3tsdqgmoa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3ggwpczgw.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3errhpcix.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3pipauogu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3hhoidmsy.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3itijrtio.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ushxzsga.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3vaeelbyh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3vaoejcgt.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3yyivazbp.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zkadelku.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3hpucjtkc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3gafzdnqm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wzlvycww.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3jlwfxcgm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnzxisiq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3bjzzkhmz.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3hgcnkmaz.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gwyxnyyd.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3yekkuebl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gklnsmza.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3dwisfjmq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lqnvwtez.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3mlkujaxe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3lucwjzfk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3cqgntqof.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3llabwiic.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3kibnqlex.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3zbnawgra.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3upvfvqbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zdzrhlbn.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3zbtvxcvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wpoykcbx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3raqshwds.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3istemuch.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pcxnsqze.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3tcajkhyr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3tnexbxhv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3veyyxazm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3yhpgdmuk.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3lzaivajh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ypwvashg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3xphlobij.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3hygvshac.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qukecplr.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3feiumbkz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3eemkmxqr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3embkfhpb.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3uudtagnh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3otedhuwm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3gdoogokk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3cakaeavn.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tddkxofw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3hfavsxru.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3cckyzjjw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3kwhithdc.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3svqhutym.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3vvrhiqgx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3lcgkhqxc.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ahmhuqne.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3uutifhkc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3kaqkpnmo.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3eobnttjj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ulcyswhd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3luchuitj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xlsdarcx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3nstphsmg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jitmdntd.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3bilxupdy.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3yeorhpdt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wbsxhksl.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3yerwhvlw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3twrutzne.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3dvbbknfw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xqrvaepm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kapnsrpp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qrcrxkvy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3sawxsgaa.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hekezgzy.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3slosbuwk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3onqfpwjp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3pdkcxsbl.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3vbsrubgd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3fmnipsip.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3jbcembsy.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3foznikgq.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3qckybfnd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3jdzuxifb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3bysliysl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3rbmgwhoz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lejnbqkf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3odnmhvds.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bpsnuaqz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3lwzehbbx.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3nqdbafdm.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zxroypsp.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3wcvogipf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3jyfreodl.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3yycwbjdp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3lnskmxjr.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ialjcjsi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3fkrgkwfo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ykcteivy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3tnmxjcvt.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pjcdundi.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3jzdskocu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3kzguwbtn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jihwyevr.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3kxaqszxe.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3rrejzjue.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3yazpkwlh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tyijvbco.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3amqucadh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wkxbukec.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3vxbdgmta.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fegexzio.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3mifvrtyz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ylfurhib.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hnxeqroq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3krlwmfyn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3rbqlbthh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3zfymmcbm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3rxcgkgtq.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3heztariu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3xhptkobh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3zjvyjaie.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3wigabaqx.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wviblmaw.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3awueloma.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kiudkhma.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3hgjhampc.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3olfjicgj.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rsyawddq.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3brxyutlv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jtrfzjjc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3katyorae.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mkbbbuko.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3ezkjzrzz.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rrjeoitx.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ycpwmvxo.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3upnexpfy.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3aphnqtfj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cgzzookk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3uhgxzuqj.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tfjddiog.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3iithlahy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3souupoem.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3fgiacabl.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3bclptzds.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3pdqboxwi.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3uwepnyvs.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3xgdtmxlk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sytoxnky.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lgzauhog.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tyxjunfd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ouenrhjp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ppyibdrs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ggciljyy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bujczeaa.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yzvyatnp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gjywwfgj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3byszaslv.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3aypazktf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jbvbszkw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3mvdkvhgs.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3lstakchu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3vrdgyzvv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zmydekjv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3aajgzpox.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hhsazaof.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dxwbuvat.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3xtkqgbqu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dcquxjob.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3fkcqwfev.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3nbrxhmms.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3qavibdsl.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3kjymaxzz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3yosntbid.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hrpzcmlk.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3zaghjtjo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fgqpnrrl.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ewoizxux.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3sdiumtvx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dhjohuxd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3vrndhssj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3phykldmg.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ehgklyaq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nwryanlr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3oeramwrt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3vsocbbpa.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3gmwxyewe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ngjsrycb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3jiodvlkq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3amyqllki.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ufqmqqmf.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ivlwivqy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ysxhcksf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3cbohizxx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3qssvqjlg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3vmsktqos.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3cadoxbvo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3jtoojzlc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3kcbnssnr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3tmczaiwl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ukhudvfg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cfftkebi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3tsorrqam.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xkeyvyyj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3aybtnhlu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3gvomxxny.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ydtofoyz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3isrhjmep.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3wyvgzvcg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3raggdkdo.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ffxbhefo.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mcbedaag.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gentonfu.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hkapmeas.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3iikdhtvk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xisvjvjj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bvpbygyj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dwqpecxq.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ajgzhudd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3jrljbipb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3yqefedjh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eiyprqmm.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3twnylhxf.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bbmewatm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3irdfgdfn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hbtbokra.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3eiozrtmz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3yvzffeuq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3dkznktrp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3xqsdrclc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lervlmod.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lwekndzd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3bpftuzpi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3ppwnfudu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3xtoltidn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hauiyllp.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3fzcxdrgt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jdfidtvi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3yvwwrqtp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3ncqjbrkc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3xcukyldt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zxxvbuoz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ysvmkmgg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kyaypmgr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3mgenjmhs.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3kbagycpn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3yxgvlsoa.html


<!-- 参考信息 -->