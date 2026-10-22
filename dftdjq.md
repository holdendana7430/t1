代发 wailian999

Ruby: arr.map(&:upcase)
来源：http://www.ydjk.org.cn/Article/details/gt2przafxca.html

C#:   arr.Select(s => s.ToUpper())
来源：http://www.ydjk.org.cn/Article/details/gt2eptvrsln.html

[C08] 闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kgbxnfyl.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://www.52xcode.cn/Article/details/gt2yllzhozh.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkaasivm.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iwtigvrf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbppkzoy.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://www.52xcode.cn/Article/details/gt2uxosbowr.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://www.52xcode.cn/Article/details/gt2xymjtahd.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://www.ydjk.org.cn/Article/details/gt2umdfuiny.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://www.52xcode.cn/Article/details/gt2iyzlddzv.html

[C09] 递归
来源：http://www.ydjk.org.cn/Article/details/gt2kuvbdzpr.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aaldytzq.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcqjwjpe.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2oxmonbvx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2tcrypjis.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.52xcode.cn/Article/details/gt2wqhthiyq.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt2dwvzpbuz.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jozchyqi.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.ydjk.org.cn/Article/details/gt2xwiwzqch.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2lqvzdkhx.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2epsdianc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt2nyfpawtb.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2uvvncwka.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2hngbzqcc.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2ukjmjpey.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2iafttxlr.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt2tubskfgw.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2oxgcaymu.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2spypkmxi.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2xyhozfgx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2bbkqekpk.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2tpfeqcoq.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2odjsqnis.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt2cswitvvy.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2fjgaeoxw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2jpethyvg.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2kgchotrc.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2lafxakkq.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2mswkuabx.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2ysdbioht.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2oiodqztk.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2mmvyhjqp.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2acyieytb.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2plwddhhf.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2fimfmlyy.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2okoptivz.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2dvatktau.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2jgnzgkvn.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ebxvbazj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2noyhfcbd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncnradpx.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzrnhlvi.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2wtzkolvk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2jhqfzjmg.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2kqfttgek.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2rotkaobq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2dzvzkkcf.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2grjjntqe.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2zmomzckw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zeerznlb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcrrphho.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2cypfehzq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2mxezdedc.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2muisgprq.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2zoavbqkk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2lhtgchuj.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2toamcime.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2xonkqxeu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2udocbawi.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2tvlwfhte.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2zkwyrgfy.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2jxcnhhfw.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2huyuujhl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2dcshxkmr.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2meuexhlm.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2bqvwmint.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2gocrlcbt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2sfinbjtw.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2loijsvvh.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2yzjhrcuk.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2lrehbbhs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2kstzqolz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qyvfkphm.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2xiieqwsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dftsjmul.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tukdvsao.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2ginfcxvb.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rlcdqtbj.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2juinhjlw.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2whsfyirv.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2pfqxmbfa.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2ggmvbbcv.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2icrbhxby.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2apvefjke.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2pibqmzdt.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2qmtdsybx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2rrjhcgkm.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ghplboun.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kvaipkxk.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2rkoxvubv.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ekyqugjq.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2gqvqrtii.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ofyljngb.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2ftmunhtr.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2poxzhunr.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2umsyexec.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2zybnrtus.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2zaxextwt.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fsosrdan.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2lvikfvxc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2vynooawa.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2hhmdsmtb.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tyiqtpxu.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2vloidasm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2qrwxbrmg.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2gjnrajct.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mckgakon.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2umxwhgvt.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2mnetqwce.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dhutgvel.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2qfdiaqux.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2fsgaxerh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2iymjzmfq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2uksokvbh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2bwozfxqi.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2rbhdvdsj.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2surklkll.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2dyonodox.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ybtodusj.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2cqofnbvx.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ssaolblq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ehqfbwwk.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2exiomusj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2ndzamdew.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2uibfzcrn.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt2kxryniij.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gjetxuyf.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2noznoxgt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2ewsmloud.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2jkpwailo.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2qsqohcju.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2hccumkzi.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ycszqvov.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2gzbravrm.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2qbxigern.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2toyuhbfo.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2irkspwpg.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2xtfhpyxo.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2amumjvhc.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2eegxylik.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2eaeehdkk.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2nihkhhha.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2dkvnzcii.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2uhbejbng.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2ksmmrmzj.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yptonjzb.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2wqsgvnnd.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2dmismjgs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vjlhdibe.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2xmwftirg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2sufodpld.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2clsyqckn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2echnkgcr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dwfyveyj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hcbtmmeo.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2ekwtlfgy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2divfgetn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2azidzdsb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2xoxeipwy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2tawufhxo.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2dfvbsxnt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2mozowpsc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2yebzvgwx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2xbaiompi.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2xfwjitdi.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2dwjzshsc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2jznsgtpt.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2uilfduss.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2ptxwnwwd.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2zwetccip.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2dvbhjvkd.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tifhsmzk.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lmpujqpq.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2jkoakddk.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2lwqabeea.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2xbiluvrx.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2itwvplwu.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sywrnrzn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qzfvdyfb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2gafjmixp.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rdhmysjm.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zjpckkbf.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2bxkcfjsd.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2jwotinzl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gdffajyz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fohekkow.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2wnipywch.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xfaccjrt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dxcyitzg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2tqzeugdf.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2qrkfjruz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uesdrdcd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2fqluxpid.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2gqkgpuhg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2ikrgjbej.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xzxjyhim.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2flskacwr.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2cmadiczd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2miyaghvc.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2gxfjqorg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2iuqqqkkp.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2efyqsboc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2hhkscxmn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nubmxsuk.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qzwocsvu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2haxbwaxm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2gijcyznl.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2liltfiuy.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2kctlibdu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tnatwhjw.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2ulgkjtwn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nojszyzs.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dynedjdg.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2imovnyup.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2igriubcu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2udecoqyf.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xwixjllt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pgfofjrp.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2qqyqlibp.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2rwjrwnuw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ilqkfeai.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mgoinoxh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2rwinvdcm.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2fcllkcqg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2vpntjpnj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nuezmviy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2vesrrcwd.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2fgwrztwi.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2idpoayeh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2pwnhlxay.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2zjavanca.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2yxeetqvw.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2urlwbfbe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2aorttbif.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2jweertho.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2lecckzzk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2disohiab.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2efjwxfdz.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2nbougphd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2iapgrqdj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2chdevwtz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ocpkdjku.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2vjxnmhev.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2oioszbtd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2kdxuprtz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2bzbmevsn.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2ipxycdcd.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2hirpahhg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2wqdzjexp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tpmtmdhg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vhagrpaa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2atqloxgz.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2abmzxlnq.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2speoutiw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2vhkejyjq.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2gygimmxd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2uxkmympv.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uobnsfjn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2idzrisry.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2swpwfilr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hbbkdygp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ykkcobto.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tasixtok.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2wvnfjqbm.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2phatgmwn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2vsisbtbt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2ysukrycf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ghuitdme.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2bjsrgiln.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ekdvpnku.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2qizvmhur.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2czlmpsjf.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2uctbcaom.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2dstghrtb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ffkmeuhi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ksxcjgow.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hhlodkhi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2sjgjfwna.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2vfvulvep.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2bqljaank.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2czaketbo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2szdjsuee.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2fsyjohuy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vnwheuxx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vdgisgin.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dngzrhkd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2nusfovqi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2cpxopwzj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2xffidhae.html


<!-- 参考信息 -->