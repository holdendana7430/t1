代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt3vuxxtxre.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3vfyijedd.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt3zxvjxfle.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.ydjk.org.cn/Article/details/gt3tsqszpfx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ywpbycfn.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3rzdrquvd.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewjyemzb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.ydjk.org.cn/Article/details/gt3vupweghk.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3ngeoeymy.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3plomcjqx.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3xnfrozrl.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ohnvqrpe.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3mbunzkmz.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3hpleputq.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3qvknnybc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3tzvnxugj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kjbuhwst.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3sinordcy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3qkmidotb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3demaigdn.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3evynzpem.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3gssqpmku.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3fqiwfqgv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3lidrdujq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3rgdzmpez.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ikghpkhq.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3ashssute.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3zjmcovmk.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt3isxsvyql.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3ydizggmj.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3robahxte.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3fcqvkzfs.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3wvnsnfsh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3yfjuynek.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3fujanngg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3ngdztamg.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3zozhrtui.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3enydamxt.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3zpnexsym.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3nccfztwh.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3xprldfce.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3qnxtmsyt.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fqztrlnt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3dabnbbny.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3yenlpomy.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3xbtmathv.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3jatpyzbk.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3exjeyogl.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3eszcnefp.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3kfpvoohb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3ubekzwpz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3aomubyur.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyovqjcs.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3uwhkvyju.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3jbyriloq.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3wkdegdwu.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3vgejclsg.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3cvpuysnf.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3bchaeigg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3oekrioqu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ffinvslh.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3iifhrzwb.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3eyxmmrjm.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3icacmxly.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3csitqgkw.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3zvxiikgi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3evglmhxt.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3cpebyhqj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3pjvrpjks.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3wlitffhu.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3gmgjjdkd.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3atcbtnni.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3skimtymc.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3gcycvazm.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3qdovrijk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3tkwpsrwd.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3nzamzayu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3sxqotwdv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3gmvhqrpd.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3pmmzyqkn.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3oyoketmz.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3dgnjlpdj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xgkeczhf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ydlhmwes.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3brxsjynf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ohutktrn.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3lxrojktl.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3dqbtbfxg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ulurgddm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nwkgkgig.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3eastfzrw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3xoqbtmwy.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3uxxpjqfq.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3piedbosf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3pohwvuwi.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3mpaeepol.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3vpwyjikr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3tvjceygm.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xmjtahbl.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3irqmveoi.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3xvsquopj.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mvwxcfld.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3vbcvnkzt.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3djpsneue.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3jmswqcns.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3vxgaasaq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3qmetjesc.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3iibtmsag.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zrycqjle.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fmmegotg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3nxsghcof.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3cenbcmso.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tkzpebbw.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3lrbcqwme.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3errmlrpn.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ahcgkbzb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3uwhahztv.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3zppnvdnt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cbdhpefe.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3fztqrtqk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zjyknhut.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3znooeecn.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3zygzzixk.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ghpvzkry.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3hpmbrklf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ekokgjdt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3pbvgwjgf.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3voaimvkv.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3ktdtcjbl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3dsqwmawp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3dctvawpr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3tthtfvvk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3btabeprw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cridbpuu.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xdvmxgpi.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3kemlyfzq.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3wtcfdbbl.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fsydoscw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jnqkcvgg.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3hkdvwzkp.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3dqcslojw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3xustjabr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tnazyitm.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3xupyurlp.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3rfamkcqc.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3lhkicqsq.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3nykuwwmf.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3qnhtgesr.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3wfhwgquc.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3xupahglv.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yxajjgvt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3qbatrvim.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3pttacmpl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3leknelbb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nchncqde.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3qnicezay.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3oqslpiul.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tpsmkdvn.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3rudnllae.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wqzqdpjs.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ccqmvlhy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3rugdfoeo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3ufemkuup.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3okjyevpv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gtpqhjmt.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3gmucxlfb.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ihvqgvad.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jncpjdfq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lnmaddud.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3eedfausc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lqiskhru.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3alxsabjs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3dmvrwjro.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3oaesxgko.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3rpsstvys.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ewdvttmt.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3rzxqgeft.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3tdutbzqd.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3ajevlodv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3wykakqiu.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3swmrtvwe.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fnvmxkpb.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vorfutiu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gzpchjih.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3gkmourve.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3cxlgpgah.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3zlymramq.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rifzghqu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zgeukdyv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3wlenvkgw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3drjdqizl.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wkssdpnq.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3eygojmxe.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3abtikzhv.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3zdufkwja.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3capdduvo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3katqhkge.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jdhcteax.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3dkittvlw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3uvgudnfn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ajwhcpee.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3nxybwwza.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3sxqohtew.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3fgfbbwuz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3doiziipn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jmakchqy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3wgvyxaux.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kiqzgkbz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3gmzsbnvf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3syoditsg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jodpiwck.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3mmgxubba.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3evmlhtwn.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3slxseyte.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dyucofrd.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uddiseug.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3njrweiuy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3tmjfpixi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3vhadydas.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3nynaarfp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xawsihcg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3oepskiql.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gyuutejd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sxapaotm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vawkiwqw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3aktooqyn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3stjkbhxm.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3vvhwxmyt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ehwliuep.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3vpotavde.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3tzscases.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ioumfifd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3xuvehpue.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nlsosznq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3bulptohg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nyivgeot.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wsbqejfu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3fwasgabs.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3lnbxzhia.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3wcmsxsly.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nanyfoif.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3vdgyujtb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3mbghtchw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3yaebxjut.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3phwwjyho.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3khayxyro.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3fiypfwvd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3amiqstxr.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3qvythnah.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lktcgqem.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3fsgetabs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3kzzstlnt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ymyzcwly.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ftjynivz.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3fiulomrm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hqfjsiew.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fnjqzbna.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3eopkefqo.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xjborcro.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uhjgzypy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3rvxjucnl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3tiktnmlk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3xeyjazpe.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3veebweyw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3bjisexmu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3kunmaifa.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3dctsamss.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gmyfwogb.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hveaxwld.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3oralntrl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3axobuyic.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ajqvawnk.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hwpwkjye.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3weulztsz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yynfhpeo.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3vzivpyqi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3cptzcffb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3zkygxiip.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jzalnbkk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3zrzqhxxr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3yuizqvmw.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3sudcxrca.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3brpvvisc.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3hltftump.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3wpeodory.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3rxanfhqj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uyfszwtd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jwavggnj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3zioktduc.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3uxampnfo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3kuibhjxi.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ozqgkupb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3lghtjiyq.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wohblnft.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3xntpujof.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ljhnyqqt.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3zeeggxth.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bvygpvrg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3uqjvzftd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3nrtugvhn.html


<!-- 参考信息 -->