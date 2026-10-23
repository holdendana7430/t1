代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3ueisgobm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rffwtzuo.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3twuuisin.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3yvmaclan.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ysvzlmne.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3jckifzrc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxyfqizl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3quyyvnhi.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3fpsxpsbh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3fltejpqe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3rmsinpvh.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3cvzfbcgs.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3vaipxpsf.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3pfnineel.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3tndtkkgc.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3clpzhkth.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jkfexprh.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xyeqqrap.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3tfukfjux.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dfyzlkoy.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3syefbzrl.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vuprkmyn.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3stthdfdw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3furtijqu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3rliasasq.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3uiwlvyeu.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3dihqoofy.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3wxoepkdg.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3cxhfwivw.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3kkrslecz.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3iclvplyw.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ciatmnmi.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3ycvuxuyb.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3fkowscau.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3rmhicqud.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3tjubzokw.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3mdnnfeov.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3iiforkui.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3elyoetdl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3djaozujn.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3hpfbtoay.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3nrknkcmx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3rpqovkmo.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3efnaheod.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3hnvguxgw.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kmcclkxj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ltyigykh.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3legbdgtq.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpqodigp.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3qvvplkzi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3rvccixkz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3fznecodo.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3knisrqrs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3yfcxoxpj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3vvstutvd.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3ibpehulu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3owpurajy.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3zwlirxqo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qifnaryg.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3agextknv.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3kclfjvjk.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3ldceetzr.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3vlgiugdh.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3awikoguv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3wcpyzriv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dddiitbf.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3knjiaoud.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3yuacqnrv.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3jlxrwyez.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3mgabwtvb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3huqgynko.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ucthdffb.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3yzduosbx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3creomgfp.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3gjywbimt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvgvmnyw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3gwparxcb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3vhghbndk.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3voyjlmbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtyhqldp.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3cculfayk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vhqaiyej.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3mewiohaa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3vuhtjndx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wctlwpye.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zzxkdbqx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3egneyyvn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3rvfyznrc.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3qtkrkfjx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3olxvjpaj.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3wswachcg.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3bnbotftr.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3vdfctnla.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3ldmwakfn.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3szjbzqcm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rltdihfx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3nmlfiifi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3jegcugsp.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ralvfwwy.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fystxjuq.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3pbgckrlt.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3xzqbszes.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3brsxtjqx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3euoajifc.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xrwcknjc.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iviqwzom.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3axsnlhbe.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3doovaccy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zivshdds.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3qvskbfah.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dlbuzaed.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dixzopso.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ciwzatby.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3drmhmnpj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3msvfxveq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3zbaqmnam.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uvspoehr.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3pdrjeagz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3pygooitx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3nnvfamvd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lfqjsjdc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hsktzkkn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3aomcangz.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ommjgpgh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cpugokyc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3qijtkxmc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dkflxhoh.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3blqoxjza.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3stzarzmv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3czljtdai.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ingfjyos.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3gxlouxqp.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zsbqcwit.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ricbjdch.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3jjrhyrgh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3gawqrkwd.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3nwpktlhk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3habkyfel.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3stdtbfuk.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rmwgxumc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bvpmhgdo.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kztjhqzh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3bngklpei.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3knkmsrom.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3njnwbxjf.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3xboktgoy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ynylfykc.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3dpcabbpz.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3lnuhhpqb.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3dthrvoso.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3azhdqckk.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3xsizcxut.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3spkqffmc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zvefarja.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3tonvjtja.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qaevxxez.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xlwoyuly.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3upvruvjh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3ubrvkaeg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3kgvugxpe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3qwedhbfb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ykbcyjgq.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3qufzcsdt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3nvywftis.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3hgtrclqv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3rdaxgnww.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pvmmmffw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3skfdfiww.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3exfvuzsd.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3ggqewryu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3pwgpnibd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3qxefqedk.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3udtediwc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3kwbkumfy.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3srzqyyxb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3fzukvwxo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3nepqngap.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3hwptgcpp.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3puigkekb.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cbaabnpq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3lokwmfnd.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3xllmvdyx.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3dtfnrbgu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ympybsai.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gzvzribd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hfduoknx.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3pjehxoed.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fdruykzz.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yxffvygn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3cijxsezl.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3dsyfqtig.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3rhqgehdh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3bldcilgp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vqkxpxto.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3tzccaurv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3eujomjtm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ikerldmy.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3fszkbfmn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wlnfqovb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3nixvwjvq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3igriohhl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ehbjkmcx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sghjwfyh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ktkvnsmq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vrlkoupj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3xcelrtlz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ktkustch.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3prygkobq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ygktxuje.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xrittjtg.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3jwoqdupi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mpssytpb.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dtwronns.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3gubtfezj.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3ckdutaku.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3ealnpjbx.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ttkfjfzc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ivgzurnm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qrpuktgf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aecabuoy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jqdogedk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3fjwzbabt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3fqveozce.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3nyyfigwk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3hkphcqtv.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3kygndkmh.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3oldbwkqu.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qyoivteg.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3qkhzeytb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3plpjkkib.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3iadyndyo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pxaxvcnk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zunuhsgp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3arnnwcld.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3hqnfjdac.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3kondbgtt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3yqdssnov.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3thvdbfna.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ascukzis.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3pkflrfzl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ajhbbgnx.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3hntlcnks.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3bhezeheo.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3wezadeya.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3pbbyprhw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3jayadobc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3tvmqmdkn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3cjfgkcfl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pfudmpek.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3qhzzcyzu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3xnwvvltk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3toagpasb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3acoozihi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3drrxiepu.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wytzvakw.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3alfyjtue.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rngxhdga.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tjwlkfzg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3euqiaitk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3dzlsoauh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3oanraxsz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3bfqlpyqk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3daysyeyz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3rirhwqed.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3rjzlnsab.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fcadplox.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3fyitkfal.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ebcensey.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lxezqagn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kndxvxzl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ekwjarwm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3rzepznze.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zoqzhpsv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3uaumaegx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3peaznqfl.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ycxkeprr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pzfdxmmr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3euxxuzjk.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3lglvagqt.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ojkcwkaj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3jrmwnrou.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3syijpftm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3upfqopow.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ubvgubnw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ohasiqqr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3cbbhjzda.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3lbmvtodx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3nvaislci.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3nkezbvke.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ftadfrbn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ycntlqfe.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hnhwgbfe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3apzxobfv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3gotxfwkp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3vjjyqwpb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3alqcgjmv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tikkxfhf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3sfhtjvdf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3afsnpzir.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3vkyhpwsf.html


<!-- 参考信息 -->