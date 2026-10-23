代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.52xcode.cn/Article/details/gt3wedhqffc.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt3dkajwyeh.html

[C08] 闭包
来源：http://www.52xcode.cn/Article/details/gt3wlhapkqo.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt3agugxgqr.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.52xcode.cn/Article/details/gt3zuaaaqht.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjrfxadn.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt3oolwabkb.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt3rddbgprc.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt3ogaycohm.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt3wkzblynn.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt3zumgvfcb.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt3vhievdxs.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3dbhldjkq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.52xcode.cn/Article/details/gt3kqklrrlv.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3dtwaucck.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt3qqvnkdns.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3iffereey.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3fbyxcucc.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3yzihszqf.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt3jrpabnxg.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt3xprgnrke.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3aklcheei.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt3daadlbfa.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3yfewirko.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3mgtjesph.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3slkehzqs.html

Go:   花括号块级作用域
来源：http://www.52xcode.cn/Article/details/gt3vljewmbs.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3emgehlto.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3nfzcjirb.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt3amvkmwpw.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt3ellifwjz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3ypfvkgxq.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3vpksbkbe.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3hlphvdqq.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3ynkljzkv.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3ipgtwhxb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt3spigvfqy.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt3vchzmhvl.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3fmrgshtp.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3exnvsyqe.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt3iedctfuk.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3bkaeizxk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3afmzkmgw.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3cjnmxykl.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3cqbcuweq.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3kkhpayej.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3lknhucpv.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3qjsowdky.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt3wsvglurx.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqtyocse.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3oixkjooc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3otvosebb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3aiwouxmi.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3cswuphqq.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3huicagvk.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3dmkjpefd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3stcvhyuo.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3ovidfjud.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3tsbgxdeo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3lacwdrlj.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3oyvzjigt.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3beilvfcp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3qthtrajb.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3zjuokdgk.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3nferswtv.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3xhvsuuho.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3koqguwdw.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ptceefrv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwkunptn.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrrclhtg.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3sprjqqeh.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hfvilnch.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3mygsidbv.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3ampofylt.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3jmfepfyd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hrugmgcl.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3hnncclab.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3qpjwmmlo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3ovcajxjo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3nxydzoql.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3dbflhgxf.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt3ttfjjrvt.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3vmxglmkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbqmnylq.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3niwyksyb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjkbylgs.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yalygkdn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3sswiloqn.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3nrkfmoqh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3oodgjkoc.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3kfmamptf.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3ijizdplo.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3rsnluvtv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt3hcfdzwiu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt3jsandbkc.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3xjpdecst.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt3bzluaxwe.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3cjewlzkx.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3yysxijyb.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rbwvahdr.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3bihsnbqm.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fyvwyqjy.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3nkwudvvy.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3cnzmlzfc.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt3ajiusnek.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rlmwognb.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3bfrdmukz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3igvqwddg.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3tnhdlwrl.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vxdoelap.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wptlreer.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt3zpvygayy.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3giovkspp.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3xkqiisux.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3zlfyuiar.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3qmsolzrt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3soovzhvb.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt3lnucxjwq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt3wezcwwjq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt3aktyuusq.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3tcaxglbi.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3nnuqkcrx.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3henfyevs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3viakszwr.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xbvanlhb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3rtcgbjit.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3xkeqibeq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3phyuwgxh.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3qldmpwdq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3sctwwcqq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nejdvcea.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3xtzmujre.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dnicurff.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3ogwhejxj.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3zijhluun.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3razscfdk.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3sdlbcxzd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rrinkwuw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3juirrhbn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3dtghuhdw.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3rxwryseo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3wwumpahi.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bwwrwgct.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3kurlitrl.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3nscnbcvz.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3tsxbpzyf.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3vyrlofap.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3ydtwqkys.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3nlbudrym.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3vzlnpyuj.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3gdbkuong.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3lqugvtdi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3jizrtyhl.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3iezlmqeg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3ezgfqbhf.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3zgiynckl.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3tahoxxwx.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gzjmqbye.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3sisxbqmv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3jbrgsnos.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kyyajnxj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3haboffli.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3tvzjztig.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3vrdmpjgu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3pqmnooza.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3uolzrdwv.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3rjkckaei.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3cuktvnki.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3empeiedk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3brsyapyu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3jzrssjtg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3jumlngag.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3hdxevxcj.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3aatsnkvh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3tuwptuff.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3cjehtlhe.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt3dueygudt.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3vknipqyh.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xdadpkek.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3gzhhetgn.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3wirjgsmr.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3fdmqflfq.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3adzvtouz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3pfjyejhp.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3zfkaguhg.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3klvqexru.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3ubaoctad.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3sotqbpua.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aafdrtfo.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3fcplufph.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3mdsfzxge.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bmqjijuy.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cplncamk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3lntillju.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3txhaaosb.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3exwbmdxk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tybhzybh.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vcoxdytf.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gtmhnfvs.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hdmxqvib.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3fpbtnepz.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3atuwctkk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bxuwzzos.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3wuaalwks.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3jfuqlygd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3dmsvtjmp.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xaaupnmd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3qyykdbpc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3bmuolrvw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3kqcmijcq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pdfkbvhc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3lzrhvbyv.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3xaqpgxve.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3jggeoxkx.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cfigirzj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dvqldygm.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3tqmtxwgs.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3ztefgudn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3lqwiigio.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3fuvcwnvu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kzgluxwe.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3tgkdcfxi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3dcktgcwe.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cyuatoqa.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mheltmkz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tkauqwwd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3wtcomxmv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3omdkidql.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3khqfrfhu.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3hllglspe.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3oynpysxe.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3xwsezqbg.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iwetvdxu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rjnrlxfy.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ttiqopur.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3wfoeqkhp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tsyrdpth.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3kjsipedk.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3xfdtrhrm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3mrjeujuq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3xbxduatj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ixophuja.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3wmlmigpv.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3nqcixwxr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hporhrsf.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bneuhxep.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3bviibaiv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rlulbjns.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3wcpxdjoq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ldzudwmp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3abjwnjjh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3wzgzqkew.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3wgfeoknt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3fcluiuer.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3bsfcrgbl.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3asgjkkba.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3axkqzzzk.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3mvpiobmu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kajspwhc.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3gnyinvza.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vblpveqv.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3sjntcamf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3dhjblwpt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3cpusfpfw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3bsyiutai.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3opcopudv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3llqfhrhw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tuizwces.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ivvrhjgf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3iuchcupc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3idopykka.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eogjuyqd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tbhztehq.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gvcqztht.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjcdiwzu.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qcphjhtb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rnbggphc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3rifbinpb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3wyofjbpe.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3cqftbdih.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3iwjazrtb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ehhqsvzj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ijbjttal.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3masoymly.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3zpkxkqqh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3ddvdplww.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pogkfyou.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rtmyosey.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wjmqfzca.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xmrpkvbv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3nfwnqdmb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3ljnfnvji.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3babyiovc.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3pakcgntb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3fvdesqxj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3shanptlr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3uyjretse.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cwukgxsn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3tbdzdfxs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3aifqqbvf.html


<!-- 参考信息 -->