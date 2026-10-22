代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2dzxnhqbk.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2cjfkiwjs.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt2wiyktsrm.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2oodzyxfz.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2emrzqvva.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2wmpebgco.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2wcjvfcvd.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt2whlunjin.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2etmqeagl.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2rdunovxg.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlpadadm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2bviqkubm.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hiiqxydh.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2eaqsxosu.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2tcybxgyn.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2zpqthhdn.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2luwdexqz.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2adzjwivf.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2bsfncafh.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2xglaznmy.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt2dpavemma.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2walszafb.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2nhsompeq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ybkcmisj.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2mxbugqes.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2yuipwqtl.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vblytieb.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2syukkxum.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2ouxdnmqi.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2kuacshfr.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2sqkholao.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2pxmaaaul.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2omogjxsi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2ehueptxh.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2rysstxuc.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2acwxviyg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2bwulyxna.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2wlexdwkl.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2ouxybhfz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2yduwztzq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2hllanvhn.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2efcijxju.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2miearanj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2yuukjdif.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2izimsfoy.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt2ryvneedt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2vnnwctxz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2mrfwdefj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ovhxdilg.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jzctgfyq.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2xqwwljyb.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2eqasevaw.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zpwyunsm.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2furlmulm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2kjpgcadl.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2awuxgvyg.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2bglqzvls.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2aetyjyvf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2yevaaslr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2rqlmmosj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2viiqvbac.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2frwrharu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2fgholpof.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2aeakvrlo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2oyemvmty.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2zpheidxp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2mtuapesr.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2kjpmortx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2blgxttna.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2uckaeakn.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2gwhxqxkn.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2sijgmzlr.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2futvbnuz.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2fzoozdes.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ompesiny.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jmfaeekt.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2otvmnqsz.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2zbebxegm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2rzljizhg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oifrdtuh.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2vikgswpy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2resgfeea.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2vsdgilfo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rbsrldvu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2kgejaqzp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2slfizhxg.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wqowvfzb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2qsvdrlbe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2pinhyxwh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2woytgchg.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2qqvjrbjn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2omwvjjoh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2cxzfugge.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hvsyjwki.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2skxtlzku.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2prmgfjer.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2mevkqaeg.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jvfbefic.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ezqtsdby.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2clxrzhdl.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2klxnwrhh.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2wvdizdyk.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2utysrvzt.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2lvdyzirh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ttvxgwpy.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2qsykmhaq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2jqrzgwgd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2wjjthwuf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2blmzfuhf.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2njfxkoeb.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2epscialr.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2nczajogq.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2yysnkkdd.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vtqfcdex.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2qvrqcipb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2rsxfopkz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2lbscutga.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2odrqsoyc.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nrwtfona.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2zejowplu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2huksxzbe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2sseseplq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2rlneuomc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hxpvogis.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2nnjwnsuf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2njneegtr.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2sjzxdhzw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2songzhnq.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2vnlntrup.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2eoapfdes.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2rhxhhjpd.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ktbsrjcw.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jsamjszh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2jeiajdgi.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2bytjavja.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2jazxfekl.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2puoqfnko.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2xcpmowfr.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2mowlymrz.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2fpubkccd.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2kckqmsme.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2mftuydmy.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fjblsydz.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tiocbbpi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2oiztnuzg.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2tktegdoj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2banjrqss.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2hnikdalt.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jrxeuhfs.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2orxqivax.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2ozdxkhvo.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2jmdjkkic.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt2xmchefmd.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2iypicuov.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qsjgecxv.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2nsioquei.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wpuyfddo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hadgxgeq.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2jichtsbl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2tmioixjf.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xzeuqnbl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2sqqxqkpj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2cqvhfjov.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2dqwrworj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2khsjbdtr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jghnljjx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2dllsokfq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2nvwfgjce.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wocwjaml.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2amwkfvub.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dettohha.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tznxakcd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jnlfkctl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2gzlxvlai.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2mwazxobr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2hajxrtfw.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2jycmoqrw.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2cxmgmdld.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nzfkdrur.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2gvrdwody.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hgztjanp.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2auskwthd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ddyeaeqd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2mrwsmmdy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2aicukhgi.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2iazochnj.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2rpnvdnqp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2knjmlwfg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2geoejsnj.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2crkfoxfp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2vsulfbul.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kibqavzo.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2banxhvsv.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2aptjwkud.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2qzgpgpxe.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2qxivkawy.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lvdiubrg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cnkgryiq.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fanovzqj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2otxsrxnp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2seulqhuq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2zaibuncz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yssprlyn.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2yljtopqm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2dovxqbtc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2efjzxkhx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2sskzpale.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pgwfwdky.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qhkadway.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kfalndff.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wsxrxcmp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2emjofvcj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2qgzlhxsq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2vdnyzasr.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2mimpcwiy.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2npuritji.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2jdgkjmtf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vhrkcpak.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2vvhruvvl.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2aklapqlf.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tsppmrgj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2gxylhdjo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tlacxwll.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2slyngssf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2mnmdtwcb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ziadggbp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2kwkhtpiw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2dghsgxwj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2cjbxvnea.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2nkyhrcku.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uyguazif.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cpmlremx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2gqoxnaim.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2rnjkcqut.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2qlukjyhi.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2fngzkjis.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dpugfhwo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ffcfkxzv.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2plsixpmj.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2llvygilm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2bcfydhul.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2zcdnvkzh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2vboydgaw.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2jjixnbhf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ledhsqwq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ebrpbmtw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2shmiztln.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ywivnnjf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2kmqamsdq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2khpknwtx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2dekwqpig.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ofrbgecv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jzltopiz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2sohdtdmk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ntwkxyiv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2qdepacws.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ssiwynic.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2sfeajblv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2khvcvfou.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qtzbemqi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2pvlqogvg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jfdmdhpt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fbvotidt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ycbyeuwx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2dsfphula.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2oujxwunl.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2huztuybi.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2dusbfjjj.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2tgfimzrz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zvtsbwnv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bugnwxtl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jakjkfzu.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pewdkzlj.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2iujsaxsl.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2mapysiih.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2kumbyrzh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2gyodxdea.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2murazing.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2joktfgoi.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2dqweplwr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2btsfjrko.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2cvgezbbw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2vohimnva.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2pebknrsn.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2kvrdfalj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vfmcvtuq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2uhuvsccx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ojqwaoam.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2vkmpinel.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2uegdikwq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2enhxxeej.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2eazgxbfd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2zdijtkqv.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2qexwbkdl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ioojdzcs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2jzyakebx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tgxyyris.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2lygrwvzr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2nitujkya.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2acnotfym.html


<!-- 参考信息 -->