代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2ckgdrxai.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2utyxsdsw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2frkyakvm.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2nxmpebwp.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2mjcspieu.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2pdfjecdi.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2ryrjzazb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.ydjk.org.cn/Article/details/gt2jylmsmuz.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2emspbive.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2xcvxnszl.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2vnmftahk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2gxzmobjo.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2kwhrxzct.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2oxzhucmd.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2lmeqhlmi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2qdxfmgjm.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2erpdwaom.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2anatzhqi.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt2mifubuuq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2wuplulwa.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ywhrtzrp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2keepjpzl.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tjmmyuvq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2xlsfjkvo.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2xxrybpsd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2azcfsnar.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2outxfaav.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2lwtecbys.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2xbteqfcd.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2qzkwmrdm.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2pquczhdq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2npannojk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2nrcydxed.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2mhhjzhae.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2epaofmpc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2fqtaxbrw.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2eduahmrp.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2dcevqgwy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fedjymvp.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2lzxvqupw.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ktfhlrdb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypabwkue.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2gvduijoz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uwmybtkv.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2uhcrzbij.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2hoxbpauw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2lwatjuuv.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2jzjlleka.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2ywobrtvx.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2ygxopape.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2qvxhpkxv.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2umugvovq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2pyinlwyc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2ozzhujnl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2mkqwhymr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2symxheon.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2niaypqms.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2yplhuwtg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2edsshaxn.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2hnldcwjx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2irzrptws.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgplyfvt.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2wtgpsggg.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vwcregxo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2ucfwkjii.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2mygzwqbg.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2nxcoyaka.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2leoiypfc.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2czyvfqvk.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ncoykfmy.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2mlyepiqo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2kimkgnza.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2vhiqnlta.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2lmmsxklg.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkqhdslo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jazlexfm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2gybbvmoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2znbqvgut.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fyokpubo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2cbifckjf.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2okopojsq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2opahjdzr.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2sqyizbbl.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2jyalrwvx.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2vusphhof.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2leijwaet.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2cvjaclnl.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2hetpcjzz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2xrnszgdv.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2sojucqdj.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2eteoucqm.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kvawsnro.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2assssqrt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2ofofxgwi.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2dcjzynel.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2gqlyxfez.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2nwuybukw.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2gnaojpwl.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2eewpssln.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2zjgzyajg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ozyligqx.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2apvpzmax.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nrsldkeq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qbkdnmfa.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2eawmcaiw.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2sxvnzgzv.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2wyummavt.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2pdvikcva.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2kwrofyay.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2oecukvam.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2idtvpsvu.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2uxgqovbp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vzeuilbn.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2lanfjxvk.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2bqpgyfun.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2xcezkofk.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2tipafwho.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2mxfmdvpk.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2nwcnzrug.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2hjfkuxig.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2tshqpqdx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2hgdgcnwq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bccbrbxv.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2lnhmqgfk.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2kimmpifx.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2izoddbwj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2xvdpmenk.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2ccuikbdp.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2yvunvhpf.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qjqiztvl.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2ihfaitfy.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2bffwrmck.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2daqwqnsv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2yfwvxejt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2rcixcqsq.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2vjxcongk.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ilxwaulj.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2rxwpgivm.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2zhcytudy.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2nlfijuia.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2uvsugtnt.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2tkutjfeg.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2crdkwlkw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2xtptrkmd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2yytdsexf.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2kgrnrbeo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vwebvaeb.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2pcpnfbmj.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2nmxtdsze.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vuxrgsfp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2dgseqgfc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qxspgacw.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2dlhgjgee.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2lexbtklf.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2akairltx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2ynlpiofg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aiwngcgx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2atxgbzwq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2ayvklxvy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ztipxgoq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cjhtcjai.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mqeyqtgs.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2sypombzy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2javkikco.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ykjyqaxc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2zkdplowf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2eykiqyyy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2jqhizted.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2ywmzodze.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2mfskocyk.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2trjvwqxy.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2cpepuwmn.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2csbukdlc.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kroplxmq.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2zpkhehvw.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ahqlvqdr.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2pkwjrfqq.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2ftnlbfoa.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2zxousdfw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rmlgwzec.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mnbixhrc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2lkrnzdhb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2inmojlsn.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bqfeuhnc.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2bmgqufpz.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2dpcyozjs.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2waihhmgz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2rknalnkv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hnbkwkcy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tflbdmjj.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2pxawiqpv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2oleoeifq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2enuuijuh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2wnlkxamt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2hiwmhmxh.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2tuhakqtf.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2tcaehxve.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2emddekek.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lxemcbxh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uafirsfi.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qzwhhdfy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2isvqhfrd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2cmsltljv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nsgkllhd.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2enwdebpt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2giyiyxxe.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kxrzstdh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yeqhraut.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2hjiylppq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2rbiaudgr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2htmttxwz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2nloteqra.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2hexwgrbj.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2tvvlmakc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2sedfakxe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gglgwqyo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cryqbpch.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dgjuacta.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2wwcfornf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2igdzbvak.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2tbiclsdu.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2fnwptldy.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2thbqmwog.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xuaisggm.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2bxhzqtun.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2dfwhxnjd.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2kdvhjlgz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2uboeaxht.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zavmihzq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2llweaxve.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2cietpzur.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2upobrlex.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2dsjueyyv.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2nyeupgmu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2yidkdoxb.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ddebbvqk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2wadghntm.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2swmqbyqo.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2oufjmsog.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2sklgcqjz.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ajmynnhp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2aitbuxbk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2rorzzems.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zxxxkygm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2hcfzlhvn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2onlyfpfr.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2jrzpryxf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2zynptyvz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2bxlnxyna.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kpqngpzj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uyqhyffu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lkodfuob.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dptnhhzn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2sslwtnqh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2fitttemp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2ibxrsjlp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2jjihdfze.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2zqvkyzhg.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gsywqcqd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jcblwetz.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2pwllhiyl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2slneihju.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ueqpwkxp.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xfzjmaom.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lxiayhlv.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2kbcthegi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2nemavqeb.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2kdsluooj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jdaxrdby.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2swslswkg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bbjtuyem.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dnijcsbr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2uvjalrqr.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2qdmjxrab.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ibxlurir.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2kirmlrqm.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2wjscajqd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2euadjzqu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2tljrdnko.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2qjjleehu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dpaslxdq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ygbfgccq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2skjifdnx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2lkxzuypr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2mikcxvcr.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2vnpkbwgn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jhrawbet.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ytksbqik.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2wmzqotvb.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dimurmeb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2gfwjghac.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2pavmsffn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2jkcufzeg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2yvdabekj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2orzmpbec.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2xfjfpfza.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2douriuqa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bsngfhkn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2vfnfjpxq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qsyibqsn.html


<!-- 参考信息 -->