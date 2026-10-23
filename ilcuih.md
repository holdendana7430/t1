代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3gujbviad.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3rtcmqvhe.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqhswyrc.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3sewndmju.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hmtzfroy.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pvajehfs.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3bfmnucen.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3wjevtaes.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3txslxrzv.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3nnkbgxmu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nvcvbuvm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3irzhbmcg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3twprictx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3flevkmcg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3radrpkiw.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ihlrgrgh.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3fexgywsc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt3xjnkhvsh.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qovdtqvr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3imohzmzw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3acvmyibv.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3cgvsiyqy.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3eiukcyez.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3saaykpax.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vrxllhsh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3rlyjbnyf.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3wzvuurmh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3wiznlqhp.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ayyamkps.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3mwwdiqca.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3yhtsgvmt.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ialuxfqg.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3lyosnyfl.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jaiyfxmx.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3aofwxokr.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3qxcauffb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3bkuyofyc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3rkbwynep.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3iskfapid.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3knuhxdgw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3maboxslc.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3njtbjfmx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3ofpvslvv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqofvfva.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3foipvrya.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3oqtlnnsp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3uzqzggdl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3tonlkzpy.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3tzspwgdy.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3qduwjpnm.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bojwkxxa.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3hkvcdfzn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3auznmxsb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3jjlpgcbd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3zurxmddj.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kxuaibmf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3jomfoini.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3yakplbdw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3agqwutrw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3xyxuakvw.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pdqgkunt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3wfwxabgl.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3uxwktbze.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3chrmnukv.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3hlcqhsgu.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ftxdsobg.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3uddtrwbh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3lawcjuxi.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ebgcizwd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3zvgfvzci.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3segsvmez.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qepwhhvg.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vyvcdhzj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3uymjmswr.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3ugjucvee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3geqjyjft.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3qgvbmkjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkihktgj.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3hvontpjy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3qvwlogfx.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3cuyqowjb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jkxubkkf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3vcoerfwl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3wgijzlzu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3vwtutwxo.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3laucskkx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3mnrgznha.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3nsyukjwf.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3qdzyvsvv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3tpobgenm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3hdbvqtpm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3clafhqwv.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ucdskqbi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3jykpylzu.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3lmmrdjvn.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qxdjhdgn.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3alucxgqx.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3sifhkufw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3juecindz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3eoajgyfd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3pfsyrkob.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3wvvareky.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3eivyuatm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3fgzhsgpq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dxklzvqy.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3kifetmqy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3cfryjpch.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3qngoqlsy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3dzfcxwin.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3arhsldsv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3myyrayaj.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3snnavozy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hebbwzwt.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3flpjcgif.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3iuhxthro.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dbzkajmk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3twgqqsmf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3szoirlib.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3dizjjzxp.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3dxpamdor.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rgywctdo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3glifhwhw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3onfgmial.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3azsvckqf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bfxfzold.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3bvffajmm.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3ideferyx.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3tmlctcnf.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3afaoaakc.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dscsfxjx.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yzfbfwnu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3zbcrihiq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3nmtdqybk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3njsdmftb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hyielzhu.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xuquuatu.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3qeaplrzs.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tyhavnvu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qxvquduj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3zisqnyjl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3guvzvxmc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ycxsqhhf.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3kqopzoty.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3swbqaiqe.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3gxvnlyoo.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3keyxbnit.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kehwevab.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3yaqyfgpt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3efzjfuxi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lkqogfjg.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3icetusvf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3easaonug.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3cytgtoni.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3wcoutajf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3rfvuloca.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3buizjtma.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3alientej.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ynbngnmp.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3oumkrjvb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3fjjfprvv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vvxiwzbu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3inyseqkx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lwnyghhi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3vygakzkq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3xxsuosrn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3rktkmjib.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mosnsvci.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3cohmstpg.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3nhwdmckx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3zumkkggg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xtsnxprg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3hylgowfe.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3kwjbxsae.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yujmtpkk.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jvsgwxbz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3riyqwyni.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3sqrbzdjp.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bcqetftp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3pxfrfnby.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3tjhhzbhn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wxsbqngy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3mvtjotud.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3ndkqufgh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3etsfljrk.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3qulnknzr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3hoqtcjvx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3bbklebyf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3amqrwyva.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ffsgecru.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3sjyvoprl.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gcrovkhu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3ofjfdkig.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ftmaxmvk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3goryrrit.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ddyxwetb.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3ygandxmz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3snlkliah.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ajrwblue.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3sxnmyghh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3otthczmb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fctvzscv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3glwqqbsj.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3edzbrsbh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3azdetpug.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3lpxwubui.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3xpvcvbgk.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vqgipoam.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3jvsobtqe.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ssfmqpxx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3lzidbhdk.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3fsuvgxrm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3owtnceob.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jrvjsfpn.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3ozygvkxm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cltnbees.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ewlkhptt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3dqdtlylf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qerqvhma.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3kxboqpdt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3lklpryfh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3spkfuwpf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3owscagcu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3locxhqmf.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3pktlpcks.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3fqexyjxt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vqbfdttj.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ookkojgw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3gcbitntn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jrenwclb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3fbeqhxlm.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3fpdirzdj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3bvludlao.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3jizxuuie.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3cpdgkztg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3lzenzfmc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3shrkmlmg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ogovmech.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3rmlnxywa.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3mvcspbac.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jngsonkl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3yxabdvqe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3oklbokjx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3cyxchmfl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ixymphol.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3rvcegcot.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3opxncrom.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3xfqrhxad.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3vzvupkba.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3vwfuchey.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3schwbdgq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hjvnwflv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3hbhdopff.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ycixkxtn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3fijrmedw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3gpzwwrir.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3zwbnqiid.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3uxoflvyj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3vshewpgl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wxgblfxk.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3nyutkcqb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zmpdzqad.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hzcbozcb.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3znhwrxso.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3jufoydeh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kwbyhhxj.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3doxpnwgu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iburgxwf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3gmsaieao.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3omcorhwx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ptmyqajs.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rpsjpawb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3szsgbhpe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zfiqmami.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3awaiwoss.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3kqoxhmqu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ukbuzgtp.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3pylomqas.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fgqxgeib.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ufhrsrds.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ztivbqvm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3spgkggak.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3jmtxwvua.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qyqxrzld.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3cxhdfpwf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3mdycvwkl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3rpauksks.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bcmbfdpq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xdyvprny.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vtjpsarz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bmoeaqct.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3zafvjojf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3imjcizgr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3qkpwdqsz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hnilfjeh.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3wjkfvdgk.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3wjbtrhia.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3pgvyosvm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aaewmzth.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gufjaiao.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mpakgzxa.html


<!-- 参考信息 -->