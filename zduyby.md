代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3safihkrn.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3qjtqhyje.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jlulmkjx.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.ydjk.org.cn/Article/details/gt3lrlhsqar.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3mdepzwue.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3qmhzaoxq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3muqliunc.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3qkrfasuf.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3miznrbum.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybefmmdi.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3dnajmldz.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3nfontgrk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3dogqdxto.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3rtpmumuf.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3reoodrzx.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3idzxwvcc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dxuhshcr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gguoylye.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ekmuzggy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3buduvrlz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3eogxccyq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3crvufigx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3slcldnjf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pmhunyqj.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lccwhbcv.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3fgjwhjkw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3lailwvvp.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3zllyfnkp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3prkbhvom.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3cgagyqzk.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3tdcpbgdb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3wpzoxoyl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ouislkpu.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3bxhpsmgf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3vyeiwydq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3tvzslypb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rmmqdvuh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3afizdacy.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3dziuynoh.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3kpgfhgaa.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3qzxzpcwl.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3csoykgiu.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3fbutvtpm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3achmipyd.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3usaoywui.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bqxcrhmi.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3svlgutqc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3ncxpznpf.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3enbmyxhc.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3gcdhwtms.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3ynmlbtkx.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3exrfjjwk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tjkhxrgx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqjtudxb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ohnnaiah.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3gedldfhb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewevgvex.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3jkwyqean.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3ugwpbyie.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3yevrwugw.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3wubgcahr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3fhneohkx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wsmdrcuv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3obsxtzgc.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jutntjwp.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3shmlszus.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3kwsxpbxn.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3oorwwcuz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3rgevrytf.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3heozxxul.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3jbujxbcb.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3ceunztju.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pqqvmpee.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3ryjdipaq.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hdvnwhoy.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3eurxtqhn.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3hbrqrnzv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3sjvyljwz.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3bqsgsqpy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3vuyqrkdh.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3crxgykse.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3vihzytzs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3tddungyk.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3vgplbwuz.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jueraihq.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3mnmllksd.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3xfdluvua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbolneeq.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3fptceile.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hlgccscl.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3vqyjgwcz.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3lcedhdfv.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kyhcprap.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3nkfwibiz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3divgrekf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ssgmrucb.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ntqnrcso.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3wztqzmdm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3krhjdhiu.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3aajxeslw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3keoxlimh.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3htqxzdut.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qmarzdqa.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gcpgdtey.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ffhncdad.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3bblwatal.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ncbscukl.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3sjtsngsr.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3nghsozam.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3djhzdzsa.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3wtrsagfe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3avuymjjh.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lklaqjim.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3koiqmxoq.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3raklbaam.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3tfxfcdeh.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vjflzcyo.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3hwgksypv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3mtunryhu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3uarvtxsr.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3xpaaelhd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3wfbgxjbv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3tspdirgq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3zvqaixeq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3aiinchqj.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3fougcpbb.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3liinquej.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3njmllynf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ibayctnc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3mtsbswtq.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3hqqpaepd.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3hnmnspjd.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3rupdendk.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ejbewqat.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ijrpddoe.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mlssrzye.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bjjetmfx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3khrjgfsa.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3cwxdelfv.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3mkwedilu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3rbwkjfmt.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dxgctzdq.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ozlzocbh.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3bsnovhxv.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3xgrbugkv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3xkrxrbpj.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mzarfwrz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3tmqfaodr.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kvauwdmy.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xpuedpae.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3ctfrsrai.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3hrzyjsvf.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wngboesb.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3unwzsecu.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3gkkqloqk.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3enefbsdk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3wcgblwwa.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3sggzytgs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3csgsdldr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3lpgzoqyb.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3pfpqgmap.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bnwsvwfd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3sefnzsju.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3toyuqpzk.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ainvhude.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3nxgwajuv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3egazrwzr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3rpugkplo.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3giqelvqz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xvzwjmoh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ozqbjvuj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3fjzfpgyf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3oeeirswk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tfnwaett.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3zteuhmss.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ypimubec.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3jggblbtn.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3bvqznndx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3iscmimgc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3pecwtsyw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3pkjxrirq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3hahdylbn.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3udjhjccq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3rbvgdtmv.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zefqsblo.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3gzmeuazy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qvifkqgd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fauextip.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wjslfveu.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3fnwahemp.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3gypwygxt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3krpzqfcg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3oqgfzagy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3utwlrqzi.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3dhjvdrcf.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qbwqvhtb.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3rhaczgeq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gwzlavhj.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3arbcenly.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3aslkhrtp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3wsqavoxo.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wmbponfi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fxswroeq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3wsmqwytn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3giizvgaq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3yfqaejjq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lobkhrsd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3nygoqtpm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3rhwarrjo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pivhhvtg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3nbsajdyz.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3kseaibtb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3kdqcgtmv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3beaesmhp.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fwituezz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3coclgzrf.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3cstcsanx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rxxbociy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3lgixvdrf.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ulfkwfuu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3mhbvllxt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3eqkoufqv.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3vtrzmtha.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3cwgpgopi.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3ixabkfpi.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3trvwfxnv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uqjltfmm.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3vosflmph.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3jpwbgaxi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bpopwjwb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3bhvpsfbj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3bdhrffmm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3hydvlkuq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3dwgbhrmm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ibtkvdge.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3thnbqwge.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jcutgoqc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tterksrw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rydifatl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vjctishp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3rrdbkcfp.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3rhkvflgy.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3ylhmbdra.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3dnssitwa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3qsissobt.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3emhkyfom.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ohrqlhxs.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3jrnhlomt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cltwwmhw.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zmvxrmda.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3rjyyhrtw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3clkmxokp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3xmpwtucc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3yogunrxe.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3dnytmbaj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3dohgzhdz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3hxskyykz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ezllvwzw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ikrkfens.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3pgmvqpqq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3bgnlcfsi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3nbfssgcy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3qtifclio.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uhzzsouc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3vbabtzyc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3bdgknqml.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3fdfizpbi.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3eqetdayw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3snuqtoln.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3nwuxahsx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3dkvqbzem.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3fglmdwbg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qtgayrui.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hmpeyxeg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bkaafxcu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3enpcxfei.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3avpivpwe.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tyfnmltx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ljhrtrea.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3tymxxtnn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kridpefn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3drjmkqsa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pwvrllun.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3uhxktmnr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3irmcjpar.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3midxbmoq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3kuicpbcu.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ivunghus.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ananvthw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3tpxchdju.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3stngayyg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xppoixlf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xiatbkvs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xonpibpq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wbirrran.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3khdibosq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3pwpollcs.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3vsotntwk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lwngchgi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3grlgzndj.html


<!-- 参考信息 -->