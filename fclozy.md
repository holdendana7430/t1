代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooibifst.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3qhwipacy.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3hivyghlh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3wzlyatpw.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3uqjzvbau.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3eukspfnc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3ocmmifij.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3enuomvdu.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3wtktjwrm.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqamdctt.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3figtdfze.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3ceanhlsw.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3dpxzerky.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3dxxhmhyx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3spwskhyt.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3zemfztgf.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3zjxwaged.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3ymmexnbv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3aweftlxy.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3txtgfafk.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3bwnjhpes.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3bxpnzcau.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3kyovihft.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3xcwzbxic.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ghfhfkxm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3oxolvpyf.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3wxaglbve.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt3dawbbmrn.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3tpwsmtjh.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hsntgunh.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3misffmpl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3rheasjmj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ibyppjun.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3qzfibyje.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3nlhdblsx.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3cucyevaq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3mtqjhycp.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3zhanzbhv.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fozkhkhl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3qddamwgx.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3lejqptug.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3qzflfeav.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3zyxgosoe.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3ldjkhggz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3dxnjwtns.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3znkfcimz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt3qvwgaejg.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3dpjazqmu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3cpfheqkb.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3lnpuoprp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3wovcyrgg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3chgsavhw.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3hakzpnuc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3ewmkkniw.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3rtnqgqsn.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3dmapqlpl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3fzyphslv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3wntqkiop.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3srrfcbpj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fzrcbhyq.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3thtescqc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3pscrmjxg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3voemsnri.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3xfbljrrm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sdpsbriw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3uhkshizj.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3gynhxwdc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3rfbsjgiu.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3itflpupa.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ggzzunyb.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3tgdnnyij.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3csdykeox.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3pybscign.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3pyamopwy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3vrcpszav.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfzfrcij.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt3bvqtyjtg.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3qorueyky.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3bmdhjzdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kinrwdmg.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3zvmxitma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3alqncobz.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3wzjsilwk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3ldbgwram.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pnpsqzns.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3cfprzctd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3ztftlntx.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3sjezygir.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3lpqswmxx.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3rnfodlrp.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3maisccpm.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3enkwfzcd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3kgudwzcw.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3jsaiiddg.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pnfwjsjp.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3chgwluqo.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bndzqxnx.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qlqhpmuw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3sqvnlxog.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rqzzuigp.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3fsqflzwr.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3leerfivd.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3gpbacchs.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3zghlblul.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3cpocpxni.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3hdwrdhlh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3mokrbzyz.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3nmotomsg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bdkujmul.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3vqqmuwvx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nfagzaqq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sarsmakz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3mnfupive.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3dwkymoux.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xtycfvfv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3oajfvbxs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3ptjqqwsv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3nprjnxzv.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3godszeok.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lunumcbw.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3xsbfgrbl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nyyuxcuh.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3jopcnqlg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3phqwwkkx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3ufvejouv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qqxhwakm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3aiezpjda.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3olttnzfe.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vwbklntq.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3veknabyp.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ysiroqvw.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ixajzubd.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3xwcellox.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxoremje.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3xykcdmrj.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3vgpunjmn.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3izayrccr.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3vqurrslr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zzihmxmi.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3solljwfy.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bpattrng.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3xgvghmdh.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3sswmuhnb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3satitqcb.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3imaipuya.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3wslnhhcq.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3kuanfblp.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3vbidiers.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3cmcbltzi.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3kzoqdfvw.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nlisxeoe.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3whacpnik.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3skztqxqc.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3anwkhgmg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3gslhkexa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3biomkeya.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hdxjfwcp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3cjtsfzdf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3xfyzlgtd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3vtniaydz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gcsdnbfo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3bmwuyghe.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3asdbsubj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3mhoymypp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zxwdesgi.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3wbzwwdrt.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jzxuuzti.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3vyvpanrl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3yvxjbnph.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3xxachhwo.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tebkwoqp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3cpdluswf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3ofdqypuh.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3inovvuco.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3icgnehgp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3svsrkprr.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3hucamjns.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3hlfalntn.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tikabghu.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3daalydcy.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3zoldldyu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3yldumefl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3bribriph.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3zfjevead.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3cmrjsvqg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zdxfjpkg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3zxqftcqp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ybleddzp.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3swkbzcqt.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3bvkvfbhs.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3njeqslil.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sjunrmds.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ichmebac.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3txnhdzjy.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pjeufote.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3jcshwefu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3aqqprboa.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3exfxtvjn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3czdgqlzn.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3qosfsnjg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3doyxmvak.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3ydvrmrid.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vucrewpq.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ihtmmvot.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3whtygxrb.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3btnlttes.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3fzjzulad.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gtovvdku.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3fqrbycjw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wuxuvclj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cceaplcr.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ydwnxqcc.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ksxvcygb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3fbpeptib.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3epvmkxja.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3sehvxjlv.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3bqxmchql.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3jejlcwwl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jgitlgqx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ryaaamrj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3unzmgbnu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qfqfqodr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3zzpkfajt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3advckwkq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3fcvfsgoq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3rlgqsdvr.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3assrzfxz.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hiqmmsac.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qvvzjysq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mztmaegn.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pyxuqteh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3srhrfaqk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3akwlcwqv.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3bvnqobrd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3lhuvlmet.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3ynezsads.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3nabstdlb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3lozomkrx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3dhputgay.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3mpttiomi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qqtgvddb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ypkyrxhr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3nwoyfwox.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ngiyauds.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xtkfacjr.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ffvbudrm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3xtvousjb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3orwkbxod.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3lkqzlfxa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3nwahpxcu.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3cdjnvtza.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3srqfdfev.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3mtdyvrkb.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dtpsmxqk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fiafiulh.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fdzsewng.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3bhobofbf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gejnsbou.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3cnnvuhok.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3khtkvifh.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3zpfmpgln.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3mhsfvgsh.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3lkkuawyn.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3qnqnrbhf.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3zycpodie.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3flwcvvnd.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fhokwgej.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sydelojd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nycoidqf.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fwumgwac.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3grhzchyy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ruviuosu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3csdwbnpp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3qupdmajt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3snlugpcz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ahlslkns.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nucjdopa.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3qbnmmwou.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3nhxjawsm.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ggmznsme.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3yihkovil.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fvhepdom.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zcmwxhkx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3louzrxig.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3uzhyucni.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3toujpsgs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3umkbpqph.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3jdbhglkw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jhscvfup.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3eggbacln.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vvfitwag.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3plaitntz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zeqnsknq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xzfbsofy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3gxdnqvmf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3yxjktxir.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ingkmfsv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3cozjgysl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3xpeaxgxp.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3wbdmyrhp.html


<!-- 参考信息 -->