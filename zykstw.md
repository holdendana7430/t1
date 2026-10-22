代发 wailian999

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2rbhqgusc.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2dlnfasol.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2alteckpa.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.ydjk.org.cn/Article/details/gt2mubzevoa.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2gjjyxtcr.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt2vwewqbfm.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2qweouhcl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt2qumpusqt.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2fvwqoows.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ayitchqa.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt2afmenoxe.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2qyjcqyfu.html

PHP:  (function () { echo "run"; })();
来源：http://www.52xcode.cn/Article/details/gt2rkynyibh.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2sozltlpj.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2ovdlriir.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt2qlyrnqzm.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2kcxsueog.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2myxppmvk.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt2alrkduwq.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt2poxsmmms.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2uvhhwbds.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tttvxctx.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2ofnkyjka.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2shprsmfb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tkbplixh.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2alsxjesv.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2clxnqsto.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt2svvihftu.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2cqqhsjqn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2auzniovn.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ykveesxo.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2ekubkwhe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mohgmnub.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2nxxyurbi.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2kkbwnffa.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2tlficxbr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2nmnmwuop.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt2kmaaajel.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2qehscgno.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt2kydyecjr.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2uucnugoj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yubnrdzg.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2ldhhezor.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2abzfvgwb.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2tzixwdxl.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2byngjntw.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2nxoqiivn.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2wkrinwbx.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2dmeuzcrd.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2vbskzkhk.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2fmdvqghv.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2bvrejfer.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2dcuettaj.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2twkbuobq.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt2lcrbnwyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2peuvczux.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2qnbkflac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zoyicmmm.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2tzxurzya.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt2uvuwwqnq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2qpabspba.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2pqtwskbm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2brmifppi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2uewnrtmv.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2itfjcwml.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2hkxvrphw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2kpughwcj.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2drtvjxdy.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2squyjnzf.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kwmokvzj.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2jfabklcr.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dgzdcmxp.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2ggtaerqj.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2fkipnfnx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt2etyquzhp.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rjhzcruk.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ylkyqvqt.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zzbshvlc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2ucathyml.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2hycvwhvj.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2hlblmhjj.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2qkazmqtp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2djkjhuqc.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2qxdzsvyo.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2blvqqccj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2aksqgwms.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2rhzbrocz.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xsfurcre.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2vnyyuwsq.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2mbesmnai.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2tsbxvsrd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2hoxmnprs.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lfqxpwre.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2kpmalssq.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt2pludecwv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bfkdpkox.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2czbmdmez.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2fumaqprn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2flgcnidl.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2jqrwbszg.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2nhhfdife.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2csbthpdf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2rwhthpgw.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cpwfkmnm.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2pelontdz.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zftlrbcj.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2vekztdjv.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2bjsatwtt.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2kjsflhwe.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2ydkoxfun.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2mxhjfghp.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2upzigjnm.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2mfakkewq.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt2rljjtpzx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2yrlusoqk.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2zbokqiah.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2wpxqptby.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2ymddoxlp.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt2wgplbuok.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2xhnxqllm.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2uruuvpfr.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt2snrdcwya.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hjbyzfak.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2kmwthgjl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2qgsbxhvt.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2wkawxjuv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2tyjraaim.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2dhlaeyby.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2ucmhgdim.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2ylaueaql.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2pgneyrnz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2cegjkrlb.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2bltorlmw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2vixleyhj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2htraoixj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt2kkpwmaoy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2oyhmwqli.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pxhasccp.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt2neytdpeo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2cbehkyvx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wtqxrpgv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vlggmybc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2fpwcmdau.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2feisrlxv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2ioxtagjt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2fxhdzxnx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2nuukjmkd.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2ragbrqau.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2cljyfwtx.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2rkrynxdg.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wmtjcqjv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2yycdcrba.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2qopvvaak.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ppttowir.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2zxqomunn.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yllqzqga.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2pfyxviqo.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2oaybgjco.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2hgiydsby.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wdepcixp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2zeotljkc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2wkcgwzsk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ndlosirg.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pzedvwqk.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zyuxiygd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2bgyiccqg.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2sqbcxosm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hmermdsp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2nybgpvsy.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2jrnyexay.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cjnrqiyr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dtplbdyo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2jfpvybkw.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2lmoaheus.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nxqtedyo.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2aathmgmz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2gnwtuyrs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zufioprx.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tehtyedt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2hnwtmfgq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2przvsjzj.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2pnzjyawl.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2myiyiiju.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2nzixobvr.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2swkmisus.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2mnvhbpkn.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2excmapoq.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2eswamylf.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2iizlikdr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2sjzhoxrz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2nmafwdfh.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2uicqvxdp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fcqkmsjv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2lysgbulr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2zkysozyo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2phzglwad.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2iwjalsvn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2yzktvilb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2dpdfmjgy.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2wogqjcqf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2rdpixddn.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2epipeijn.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2prfsbevv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2znqiscqs.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2jbnkzbcd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2mbidzlgw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2jvaxjzpj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2xhupkmot.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2stbefdfq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2przgvfow.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xjeaodhy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2gbkgedac.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2dkfahelk.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2gnoihjts.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2kxtaqbet.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2beqwquvo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dpbpugeg.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2wqpkcnmx.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2shgvcolm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uwhyiiuh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2mdetbrab.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2drrvncia.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2uwajggjc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2bjdtczmg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2gebrxheo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2qotiwvji.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2kgkxlhjz.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2ffsdiisk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2rptbeyes.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qeqsuzsf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2pskxldge.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jrszrjze.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2waunjgur.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lgqcsatc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2vxkmsaov.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2mddwbsrw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2krdezbmv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ijbvuguz.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2tkavtzlr.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2hxsqgsln.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2ozhrutjh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wwzwfdno.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2djhdioxz.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2biymzkgy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rcybvynj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fyaoquxs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2kchhtxjy.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ugbzeler.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ejqsnimy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2immrfydo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2owiufubq.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2zbzpecau.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2fattzgsd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2zdhjjdbi.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2xkbedaow.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2wrqtqkig.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2rvkaolma.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2qegxodws.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2glbbutgq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hhwgpgzm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kffkdarb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2inufrdsc.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2zaiuaukv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2mydzzgru.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2sovnixut.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2kecxzzpy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2dlrzalyk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dzrenrfz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bqjvdpvu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ezavmara.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nlsgphbb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2zlujunib.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vohbdkqo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2nvsyqlxs.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2lgsjoopr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2ggpvbpsw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2psxyqtjz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zpcezwzs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2tsidtghu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ryyyjlan.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ialvlxpd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ubvgzatz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2bpxlydhc.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2udhpqqpl.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hojdpsbb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jhpsorzl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ttbjrdml.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qhclhnam.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2newsdqek.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xaovvfsp.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2gkmrovdc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2druufrsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nhxsnjec.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2jimlnycs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnxghdub.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sdxpkrfn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2jezqwruj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jxkxjmke.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pukilhvv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2clvbodrc.html


<!-- 参考信息 -->