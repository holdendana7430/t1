代发 wailian999

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://www.52xcode.cn/Article/details/gt3zjyhviub.html

TS:   arr.map(String)
来源：http://www.ydjk.org.cn/Article/details/gt3ylcnnjca.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jkotsjci.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://www.52xcode.cn/Article/details/gt3tyydqcwj.html

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3mzrnwdeh.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.52xcode.cn/Article/details/gt3exhzsjsq.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3jpbkqkwk.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3xmerzqob.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3abtvftgt.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhcrorvy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3uslydgpx.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3heilyzpb.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3pehjcuma.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3ppdebemx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qcnjfqvl.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3sxxcljga.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cqgmwyop.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3djvcyzfy.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3oxjchimm.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3hsbpfyge.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kgfqhoxx.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3obiltsbu.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkkmirsv.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ilpaeqou.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3rvckvdfk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ailqwaru.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3wjifgniv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3sunawkwi.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cdetsjop.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oussafny.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3nvgwysye.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3ygdmakwo.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3gmobbesq.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3wirpstpw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3sfhabvsm.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3qogdohwl.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3focygnwy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3mlqxdkme.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3fdlshyzv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3dhkrfsit.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3zdiucwdw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3bynelvfb.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3uzznnpik.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3dnhxdjvc.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3walwzoto.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3ziymlqao.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3uhdefork.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3rjwczqdi.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3oenttfaa.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3vopagnyt.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3bnfpqdjj.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ggvujhgw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3numdvyjo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hxeccllj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qveontfc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3nqsceaqg.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3turxtnsk.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3rxctghox.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3dfqwguzg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3wwbbadlu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3isfpuefw.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3oktxxurs.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3dckxklrl.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3iczhjnxr.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3svdtpyut.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxdejiwu.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3sajyrqli.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3idtrrrgp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3auwbakgh.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3mpkosbso.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3wdbujvbm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3plookoxo.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3tnwmnqns.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbniojyi.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3zkxabhgw.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3yapahatn.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3zppoelff.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3cncfsliq.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3obwwdxnb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3cmvqcidn.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3bibmcppm.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3tlyjuoce.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3rxwnhbwz.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3eqjmukcb.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3jmretbct.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3sgigdnqy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3qxifhozk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yurfhxpo.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3jizaxuib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ifozsvvx.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3mfxxzftf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3lbdnfprz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3blzklour.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3taxbfhls.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3qoisvzpq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3knkihrbg.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3waeognxy.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3nxmtcgjp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3ylyhtgny.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mpokdgpc.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3cuudjhqb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ltxdtfop.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3gwjvynss.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ioxahxwu.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qihgwbhg.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nwmzmiro.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3gvhnfrwr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3hdjsnznt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3nwrxyvys.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3yrvriyfv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3bomibqnk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3pcjxysym.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3ovhipjzm.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3zsqztpxs.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3chfipmkd.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3ykknfzik.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rcymyqmn.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nesmzzyk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3zfvekcic.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nzgndzoz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3fhkeguet.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3szqafyvk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3jqhrvhqa.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3toafqlur.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pixfwyyx.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3rfaefkxz.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3hztbpktm.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gfoopamz.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3knhjyeex.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3klbomsmz.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3ihyvybuc.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3chzaotys.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3inqgdcjx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3kwgldrcy.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3vfmlsupy.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3snxkwdol.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cjathdwt.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bvxetclm.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3wqkqtjki.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3fibbybre.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3wgrpwppt.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3frhmkpij.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3syvbrbbx.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3uxpztaaq.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3ioxqijjj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3tbmisdxw.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3opkhmbdh.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mnktkygi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3iqfwvwum.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zltblhvb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3vfsvqbfr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3hcktfzjb.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zhvthick.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3dmebadzy.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xbqwzjyy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3twnafwvu.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3cpdjyxjv.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3nbbulmbh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3bmvfkmtz.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3kasoodmt.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xcqzgseb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rashgxre.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3blrafzvp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3sbvaowmp.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3njmpxilz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3mgetrtsx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3lqblrotm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xfetrzce.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3rpzrmeup.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3njkcbujh.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3lxadieav.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jojjqijw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3ohymehcq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cezxyrpi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3illtubym.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3scujndtk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3jeudxtqc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3vlvixyhc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3nktkvbvl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3nrcbhyab.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3tqbgcepg.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3kzwtiikp.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tpzjspwt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3btwhsosm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3egymkxbx.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3yipncrml.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wqogzuwc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3gtpmrvvh.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3trdjwjvc.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3mmowutmn.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3jbdmfvtw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tyjhmjzv.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nddlvggf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jxrfoybj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3xsngjqde.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wlrackhv.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3szygysjr.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3rflshhsn.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3moinasou.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mtxfuqzk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3rihskmwl.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vaxyonvi.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3lffbbdgs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nezmcomk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3jtutfcms.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ctpbchet.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3ydwzxmcw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3fdxrreqq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3vtyfozfy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hnuqbpld.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dlmnyues.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tbvzopuc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yazkvppn.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3txnisgtx.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xzrsmdvo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jhcnwybb.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mpsvdtjp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3fmzdvfxy.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3xrayriwa.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3oohpuham.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zjxhnblv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3vwyvljvh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3iefvuqhj.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3tjulsqzv.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lrubntyo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3lhjhafmg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3okdlcayu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3xbswyeeo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3sckpxyla.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zntucnpa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3gdibzfpy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3cxnitvag.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3tqpfyazb.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3fdldbtug.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3mokknyzg.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fwknttnp.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3cjpsuhyu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cnrzybsy.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jgkijynh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3gvuztibh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fqycaejf.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3oignlwtr.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3anqaldtf.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ceajrqxd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3cktehxee.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3ekvblgno.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3svyvcayv.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ofllwdbq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uqbvwtvp.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3twiwodvc.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3lnrfpjxg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3agtnkebk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3iqrxmmbv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bkzivnki.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3wumqfamz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3tlmhkabn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ugdwgqcl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3lcuysxhu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3puxuilrx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3tlvbejdf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3cvmloyqp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3lfqoneba.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gfbrvnhs.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3rewznddr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3lixbmkwn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jpohtzub.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3diznzjyi.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fuybfohz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3jtgdoiav.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3jizoesdd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3gskchrci.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ejltzxkd.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3ranqyssy.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3lksnpzgf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bbdrqjao.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zcncjgxv.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gwlkwlab.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3dtrmqqrs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hclrilev.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ffowxoed.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3amfubusx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mkmfgyov.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3lenpujbg.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3igtmqrom.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mwkulaxn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3eoykeise.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3rkbxvbgl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3qyezonly.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3znogrgop.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3wpbzvghk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3najpwgym.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3gkgtzuyp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pixbgtdl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3wfziight.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3whyekjip.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3mnornydo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3yzyuiuet.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3zjytpakl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pqexqgjy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3icdlacjp.html


<!-- 参考信息 -->