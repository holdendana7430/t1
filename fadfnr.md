代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dqbkqnzc.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3ldhdaybv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3lrmekdiq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xnybvhkg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3tdtelmiq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3rbocuyof.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3zfkwzjlp.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3giazbckn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dyktugig.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3xjukzbui.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3gskpgjud.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3jxdnjmyt.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zrwzwkmn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sbjrirnb.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3envpjpyq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3niegujav.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hcpxbyho.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3zimjfpvl.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3omjxwwst.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3luqkjvrn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vcdcipuh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3urmzonck.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3qqzhxtyv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3lgtvwcod.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3uxpcbtnf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3gijumsfq.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3bmzvqszd.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3fsdrrehn.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3xcroehaq.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tvsqfymf.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ayhgvcki.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3nppxrsnb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zjajigyc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3nassccnf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3vbgpxcrn.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3dutyvvyi.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wshaiuja.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3spmjjmmj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3knhxhxib.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3tnpasmeu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qlfvwfrl.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3vmlociyp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3rrdbjsnk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ksxfzjxi.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3aooerxef.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3vibaoonj.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3qyovxmwp.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lpvdcjfl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3czixyfkn.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3poyouujy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3njezykuo.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3knzoeuns.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3hhqupclw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3bxonbmlc.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3kottdbhj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3pbpliitr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzbaiskk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3kosgwumb.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3qawehtue.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3jnwnurhi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3mmenhvyi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3azmsgigc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3blxgwmcv.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3izqbnkgg.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3iwmeobvi.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3dhvciorv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3ffvzdnaa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjbnckkt.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3dgxamnmx.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3rxgcabpx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3lkkaeami.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epodfcbk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3hvccdkuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dxlnzyjv.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cnovgcgf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3qckglkdu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3afojswiv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3zwsoopym.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3uektewrw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3assekdyw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3xgarrskh.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vtcwipfs.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3fgbzkjko.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3nkwncaoi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3brgqdcey.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3fjisvgwo.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3zyzbxysk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bpocqjjd.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3coywgnzw.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3jcszmdnf.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3ccgfkzwy.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bsaowvrh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3scxhqhpu.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tyhtoxhz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3tyytasxg.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3njyqluco.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bntiewam.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3xudwwdku.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3bschmdhz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3jivoyjzw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3blpfwlxm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3cgnvjekb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3znertbkx.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mmfdiucr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3scdwkval.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3hdomvoeb.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yimtkxdb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3oofpdbam.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bdhlwcij.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ffektjgi.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3occugpyf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3scsvwxzo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3kampcsfp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xcsokqsu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3uddprrfj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3jchkxupq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3kuqbfcak.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wfigbqak.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nhxtbnpu.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3abbafojr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3piaupvlz.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3dmsoejgd.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kxgvemow.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ublnddzl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3blxanxsq.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3drhwhtcp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3zzuxlibh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3apnwuagw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3khcloblw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3tharqxwf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3itdgvzkn.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3asmsrfxh.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ljvacyeb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3flzwddcz.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ywtxrpyw.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3adxpakoe.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vfkdaunj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3redkjobp.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3tontwbvm.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3rufusist.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3hcfihzcr.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3udjkktac.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3oljpbqde.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3inbsvuua.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3wqlmjelr.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rsioebyj.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3mzlecolh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3saptzbxq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ibwmcrrc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3xgdcnvlo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ubsjtrpv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3dqeppoyv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xypasezc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wneltbkl.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3icabeent.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3nkyqygrx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3njbtvwdt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gjbyqrwg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3fdbadxtm.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nmdxiunm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3pnaujtyr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3qbtbwsut.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3xvgajbhf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3xcpgdwxv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ukmsazuq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3yfmjlskt.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3tsndaoja.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3bpwatxpe.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3hitlizsy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vjvevuet.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vorbbhkt.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ofyrrvzr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yvssnwwh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3vvjfvqfa.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3dktrklvs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fswfdjup.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3shnlsgpo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3sauyxusv.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3tsjbfqge.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3emcqgnpb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ausahebb.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3aqxuoobf.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3vjejhsaq.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3amcsjnjp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3gljphbkt.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3bhvrewry.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3bzkiembs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ocqdtlnt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3fccdhjvf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3wjotfimb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3toidgxhh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ewatqxvy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3cnunvxvr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3odtwbkcz.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ozdspeec.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lyjcuaig.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3dvaveuqe.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lmfkdgyh.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ydtohzzr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mwaxcvkb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tirqjahu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ruvrazzo.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3srzhxtbs.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3wuhamnpi.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3admpkoix.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3twegvthd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3bxznicuw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3aruvbvef.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3bgemzgcz.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3oboiskwi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3pyrmrmcf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3focgbkyx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mfqhkwyq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tfcroprc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3teijwdet.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3esrkoemz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3zotstoow.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3mzanwret.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3jazvzmnv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bfkpfqza.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3tkjtgnbn.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3hqjnsffw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3flidletb.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jaozlotd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hbelmejc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3igcrkdcd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3jogkoxdt.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3arittiau.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3sevjctye.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3foxarjbq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3cidrddkq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3lxyhgnbr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ifwmnltl.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3zzshtpwd.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3qpnedcya.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uoilstsi.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3sritarse.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3apcakhbz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3teyrmwkp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3nizzbhhl.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3flonmzkh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3dhemdcya.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3vvrjtutb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3zotngtsp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3pgyqftmk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3zzmostxc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gamgkahz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3lkfjmzpn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gdyzpycv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ckbostyq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3xfsixoim.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3gtflivut.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3iepqoyqb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ytlppcgx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3wvgrfmjh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3wqrwliqy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rbkppxip.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wjyldjiv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ogwmfapa.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3lqcucnbh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lkkqqico.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ltzxyuni.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qltzljug.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3bxalpqjf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3rajxujzr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3pkkvhnpd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3jlkcvosn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3atapiyoi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rompriqp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jgaejinz.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3tzywxgbx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3vrelqxis.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3aurnfufq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3xinecpre.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3fcljrrav.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rkvuoisk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zjwgxhrc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3plimezsw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nmurpcsy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3dmakoqeo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3qjdjvnby.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3atvhpwwt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kebhkgpr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lwpizufz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmzccuwu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3welnlvhu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3heywkdrg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3vdyzopuo.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rasbllwe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3dhdfnnog.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3dicxhucg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3clgeggit.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3bbulrriy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3azncrfrn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3sjsfqrvq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vtbrmzze.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3wkdrddzk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3klfleuxu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vuzqawze.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xpjhespi.html


<!-- 参考信息 -->