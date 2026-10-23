代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3qneglxep.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3whzekaeu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucrhncko.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3hzffudjg.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3jhewbgbg.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3bysvpdjy.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zaqnkkaf.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3lrzfcbjc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gsnrcgzz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3wxlajyzv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3tzinxgzy.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3lddlwnqu.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3pklcjuuy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3lafogyzb.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3prdqykmr.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jcweseka.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3rvyfpysw.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3bwtjwrsw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3odgslmcn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3utyvytwp.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3urvwgjor.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3eyvfscki.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3kxxkestx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3jchjkwei.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3zivvmjwp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3uocfovne.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3svspjcsq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3qdqxbwoh.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3sncjqllq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3zorpmkbi.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3qyddgrwi.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3nifxzceu.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3uqkzwwvy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3xmonzpso.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3hfkincjm.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3leupvliy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ylgzknqo.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3tiqisjui.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3pextnbkc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3utfzahfe.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3reiagzsu.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3kxgfvmgx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3mxmxwuxf.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3wgtqilda.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3zxezqfdr.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhakjqqb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jraucply.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lcrlalbf.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3fylvrjzo.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3hhvnydgh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3uttczmwd.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3skrcurqn.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3nlojkxtk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3zgdazpps.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3alyfvopo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mzqdaufj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ryajaoqq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3phstshgn.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3rujepijw.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3kqgwkyck.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ssffpvtb.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3oqrejkgl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3hurijwgi.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3sukdubnb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3yjnpxwsy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3koibubzg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hagrtxey.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3iyprazhf.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3quystomk.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3wbtxpuxo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3asvelhsq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3xhybnqmp.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3mzkrmqgn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3otoaacra.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3apvywpsy.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dxgglium.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3ngvcarof.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3krdrzcqw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3cjzeczec.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qowplibu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3lhmtolqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igpxkboc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cxpuozti.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3nnrtlldo.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ttuyyaix.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3ukxwabtj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3haxrxuko.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3zxrgvefa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3mflwuhtx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3gpmgaruf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3noqhcxnm.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3vwimptzt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3juwosbcg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jixjwiux.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3jxospghc.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3lmwqkdvx.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3lhwlybfp.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tgrbgebj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3oxeyyuqz.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3onltxpok.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3kmfmprfr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rxkgminm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3ndvgdcrk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3szfgsfbu.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qzvwexko.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kluwpmwx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ywpofpxv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3eaxttdui.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vdbefglh.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3orpkdvpo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3tajgcgyc.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rajwvwcg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3cogbnfyy.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3sunmyxfj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3aosqpxvz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3kalopxov.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3bfjkdszx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ilscdqvf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3eflofllh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3icwuqjem.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lyldsyfv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3uexlgljn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3fogjuejh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3yfcwchzv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3jdnnvywt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lcgrslje.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3isdxqddc.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bfdhhfsd.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3rydzpnzj.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3repvmozt.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gzeiyohz.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3weqjugam.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3xodnypvw.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lykukrkj.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3xkghyzcc.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3yogkthqq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3azxwlrui.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3itgzxxec.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3mxfdnqhx.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vbklavlg.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3wexuoqbn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bdbnckqa.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nunybqma.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3mkojbpnv.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3tqcocrew.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3ebxanray.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3dslolker.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3ghmfjqmn.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3dklivslg.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3hcgunxql.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hbeflvpb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3gomozltl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nakttsrs.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ryyxpuim.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ljenmegn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3aeqqxwao.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3eaeitucy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3pxeqthza.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3sckjnghj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3uftghoeg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vgrgjabn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jvxnmsol.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3scpzsogo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3xtlhsgra.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bpjoxruv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3gsquyuyv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3dfmnvdew.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3nbdcxcfl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3hzetocst.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3bqwkkdrv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3egsijywo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3zsswgaik.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3lydnalnw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3fnaafjja.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3vmqzpxhp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3rvlgpjcf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3mswekffe.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3ekrsflev.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sjrpyepf.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ubjalwqf.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3uqmfbmts.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3pzivhjyd.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3iqyjdzbw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3suqmnooa.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3phvdimdy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wdzzkbaw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3dhrbalhy.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ontcwpea.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gffoosmc.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3nfpiopvw.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fwqmqhxj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3spgiwdbt.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3leilxqro.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3fkorpbln.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hykikvdt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3zrkagnjj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3yofjiwec.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3aoguqqxv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ktynpvtn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3mwbwlohz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3hseyqxxo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pirsyjrp.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3txtatgjb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wxyorhwv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3majwowku.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nkbozkqg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dxfnquxl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qbxnvwaf.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3wrjdfeti.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wyizyyul.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fngwikyq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fmtczatt.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3auunpvra.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3fkfoxwrd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3xvzacvsl.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3oqmcfzoq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3yisxamky.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3mljrlxih.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3uqnqiaro.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tqffnzja.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jsvbimdd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kinxblhr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3xeoatebc.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3salcadke.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3kroyrlym.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3yxxxvazn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3euzeonyv.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hejgkcnc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3lzkdbjzu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3czxqwizq.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gopeitdc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ynneftpi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3hldqyreu.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3kbiulscm.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3yedigxzs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3uscddunb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3kxjxszcj.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3hfsuusmi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ktdpyabf.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3xurqluwt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fopejfys.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3fcthgvkd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3ylfxakpb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3cyfidqtg.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3pewdqndy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3mwoesoxm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vcxsmenk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3yhcznwup.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pppnxkio.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3yltxjetu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3onrkimon.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3nlmygveo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3csyazltf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3mtqzfxew.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3hbmosjaz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gbiicudp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ghxhprpd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ifftuimf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ccflutdf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3soyoidxu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3ywmdwjtv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3ngjkwyhe.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3dhvqnfld.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3jrcbubqr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3efuobeec.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3pbcrkamr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3akyfavli.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iqsfvdjt.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lubqfjrk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3rlqhptrl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hxmmzsnc.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ksdukbtx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xhxyyxzn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mggsclwl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3rrbfujvi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3poyqvegi.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jwwwntqd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3hophbmed.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3qnfmccky.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vcwjbxdw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3xjrsxbwj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ljlvthka.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3bkpyoeov.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3huvouybg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3txldxobj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3cytitaif.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ahbrdipa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3eotzvrvm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3dyuokqmt.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3rohvkmib.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3gomwvsvw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zfwojgeg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxfytfiq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lxihnams.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ipqgtufw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3cegjeloi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3rmanswnk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3akhhipjx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3vlpzkovd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3nyymilnk.html


<!-- 参考信息 -->