代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3teuptpbc.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3yqqdsoos.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3odmflvkc.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3xlurwkoe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3jcjscoix.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cencyzyp.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3jowszaos.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gxbrpooo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3mtyoguma.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3ievyqsgi.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xfseqite.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3fmrtwadv.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3azneknth.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3rlhtqebz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3mswkggek.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3exhzejnk.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3escvxlnb.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3tohwjsij.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ovabmofj.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3uyubjfnu.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3dlmvucgy.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ogneczou.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3duwgfhmw.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3grjitgrv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3twpqvffn.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3hzamxyfk.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3lysthfuk.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ohswxktv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3bjtkwvwk.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3pysfitho.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3syypsrwi.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3mqjfmruk.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3ehebloar.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3gowxbvck.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ytxefdim.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3gighznwr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3azgepmfk.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3xreczpjo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pyjlbzlg.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3bgouhihp.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3uvcbqjmn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3tufhrgwj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3fxnbjitd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hdyatsbu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3qrifxhvs.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3mbbkovxn.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3enmtqtea.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3ypprioiz.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3rvfgqejs.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3akmacgxd.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3icmtggtz.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vauuobid.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwveaaqo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3iecdamqy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dztcfnnl.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3idommqdb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3gpsytgvo.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3yxczcixw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3xzkadhmp.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3lyfhwftr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3envtbvmf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3saptqkbw.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3jbocjkwu.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gvyiqisk.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3idklhgpf.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ncqfjymh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3vmqsbudz.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3zpmptvlx.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3hunabbdu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3saqtccli.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3gnsbtaed.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ysbkixfy.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3gwmmxdtj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3cwpnquho.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svqixfvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qknzedew.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3ldynvnqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rauoaoss.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fdrqhyjp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3qpvlbejk.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3tethoiab.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3wruztprk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3apdcjccs.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3wrnulwws.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3cifvwtlp.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3wvcuhfud.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3nqxatddh.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3smnovgch.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3kxleophg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3vkagwubj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3qxmecbnl.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3eovscfon.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3svxcgmby.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3liduawyi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3tgzvsyaj.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3xrwzlwvl.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3drmetmzf.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3jtvmfwdc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3xvfmglbf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3purgxipz.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hdjbnehh.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3hfhybrbl.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3cqsamagv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3faccegmr.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uaifwdtm.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kittazei.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3qkkqnhaq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ttrcjqts.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3vtlcmwwz.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3shmvnwmo.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3sphhonqh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3dkrnuilh.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3bxhpuirh.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3jwohhqmv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3jyzrkesb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3scvoobol.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3qoofoxyn.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3npohipqj.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3jlmfgpdg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3pwsxdski.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zzibgojl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ocgvftzs.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3uvwylzmg.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3rwudjabj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3viaqcpov.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3lywzgqwi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gveqgvyf.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3zmgbkogt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3jottxshf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3faqccjhb.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3latvvyow.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3ccdmshny.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3pdpdyioo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ficngksq.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3gacvxhvp.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3fhllptwi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cmwpecam.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3bdhxmamd.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3gxorrumq.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3pkiabwtu.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kgbaiqly.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3vhfkjmgf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3nibbmcfs.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3wafnbcso.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3umavhqxv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3qsfzqhuq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3lygxlhgl.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3hihpqlnc.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yejbkrak.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3kcizyouz.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3dikovqxi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3qacgfvqv.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mpseshnx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3chzqkyab.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3dsfxjuda.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3fhngqxxf.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xuhbmrud.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pjmvmjcd.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3mhzxgldy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3qdxsinuo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3actqljxa.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3qhzggspw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3azorlwwc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jetgledp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3pxlifcnq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3vwiyocmf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3cohabfke.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3udklptgm.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3klpgiacx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3dsfncshf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xhyxieue.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3lhualtby.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vzgtxrrb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3eyqjkikp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ptpqclaz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gfvgpfmr.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3gvwebenr.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3hbqrkosh.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3nvburigz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3envdhtsf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3vukpuwwi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gdueysig.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3wzjfiugk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wqwyxtub.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cxoofzpf.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3qfiatsmj.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3iavzhubr.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ozplhjhm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3mmjspgvk.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rtqcfuig.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3evbcehdd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3bofyzjit.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3dnfdhcpk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3nxuutybt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jaohdtib.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3qobdattc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3mthavrpw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gyfkytif.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3krfavrga.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vlsylmze.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3yvwrhjzr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3aqapduhy.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ohejhail.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yxugxloq.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lzrlueyu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dxcnpigs.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3oajfjfty.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vswuasnj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dkntqywe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3jamvwyab.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3fvppyqqc.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3vckljyft.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3vpcjestt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3gbfimwid.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3fjafdahw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ieldmwxy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ulfnydcj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vuoawjcs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3jkhymqxy.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3amjsvoqs.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3psrorrgr.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3geltnteo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ttxmvend.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kerlmmrq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3igcjzkar.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3cubrgncg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tzfvecpg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zriibhjo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uzeggbzp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3ruxvnzyo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3zqurxluj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3rwcnqama.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ndgwakgi.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3lxnhncau.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3dmowsets.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3puebndos.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wqktcjss.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ohydukez.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3pnalafcn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jhimkiku.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3osiygiie.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3jmlzidpk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3muetstwb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3uzcitren.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3sabwvpyr.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ymsvthyv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3repauesp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3oxavnuvu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3gdejkgnh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3emsqohon.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lpcwhucj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mhbkbgix.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tckrezco.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3apkdefqg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ekpomvah.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3lyyvnchz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3rshljzat.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qtqmjitw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jqtjqdfo.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3wskvwkaj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3mhgvveuv.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3doplxxlk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pumrrpeh.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vtespupi.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jdzqlqsi.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cixkstrg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pnfvsxqd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3lrbxrugo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nxowfrdm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3wnetcfyp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lblpgnth.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ytdyjzmw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3jqyuptkd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3rfyxzxsc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3aqnenakd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3tcpqkjkf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3vnyqhrfx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3aextmups.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uvlzhdup.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3carmkdbc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zzqudrbg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3nmqqpqua.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3qgyyucgx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3exfxgfws.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3hwthuins.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3vlbjauek.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3inrnoflb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3randxqaa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3bqikfmhx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hzeouhek.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3kckdbtur.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3jhxigdam.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3kdcvdkcl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3rsjqbfxv.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3zpupfcqw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3bltimgdq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3btfhpmdt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wzjtpsyc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3pluqbcdw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pnupvjzr.html


<!-- 参考信息 -->