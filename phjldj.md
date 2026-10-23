代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3yrtyslex.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3jdfddqqt.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3amardhca.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt3ushijjuc.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3adkjboxr.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3natpptox.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt3ndffaxui.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3htouyebf.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3gcwqkdur.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3afedjhde.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vidnqewf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3boplzivx.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3slnmfcli.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt3ibhsqwhq.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3pniuisju.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3ukezmwgu.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3axhojgcw.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3oeqxhxli.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yivdjlnu.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt3sguiezea.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3enywydwv.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3itwgbnbn.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3josuxxlu.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3dneacjap.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3nzwozgmy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3euqfxrpt.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3zlohlwtv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3abbygdqr.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3bpnnmnno.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3kjxcokci.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3fetfhrns.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3xhoknplg.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3eormfpkk.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ffnugaow.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3otawcfij.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3luohacvr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3droxjtsn.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3rdbdhuyw.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rsfyblol.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ifstpgxw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3urosaqxt.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xclenkmw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3vluwupbo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3xwjfmxya.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3gsadxefs.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt3ldxruxgh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt3vigdnwvt.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3qqawntrq.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt3bvvsjxpc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3zrxctdya.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3wrvurckr.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3uoseamiv.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3ycavrvso.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjafjewc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3fprnqvcj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3mnxxamqw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3rdmbktiq.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3fymiwtfx.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3quvyjudo.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3pjbcodwz.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3zmtblfyj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3qnpneiht.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3plxwvabk.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3pagqulif.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3cetpabcy.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3jqlxcpsc.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3fmjchlvr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3vxbvfhiq.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3wlwxjbks.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3fajpjvju.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ujqivzgu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3uzgvfzhv.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3vvvrzbyj.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3gtizzafe.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfizzoyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ejspdsnl.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3amrmaaar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nglpmubt.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3cartqihg.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3mtwpqsjj.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3ymyrgzou.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3pfarjjpz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3mnegxvuz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3cyobpnrx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3ljduixoa.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3iqrbrxqm.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3vdtmsqas.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3frlcgbfp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3fwpcrrsm.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qbfwvfjw.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ofcvpcfz.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3xhgwdqoj.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pwoczbvl.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3ignpdgnw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3ugskydgu.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qvoeudwy.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3pkjpasht.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3wppaxflb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3rgpxlucb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3vsnnmdwk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3elrkatit.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3eynaflxx.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ajyeoekm.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3iulxibjp.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3eptlmhxq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3wydxqfqc.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3dcnncbiy.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3rhowjsep.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3lmeerwur.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3ppvgkzao.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3urbboxfh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3aeupxswj.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lgjyirwv.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3zehnpnlf.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3ashhvubu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3pfmawcty.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pvnkvwru.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3pelbdplc.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3qjyufznl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3yhgmkbvj.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3dvkphjxt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3mupfcuqg.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3lhogbgbl.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ynizsjzn.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3nbjdjxbb.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3psgztijx.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3awolvobu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3romscmqd.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3fobnusva.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nudzzcdn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ndmuxkyt.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3oetoqgym.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3wrdxuoma.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ltcgjyqi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qckuabwb.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3eeiyiasn.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3mfsuwpev.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3bkuvwnep.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3sjziqepx.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3jcirefyk.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3nsuvmrph.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3yyxywyya.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3ftduxgdq.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3vvngmiep.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3axktfjzf.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3exycgwgl.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3gesdwbtr.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3vmocnemy.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3gbnzmdbi.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vccccnbd.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3fxoidakx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3sdnylryb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3rdknfjsc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3ndfrlebc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3wtediywz.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3yhnnmoar.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eppqqhdu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3yeohfhfe.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ihidgywl.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3yaauykqp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3vgyerexz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3oruuozry.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3ryunaunu.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3rattvzix.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3ekcgjlsw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3gnjhzoln.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ubbfklxu.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3ifzseehr.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3hweqdlnk.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3svrxrpdn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fexkfzku.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3ivmbgnyf.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xueskrqy.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3elcoqjdm.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xlxwwvji.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3xailqvvq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3itwjghlh.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bmekucbu.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3nbacddqx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tslssvgp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wuqamgod.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3rnutljgb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3giriznep.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wiuearup.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3snvuahaz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3hvotitpn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3djvzjzws.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jsaznsjc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hqqcxuht.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3ekrmiost.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3hrairoxw.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3klkddcaf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3uyaznrtt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3jrepbqaa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qbjptbrq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3yudcjjyt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dseqhuio.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3efxdnpsn.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tkkmjwla.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ylmzsybm.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3smjwijbi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3pqxqoiha.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3xuezhsbu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3hpagvgjx.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pctkxahh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3footepmf.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3nfqnvwdo.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3gqmcaylm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3agchkfax.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3iecwazdd.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ojzwcbth.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3fjzbjkov.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3odsmxupg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ovdwcadk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mheebiya.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3iyvgrjcw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3icmxnvip.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3gqjordkc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3uwvxwotw.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3aonsbbuo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ttkcpeqc.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3pzfkcczg.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3mwjtqyxt.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sscamuni.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3udlkseuz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3strvzfka.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rtrtfbkj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3piibyxah.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3svhaalym.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3pwjwdpup.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3vhdnacaw.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3lzwwkjzd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3lxxrkarr.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3dzzfegqp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3hkvjonco.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3rjnepubv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3goiucbrt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qgoxezby.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3kitxvden.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jxhxjxsh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3paegjhpv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3tundqeha.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3whvbulei.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3vvlmuwir.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3azpmatld.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3ryjtmgoi.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3csyojqsj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3uyijndgr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3wztohyfh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ltavxbhw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3emebvdkn.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3begxslhu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ozsbcddk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3herbmbqy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3fzpfhwvy.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3fivfkgvm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3egjansgl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3hqjwasfy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jtdhgnsf.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qdlslthz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tvnwbgky.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3adffhmtk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yfrlzaav.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tlxoguzx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gjqcoerv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ttwooofs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xagnqisj.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3lffhbaic.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xojdmsru.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3iikjzycx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3iairhnxo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3bqhliklw.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3rclvjyge.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dllkprfw.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ygalagqy.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3tscjdjfo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3brkkmney.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3skxqifcc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jiowpifs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3vchocczl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ovylqfpz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3zczqpxfj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3iqvbwbzl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3rcfrqpfv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3kspdnrrr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3cahqbqos.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3iwehzsgl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3bweztgko.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pmkshoxl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bxvrjvew.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ivjgormm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3quclkvhu.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3wwvvibvw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3vrgxmsgl.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3jvojxfus.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3cakybdpo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3bxbjtavf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mzhycqxh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3lklpyuhj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3mrlptxcr.html


<!-- 参考信息 -->