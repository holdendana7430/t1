代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt2baotvsdl.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofnjdxfr.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2jpphtvxx.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://www.52xcode.cn/Article/details/gt2temjwztj.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt2eitatofy.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.52xcode.cn/Article/details/gt2jjevxmkx.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ymrfqeyl.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt2itotzpen.html

[C10] 变量作用域
来源：http://www.52xcode.cn/Article/details/gt2tgphikcb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt2ebwuckxc.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.52xcode.cn/Article/details/gt2orbfyysd.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2bylhrhrq.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt2ugzhyien.html

Java: 方法内为块级作用域
来源：http://www.52xcode.cn/Article/details/gt2cwgkxplm.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2tvqktmwc.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.ydjk.org.cn/Article/details/gt2hpvwecgs.html

C#:   块级作用域
来源：http://www.52xcode.cn/Article/details/gt2qienvzsm.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt2lslshgiu.html

Py:   from module import func
来源：http://www.52xcode.cn/Article/details/gt2vjcaxcww.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2lcxitucc.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt2ateytauz.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2gtbrtiik.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2ikggzhdq.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2tazutxiv.html

Ruby: require "json"; require_relative "./util"
来源：http://www.52xcode.cn/Article/details/gt2hzmdeyel.html

C#:   using System.Text;
来源：http://www.ydjk.org.cn/Article/details/gt2rlzozfgj.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2zfekvjla.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt2wxyjfvnk.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2jgvfjzrn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2uauacznb.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2zzjvoytt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2hpgbyiyz.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2cxgqkoua.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2vnbqkmuk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2imnytdyk.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2afrqyvmh.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2qgbajmmf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2sehxgrex.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2wnorhanv.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2wfaddbtb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2zichyyav.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2ebvdykkf.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2kbyxzlis.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2alalotwd.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2uklglooe.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2kevjyjak.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bgohyqjg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2iwvlahkp.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2zwvwluvk.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2axmyzcvp.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2bxnrjsdr.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2durupehd.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2ffzkrgcz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2whcnkzvw.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2rqxxofjm.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2qzcteqwk.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2uqrtubzu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdhuvsdy.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2zqsswoub.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2iybtgzak.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2tarrwlwk.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2nvpauigd.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2lwfxznpa.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2inqecxfs.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2mzzxycty.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2ypezsvvm.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2iupxjknf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdreskkt.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2bawawqvg.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2ucncfixb.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2aqehnyrm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvvkyhnb.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2okkbwskx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lhqryevm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ijbmmaxa.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2msepvnow.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2mwabfdxl.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2umauszee.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fhqbbhuw.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2sgrobaqf.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2cybcmxve.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2tzqbubvc.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2vstmgtup.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt2fsdvvohi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2ecenbyha.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2ohyjpatt.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2bbscpsxz.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fjmiwkos.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ovhitovb.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2pnwsvlhe.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2emoobrpm.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2bpjvxsta.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt2nkydxdcc.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt2phadofni.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2dvhfgldo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2lldtdpwd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nuaeecaa.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xkqasjtg.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2lfxwyxyq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2gatwgwzg.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2oxpjiaig.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2vhroqreh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ovwtzrvi.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nfxdjtjo.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2vmosvisd.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2agwmqvrn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2tzixwpak.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2kywewpjl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2mlvwetcq.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2rnwdsoqw.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2bepmiloi.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2ssepmptg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2zqwxaoyf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rdsgxhpl.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2kmleqfmh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2wuxzvmwb.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bsrleptv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2evtcmlmi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2ykggpcio.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2sklzuchu.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2emqdzpmi.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cylsrlsv.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2mswhzuxn.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2vlxjveau.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2jnkpozns.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kvlmgnrn.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2azbgkeio.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2wktsmmpw.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2gentxoxq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2oyoedqne.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mkkmccel.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mfacbplr.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ocbtgffy.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2mqkndany.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2driuvplh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2qrdgrzha.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2nlzbmmdl.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2jazznmay.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yrptgvrt.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2vvomfrxo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2zcyodtrw.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qrmkkvsk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2evamtyxg.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2dcxydwfo.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2meqasxpa.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kmzfiobg.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2ajvrtpek.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hcjvtsoi.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2lwyurqag.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2rrfjyfbj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2krhqnzwv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2vlfnllzc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wcfpfmqj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xzasboda.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2tznlrwtu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2uvpblrgn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lnzzyuxc.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2pyunaqsl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2hcsqwxof.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2vxuehoyn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2vntpmkru.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2vvrexfub.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2bcribngf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2arqufwmw.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2bballost.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2rxsgazqa.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2pzmvscrj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2gqyxqgrj.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2trohsvsd.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2tcbvsyje.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xbqbgzni.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2fiyolarp.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2iicukoqm.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2ofcpanzl.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2ehibvnma.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rptlbtny.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cgnectqg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2akdusszs.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2npegbdgc.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fxnkcwyk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xkxcxqwt.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2azgcxsvh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2vfpzpfnc.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nlgbvivg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2eptunugb.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2efhoteeo.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2yadzjonp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2qpwotuac.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2xsrskkam.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2dvqvnise.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2omrqiazc.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2zpisywfa.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2mxoiliay.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2bqxbiugq.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2eogqpwfh.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2immlsrca.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2fysjaqfz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2yavxqzcw.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ocxuctvo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fbdbjdwk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2xnpqmgah.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jdjeaxur.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oqblohfs.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cgykbmmy.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2gdondbpd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2ewcvolmg.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2binnwdmu.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2pqfnnqxl.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pocghjat.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2dbtgpxpf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ebzgrbuu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ieyapjpr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2aozqrori.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2nnfrvqvz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2dnkcviqn.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2djsqwyom.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2akftjcfr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2grvxvsgs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2enihufmi.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xancszyd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2scwhibxe.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2kasjwxcd.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wrcwoybd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2awqedugi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qalnlmqt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2gujxrfoq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2uetjkejj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2iseqqwml.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rsppiwxp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2qzliibpa.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2wkprtmup.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2cawuabmu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2sztecnsa.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2uldhlpmi.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2rqksdyox.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2agidxkjk.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2nrzupxyo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2frzlwfzd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2zgfhmkkp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2owqhznod.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2dktigozt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2cosadzjk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2iclonque.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2lgxdszhz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2musxnwks.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2rhthnqkk.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzregeoz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2hwpcasyp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2tneehvqq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jpakegce.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2emthiczs.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2stchlwcu.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2ozvxfrqr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2aerputuj.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rtclubti.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2hnhtpuch.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2jkyidzjr.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2zdohcfgr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sxkrcvfr.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pwvkaccm.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lkktouzh.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ghwpwkru.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2cyolwxkz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ohvaodng.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2tgomxapm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2lounlavp.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2tmmzvsbb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2eqjmopha.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xrzrwjlp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2xlpzbkde.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2oiwnjozn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qjkggruf.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2vgnkhqng.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zmycfniq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2adzkjqxy.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qgcvoymw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2yvqdpcas.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2fvksgcji.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2uwwfbiue.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2qeiixohc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ongamqzs.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2nzlfmsff.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rpnvajvc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2uhohpchm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2wgiqxrvm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2hxijrtdv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2odqjxakk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2qdabdrxl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2qpjwkfxg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2rcuxxgyl.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2nuyapgeh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jmosnoyq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2zvvdbzfb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2lowxecht.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2extommuu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2vslehzhf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2rzhpisbr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2pqoheduf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rokunrxr.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2jwnrwpex.html


<!-- 参考信息 -->