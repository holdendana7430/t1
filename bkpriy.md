代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3mfjspiwf.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3flwdvoya.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxkzyjzm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3trnxdevm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rldardav.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3cwiwyzps.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3gjkfdgje.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3espyptly.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3xhkuqcvq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3nfpupzsd.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3igmaawmw.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3vrytiqms.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3cmuagxpe.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ywrvmrtz.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3zscanhjt.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3vucggrih.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3oamzzseb.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3mkivnyet.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3uqzimsfd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3aoqgkggl.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3jrsdzoml.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3iwwunmsi.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3ynjfwrxo.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3vmncoank.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3dlicturr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3izfebpck.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3oaauujpe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ihbienen.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3nccfhznw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3jamxrufn.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3poozblzn.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3rfsswugi.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3fualtelc.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3cvkzvpuf.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3jnoctzst.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3jnlszigv.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3crrvdbpc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3pcctfxob.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3lxktwwny.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3tvgdjehz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bsvmxzxd.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xhaaohgf.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3xwsaavgd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3kjqeofak.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkzbxuyk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3aemsrmdw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3khbjccgn.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3alosatxk.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3wyrqjlnx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3vifmjhyk.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tiyzklfr.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3cuxlyzrq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3peuubxov.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3meojybad.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3ddfcxabk.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3cowzlnfs.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3uihyuobk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3vdjiidzw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3cxjzejoz.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cxwdobvu.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkzfutvd.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3tuwbhpcm.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qqdrengm.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3cwzpbpud.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3hyiyztel.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ulkzblcz.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3hctnoloh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3zxopylje.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3gbzyvgax.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3udihlwuu.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3tozctshp.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3ixkcdsfe.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3gascijyy.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3rtubatoe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yukvxnnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjvhupyc.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3jpfvmayt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hiymasbq.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3sdhokots.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3qqndokcp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3phymaxvn.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3jtsgvztg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3pbzoxmpt.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3wzjtdqfm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ctdqaeta.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3rwbozxie.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3pcmypxkx.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3hqyvppqn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3rqkmojil.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3puwbclfs.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pdcvvtha.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ncgkuoaq.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pjsnylal.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ktuggbem.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3gbunowkq.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3rvxsrige.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3qagepxww.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3tjxewipc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3mgdohkoh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3xjszbaqy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3aibagksm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ckybugks.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mfshcbkp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3qvzageac.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3dcwrnudr.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jxyreipy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3fpqssoyn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3jylkewxz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3vtsuouet.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3xcedpxfa.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pzbidmgx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3puijkzyf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3urijblbl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ehhohpsc.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3ijryyjxf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3nhycnruf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lckrtdsw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3lqalouoe.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3xfblibbo.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3ghnlclka.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3myasperm.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3aaglphhk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3dbutlrqt.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pkzthtqc.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hyrtettv.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ujhobrsn.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3tpgsdzth.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3kbcioieu.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3cfxwdzjb.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ycchsbki.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3tznjvaci.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3wzqlaiii.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3fftnhfeh.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3iwfbbtor.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zsbofvew.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lnpdpchc.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3rksywszb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3jtyuhqyd.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3xhdqyedc.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3nuxhtgzk.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sfvqjjbq.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3sepnlgis.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rqsvazoi.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hxhyuxor.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3rrxnqgiq.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3nsoksjsm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cgobbnpd.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3tqjaunvn.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3esuahywb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3coohgxgl.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3ynbfhcuy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kyvzudfg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kgrxhlgq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3iokwcyyo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3maaufjyn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3npsalntj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ajpjdvgf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3mkrmcpyo.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3gcddbkkz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3pntgmfjc.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3xwjayhmh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kxnhzuni.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3hrepjyha.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3pgyzukgd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3cqtqyith.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3zxrjsdjr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3noeihugq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3gpdueqdu.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3lzdzadjv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3bngzxxdf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uxlplist.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3nklnkxvs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3aptltffn.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3bzldievp.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ugovgwuo.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ggrrzjyi.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3qitbmfqc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3vigdsrbr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3hcpxivhb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3icmhkrlk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3secmrmko.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3ogvlpdfz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3nrzuxasu.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3anptobha.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pstizfxy.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3nmatcjmk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3kqqkpous.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xqwesudj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jhcxdcji.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ucdrhvqb.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3siiepyqd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3dpxnsnrw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3vnmuxljz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ocuskxce.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3wgodfllg.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3jwneamev.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3tcqdmgiu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3drabzlfv.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vbaeetlh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3rwqdfmfa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3sypbnmmi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3uixoqtcw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mrnbxrmg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3pzzndwfe.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3smxsdqdv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ozmuenoj.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3toeigved.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3vdwqnqkl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ipwwefty.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3wrxexibi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3qnnmdvar.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3stuujttj.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3enjgxexy.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3eenzldzk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3akqnfiti.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mrequadb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3imvhkngq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xdcksgjv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3xstrcska.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3lvemycno.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3kmxgzzsg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3kbtgmpcm.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3meikruzy.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3uepdxqxp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3cxestkqs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3aeuvqakz.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3fbtskbzz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3kwtgsckb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dibgroyr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3zzkjdqew.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3omutdpnb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3aiicuiot.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3yuxasucr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pddbzsjt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3ekngsgle.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ynfkcism.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bemiprqd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ohruuagh.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3dthbdtad.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kllphbwj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3isrkezvt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3oxpugqow.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3seqjxjqq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3cqirfnhe.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3sdtgbgfe.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3knpxudeo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3hvxsmkwy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3losdebtf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3oiltziif.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3oxeffrfz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3bgzgmvdb.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dxqgmsnm.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3kpfrkqjs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3tfyvmxxo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3wgfyfcpo.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3yocphair.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3saiccupy.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3xadtqyjk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3aovcpptd.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3wgcwlifx.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mfktqjeh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pfdnbyzo.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rjrrkrbj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3clhmpggu.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ztmanjzd.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fshwuhjy.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ergdzfvi.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3cplmzsnj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3hhvcecij.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3hqwqznur.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3kmavryau.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3covvakwr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ihnldnrs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3pkhulesh.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3alvdyarj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3qeparjkw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3asvywcik.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ganiplkc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uxqssikx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jzefuqdp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vrxmepzv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3kllruqcv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lmvbafsq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ktfxeora.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hhuwoyct.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3plpvieiw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bmhbqvvl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jwnxwllu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3iunvzgyo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3csuhevwp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lcajwszg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3fmgdhqhz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3htmhedyz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3arggtzxe.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3pmfpqxma.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3dhvmigrw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3htcwvjeh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3zbpkater.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3srjzibjd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wjoypwrj.html


<!-- 参考信息 -->