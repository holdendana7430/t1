代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbvbgzyo.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3fkjfauph.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtjyzuot.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3frhzvwyy.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt3wwqcneae.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt3jmsgzqns.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3reuapxzb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3ykhrhofo.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3cikjjijd.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3lcsqhnpk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3cgeofasa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3xgsqaouz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfkvfeia.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt3dhgmvtwe.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3kbunnmaf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ssblgtbw.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3rsegjumy.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ajnikfdg.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3sxpemtui.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3nktnosdl.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3hrvhcfgn.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hdlynswx.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3wljpzrxs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3uhwumztv.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3haymijcb.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3mjrykodn.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3gwrbdsiz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3rvtgixmb.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3rdfpivks.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3mfjzxwpa.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3hsamfydq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3gsfdkdqd.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3wzynpvgf.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3esqzhhnw.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3aertvpcs.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3ibhahuer.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3ymuoujki.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3dnbpzayj.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3kfstjvsy.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3gxivrqck.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt3kdytefuj.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3tgytxbtn.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ntuksgku.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3mtgxwavz.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3frofvxet.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3dcrqgxsb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3jolcmpqa.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3iskvyjue.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3equafyot.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3uobyoikj.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3tbgfhraf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3mkpejzbz.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3deeeypbu.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3fjozppyx.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3orjizkxv.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nwalbhkm.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkhtjpds.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3ogjnigys.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3twlisgsv.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3fqtpvgip.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3lztjunlc.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3liqhnnxo.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3hyefzgxf.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3zesrbegi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ptakjodg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzxhgneb.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3qfuiejvu.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3wnzghrta.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3xcsaykbd.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3aekunuxp.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3kbfjcxdx.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3pdyskisu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3fckqdjof.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3upgjvygl.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3klenexhe.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3wxtnbfpv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3tcjsputy.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ohjbxehl.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3cqobayjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knpefrbl.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3sxqapizo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eytzzwup.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cgeolpvo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3wkttuuvh.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3csaivguv.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rwlszgwi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3tkjihoho.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3uuznvziw.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3adjzodas.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3vghjgkap.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3sbuogupr.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3ldjfgatu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3gtzcbeql.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3kmtvkypy.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3vwrlrmmk.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3odsvrxxe.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ujrdyxcc.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bqsuojnr.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3rwnnjjqu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3fvjvyzze.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3klwxzubh.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cfetqtna.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3rfypcyak.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3raslkofl.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3jvolsegk.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iigqzcrd.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zmdcxpyj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3dtulvaei.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jpfusuxg.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3nppfgzot.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3budtvvis.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hqpmqgfc.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt3egxmdymk.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3pybhzmvz.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3infjeedg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3qipouafv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3gkwtbuuk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3ycmcfpsl.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3xixgzhpt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3hhlnbrip.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3qvlozeyf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3rrbhlzho.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3kdepruyu.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3uqvoaytl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3gfeimpfa.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3zobbxdtw.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3wmioarwq.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3efyipsjo.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nusphegc.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mqbamhky.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3vwvnxtff.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ryvqfphh.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3txxrbnxj.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3liakfglp.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3horzernr.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3uoyerodk.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3umzajdtv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3rausgabr.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3kcaxrqgf.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3kcgzqzmi.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3icdzdlpb.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3zoaielsi.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3dgdbnubz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3vckdvmph.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ptzwrdoe.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3aarmpgjr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3idtcgjcr.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3xqrignzc.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3eslzstpe.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3vvjstigo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3vndwndaq.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3viyuctdf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3abhynqom.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dcgkujfm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3pnihdwff.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lormflpo.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3ezskoczu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3lwhbvhhy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3nxnmwhcm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3znbgoilv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xcjqkagr.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yyvlfvdw.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3tmuxwvrb.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3sjsqkeip.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dbwncdha.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3yvsqhyim.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3mbtsymkx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3drqcbczo.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3omfhnbsc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3qedyyqqc.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3nyubjsfg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3klaustli.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3bfyymetq.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3aczrqksn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uzsarhat.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3usjmusqi.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yfvchmos.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3slavakhw.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3yhakxawu.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pgibitzt.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3eorxyusm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3rfzmpsit.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kemyqcvf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3njrjrqyw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3xcoofttf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3byhpdvas.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3bchygfms.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dthcvwsg.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tipjxwsv.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3ptfhvtuh.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3vbscyjpw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ijescpnh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3orvkmsyp.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3tmwvclqk.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3fuddvmni.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3favhxwbc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3navaodts.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3gomvomzj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3iyospojk.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3mnqsqxex.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3heqgmsbb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hdxcugvw.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3dxkfwpoh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3mxyucirp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3tzwxkjjg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3lycdbfne.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3hrcwsgdq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3frqanvdh.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3zomdninf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3aksbyoth.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3cxjmjmxv.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3bcjixhmf.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3yhgcqcnq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3movgmdok.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3hxanzzuo.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3medcexcc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3inbbvseq.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3aymmzpev.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zwonecui.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tajanlab.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bsefiklf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rcpzjtiz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3aceqgcak.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3gjqueahi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3joqrgfju.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3fwomdpbz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3pomkffgv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jekkuith.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wwbuutie.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ncoxlbnu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3epoubtpa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3kqzavdvo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3agspnwza.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3pkozguup.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3xosgxaiz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3ihqgwiwr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3wdquuwmy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jzszizwk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3viaagdjb.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3parjhryp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3kcydburz.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3hclavbwn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3iuqicknu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3tilcgfdz.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3bbapokab.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3bmdysere.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3otyehgai.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ltxprycv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3jwusauno.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3xqcyasnu.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3ggacxvza.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3dsrmzqxm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ihmkmzcu.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3piebgpqk.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3flsytpag.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3doskuusj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3jvlaoqyn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3wkrhqcsj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3vzkxspup.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3kmwffixt.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3yyjaqovc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3zeazvtki.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3klyqrgbs.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3robmmkmx.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3hsfppkyk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pkluzdib.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qslvenzq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3vyjyrcex.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3byluxabs.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3asodthsw.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3zcfwsxgm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3mnkmwwog.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3rwfzndmu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3agjfhizj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3duorhubg.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3fztzwzel.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jkikmexp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3jyhsyxws.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3itiyzbtj.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ytdbfjwl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3xspdwhda.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cejczldw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dhjsjpvh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ozwznabe.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3wbshpuge.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3cxzpmhlf.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3iaqpwzjp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3cmvlyeyl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3equadttb.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3knynplnn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ekfsgaxz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ayaqzjqu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gzldngwv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sdhvoedh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3snifolpt.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3mlslhdfp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ixrgneuy.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ztiifpsr.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jvncbljo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3uwvwdkzs.html


<!-- 参考信息 -->