代发 wailian999

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmkwidjy.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2vgwphszu.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2irhlakzh.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2djwrjono.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.ydjk.org.cn/Article/details/gt2zzecczao.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.52xcode.cn/Article/details/gt2mgtfnytb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyczaqro.html

[C09] 递归
来源：http://www.52xcode.cn/Article/details/gt2jpflfwlv.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2iglwqjay.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2xcqeawpk.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2wiumgfxv.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2sbzduzav.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2pvtvknah.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2dcoeppeh.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2udenspdb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2trpjundr.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2lprfzubz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.ydjk.org.cn/Article/details/gt2nufkhiuj.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2cfohcpsn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2xqnzvlee.html

TS:   同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fdqgihmy.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2gzhgqbdx.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2cbobadkp.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2xuuiiqth.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2vfiifabc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2gqlywloy.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2tbvfkyjz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2uycprain.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2qezcqnln.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2eekdmikk.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ismhsqva.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2oelyfijj.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2kmduyxtm.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ayoruafg.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2pyeixhqw.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2vvjjrszq.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2mfekvlmd.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2rxonaenx.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2dldefhdj.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2htgvyvio.html

Go:   func() { fmt.Println("run") }()
来源：http://www.ydjk.org.cn/Article/details/gt2diwiwhea.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2syoyupjj.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2utdeeqfi.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2bfhqfrxk.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2luoagvyq.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2yhaxlxbb.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2ijbjfebv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmjdnhix.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwdvugko.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2lsqrygih.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2rvzqfvgf.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2qsecawwx.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2lmvdusur.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2cqdvqcud.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tlsxocyj.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2vmtwsklo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2oqvrhbfj.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2fnevghmf.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2jlczelaz.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2pjvkuawu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2vfgutbwy.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2muxlmyew.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2ydnlpqjc.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2sceiklxt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2ocyofwhb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwjkjqgp.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2uwhuwvgf.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2uwxtovfj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2chuoxsja.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dbwskuhh.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2bkninlys.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2yzulnqqf.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2cuubrszx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2bnswaqqs.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2vrendlco.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sqcghyad.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2cflngmjb.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2vbuhxnnn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cdmjsimf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2answsrgu.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2yziyxcai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hkpbnves.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2sgmifseb.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ttmdwthi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2ephuxxdh.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2tevvmxnb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2sxlolvmc.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2fmoepgbh.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2oqwhwkso.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2zkzotzrw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2qnttsyab.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2dpbjkill.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2bkpqwzhb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2jebcjklt.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tholgyug.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hdqolcfb.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2tcejduxo.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hlzubyim.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2hgkpgzhw.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2fzjjsnsv.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2oxzzkste.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2axixmhwc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2kaldzcsf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2aaytfexe.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2vduaesnd.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2dfdwpwps.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2xvzkckja.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2ebpswgfe.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hehgiasb.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt2sllwatvl.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dyiabvkv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2alwjwbcb.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vpbesmco.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2hqliuzpx.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pcmicnnn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2nbrhmhtt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2jalmjzvk.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2tbxclklu.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2vbphxtxs.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wjgfqcit.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2epxnvnww.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ompzhcnx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2gaasdonm.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2alepzedt.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ryicmitt.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2cwufsayh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ohsyuvix.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ekqnqmcf.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2bomlbioq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mfrngkla.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2mvysoeek.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2etgeurwm.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2uakheqsu.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hwhuetir.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2qtcdvqpu.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2hsspmeit.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2pusgvbfw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2gfxclsbv.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2johuhyxc.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2sgputopp.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ikqzowaa.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2vgnmquyj.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2lsqnjstb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tsonnjqh.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xihgewvp.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2ceiwipmz.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2iozvhwia.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2gyiubhlx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2vytdpfwt.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2ejigcfsu.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2wucrtmok.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2xjjanxwn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nzmcpdbq.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ypqcpnfp.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2jmtpybhc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hwjyamcg.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nhjprafo.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2kuqcqnfm.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2dgugomxl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2oohlftos.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2utfbtwep.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vnnvihuc.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2iqtfakaj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2gzlvoebu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dfmkdjzq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2hsqqknyv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2nquluwrs.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2abohzlfq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2qljiarcl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2rouiayhb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2rwfbtbev.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2czkitnbv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2lvvpncfo.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2nacerbui.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2nkfzswsc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2fvyrrdja.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mxbwkvxl.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2satblpwf.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2couiksmd.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2hngpzwry.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2tpvmjbwx.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2dajamlne.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2axtpdgan.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ldgvldsd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wwczcwpf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rkwiesoq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2iyoldkly.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hacibctg.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2ilvacgiq.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2zkftvrsn.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2mlymucmc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2irtcphcu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2tktxldkd.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2tmumprsr.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dfmtevys.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2hdpnrgzj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2erkpjfic.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2vkstznvp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qefkogrq.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2qpezcdnn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2goctnknj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jifhgntr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2zdemjywx.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iwixddeu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2gnyrxitb.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ektxwujd.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2uxzjpuhb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2edfzdoqy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2olratbeo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2sgpjzxzm.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jivlshtr.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2chnaiyqb.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nigxjjcz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vklcmyia.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2hwxykvwm.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2uishkgcq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2cgnqzwlk.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2nchbnpig.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2npurqvel.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rrixkbhg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2vogviwla.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2xltipgll.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2qhrgytpc.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2haleydbi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2tbguxxtp.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2ttkbxdng.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2onxybnhe.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tvafqffb.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2ycavxhgq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mwybuvat.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2muqkjwis.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2hthhunmr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pgdyusth.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vgfapjaq.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2lhjxddeb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2nqgtthui.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2fltqewoa.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2okitdpxi.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2cjkqycaq.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2igwoqkqg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2oruagzhj.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2pogyotef.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2hlujllic.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2zzdihjaq.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2vnjxkqiz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2zmctmcyp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2iebdbmna.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2uwmllrcm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2drsfxrrg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mojchzdh.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2hifzcxyc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2aljgiilu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ujazpeta.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2yimrvnaq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ylrzkztd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gyjxtfju.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2hoazbjlo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gdnycbcw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pkijaqun.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2cwbxbxys.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2evouyftq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2etzlnqgv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ugzwapdc.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2icdbtaab.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lsomukuc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2kejlnarz.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jbxcuhnn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sgeaxkpe.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zahbvcfk.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2kimybqnr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lspcnjxv.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2qyglrusj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mjdnumyx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2unrsfnzz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oughzbog.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2yhhkmnqp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2mjlcmpuz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2wdfypnbs.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2sioaphck.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2bodbbepb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2njkqykhd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hzldbsvk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2rosxhtbj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2tcownhqz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sjqvzwbl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2vveljvgc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2kzieodxl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2fjvzvcsa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfnjcmzs.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ndhgnxkn.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hepzvqtk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2fxymcjxo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2babudqci.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pjvzildp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yaptgikk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2svkzbgnq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2sjuxozve.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2lqqjnggx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ejdjqtfe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2ojjldbgc.html


<!-- 参考信息 -->