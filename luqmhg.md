代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyhufrfi.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzsbtqua.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3kiogzsrv.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3ratzvltl.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3akpmdfuy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3dtprlouo.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3nigzvaph.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3bkhjbrqm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ssfocgha.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ekdfxnlx.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dixbzifk.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3vacxdwdu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3ogjovbip.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3ivsuzavk.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kwizzbsy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3sqouptsg.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3irvflliz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3fhnyabae.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3ucgzvmmf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ilfzhwxy.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rmqibkfk.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3miiqkopm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3peooqena.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3lcuydcty.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jbjcopdf.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3gfbjapyb.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ggkobanh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3sqdjxgsw.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3hiqtphhh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3yjdormcg.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3pkwpdugy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gdcpkabq.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3mekemakz.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3hcdwotnu.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3gaaevyda.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ppguqqab.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3yhnsswbx.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3aemocoes.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zbjyofra.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3nnukjxef.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3uxpthyho.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3vvgqvyew.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3qwwzoppe.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3hsbfghot.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3wvdmubmj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofesawrt.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3shimtbdu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuuwxosl.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ylivkdzf.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3laauwshf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3qdsiwywq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3wtnpmyum.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vmhhioga.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3zbkgcjag.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3shhklaay.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3chnpnrzy.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3roftxnwn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ouzgpiwb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3spcsqvpl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iroxbkxt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3iobmuqos.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3wwoelfvl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3wfznjrai.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3bgsqmcly.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yclqrzle.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oywddujb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gybbyfyl.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3kmktmlqs.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3vahkedkm.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3qjrydors.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3styaopkr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zsolvekt.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3qegadxxm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3qisnadga.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ckuxmpsg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3kbgalmhx.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3qeydlgjs.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3bktuzpeo.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3uxenggau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dprhypnh.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3ionoytnj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3skecgogw.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3csskwbqd.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3pvhkphcx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3xskstryg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ffgbqjcn.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3eqnutezp.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3dizkmcds.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3enshgxtx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3uocyrlnk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vjhqkjhb.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3bvlfyfhb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3shdpjjwz.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3hdxukmwf.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dqqasbjm.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zakkdxii.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rblxkfxs.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3cbpapzwm.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3lsibclos.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3pzxmuusa.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ntisxjdi.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wdnwyqvs.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3fkiutrem.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3ejpxhchu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jdyztday.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hkzeogmh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3dvcrjyrn.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3cqhyeihk.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wiopikkj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3oxiuelwx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3icxojlpw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sbjefxin.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3cpuyrayk.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ttmyipzj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jclvcvot.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3ejdedpvc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3jfhdxphm.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3fibabxzn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3azsulmov.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rkuogwnp.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3sxhqmdmp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rxdnjzws.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3gtruszer.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3szplkwcc.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3khoqosri.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3wxebohpy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3cquwzzha.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xvjuqxly.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3juzzcnpc.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cuevmwxa.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ghtihsca.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3dsvlhako.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3mpuepepe.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3oqyvcmsw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3traqrcob.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3jjcjihfx.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3kvsfhxhs.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ruyesams.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zyduphhx.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tsepqzqd.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rxnbuyaj.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kzpgtgxl.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3fdrrrboa.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qvapaxua.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ajtspwsk.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3uqgcqcxe.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3dhppjghq.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3igdygene.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3kiqwadyy.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3gtbblhak.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3fertiklf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3pbbmghox.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3bvwrzhnd.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wgskizzl.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3exvzkxqo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3swimkyqm.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3fkhbwqmq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3rrwakpwa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ivspqjnr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3uheldukh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hgbxfxqv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gfjiaccu.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wizjcygq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3cuhoyppb.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ehkhowml.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zorufbre.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nfvcihyg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hzifpqhj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3qwratxmy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hsgsodfi.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3rbdlrttx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3fifsyoor.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3dmcyjzgn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3eojhjnui.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3psyvcjzl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3hqgbnqfv.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3rqjiguoh.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jalzazdo.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zerhvfij.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3euyfxwkp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3dkpdbzhl.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ublaxctc.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3uhntdvuf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3pncrofih.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ibajhzrm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bbpgmndm.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3spwjjvlo.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3enodrzda.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3bqwkiffh.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3amxjznet.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3yczteouw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3tdinwypa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3bzffqupt.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3iittllbc.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3cgxvnqqr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tvabvvjg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3txosptxz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3drjghvue.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mgmogdqq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qdtzngfn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3ytjrprzq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ebyrgoag.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mhkypkee.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rcgopeff.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ubihwzmb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3fmfyxhmt.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3kpyxqdca.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3amfqrwuf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3lnifvong.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3lkivcipc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zocqkdzf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zwmacebq.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3iibnqdpr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3yvzoovqt.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3jziturkl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3gfnecjhg.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ycomdcpy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ndmyhzrr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3tdkxbmzl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kgykekup.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3opmslovi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3qdbhyyji.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3uoqpesjw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3tvzgzhco.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jtbnyirr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3umjxbjnp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3kiqxmbhz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bccxchil.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ipuiyroc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3mjhrfjlu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zldoqmmo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3unkcxnft.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3resfijrf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3ehbhnkjn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3loafwvvp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3iqjytdpv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ydbwoebi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ijfbwnvr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3uiwmixye.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3wrtbjkjj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3orirtjam.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3vvapximf.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3gxnwywbx.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xqvjziyx.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ydonwotp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3vhlliwdy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3ykdkfqia.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3xnebrezk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3ogdbmsey.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ebpuvxjq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3jdzlkmet.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3rfjdndjs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3etprtdua.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3afocbume.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dofaaskf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3mdvhxpxe.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3xtpfckzy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3hafxiljq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3vfwqfcad.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ldwyvzte.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3doefkmtj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3dqvohwzz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3pkshzupf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3nlphnncd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3vishpekf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cfyntjoq.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bkamnpds.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3yyalupaw.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3emknzsnb.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fhsxnjih.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ijgyqjzb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3xnlqbpku.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jjulkmkn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3gtkqrcvt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ddppzuqe.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3xrhlfkfu.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oxrgdtzn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wxikqeaw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xprajrjy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3oiwexque.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3mkcrwdik.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3jtpjrqfa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3gdmtgkuk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dmellonn.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3lcepfzjc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ulphdkfg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tjjhyxno.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3idmrxpgl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3wdskhdgk.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3lwrpuqax.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3afomjlku.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3hznkefhc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3qhwxtovi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ogqamusq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pkgodvas.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xizpehfd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tmymligb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3pacjjoze.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3okzupogc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rbuossae.html


<!-- 参考信息 -->