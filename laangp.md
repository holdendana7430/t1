代发 wailian999

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt2hvxxkawe.html

[C11] 模块导入与导出
来源：http://www.52xcode.cn/Article/details/gt2wbwfjlaz.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt2comuknkx.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt2aaalvpto.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt2ivniwhly.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt2kytvplru.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt2nnftjrka.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt2pxscaffx.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt2lubjrlqw.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt2ihjpzois.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt2xumisqse.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt2fdgvzgli.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt2kgnobdtn.html

JS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt2kekyhcnd.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt2vgwebtnn.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt2bhrcqtty.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt2ppanyhpd.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt2zafafruf.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vezriixz.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt2opdrxmar.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2umjjkrse.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hiwmrpzg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2kaojbcou.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lotnrlzu.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2tbcrjqpk.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2dgjeyeri.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2jhdmwoxm.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2arzbrtbp.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2luoytrof.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2pkaxvwub.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2tzixjqhg.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2rhpjvjfo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt2hcctzwre.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt2mudtingg.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2idwajkmy.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2htasisns.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2ampjubxh.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2bdtvqfse.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt2kbcykcpq.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vqnuleop.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2muqvemrp.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2ywzhjbih.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2pchxtvqe.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2bwoflgvo.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2yvnxhdpr.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2dupimvdl.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt2qobfgvvc.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2vbbuticj.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2kggbkfbe.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2aiafnknr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt2rnpvmfdf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oegxymaj.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt2efzegbax.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2xriljlqx.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqocvetb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlcaprtm.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2qepxqshm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edhscqno.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2vxjtorkx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2acujnjek.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2driwzjgy.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2rzvrlhnb.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt2lkheqjen.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt2genxugxe.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2guphyegl.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2rkwxyipb.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.ydjk.org.cn/Article/details/gt2dlqcpfuu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2mhodfvdb.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.ydjk.org.cn/Article/details/gt2nojcqjxu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2saunbkgs.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2klrjvfsv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2ernpbemb.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt2afbhkdmt.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2lmmdgwbx.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2yvaubxgh.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2wymezfzh.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2ibiyiyuz.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2owjqqqbu.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt2uobergdf.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2fawysgaf.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wlavuiwk.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2sqfxayfc.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2znvnoizw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt2udzyywal.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tknntyfl.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2uugjacwp.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2jewleesv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt2egmiqwyk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.ydjk.org.cn/Article/details/gt2livmhcgx.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2wustxziq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt2hmuswtbi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2vpgdqpdr.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2bhwicgcl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt2cylbnprd.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2rgrnwvtc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2owhjqfbd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2vhkelavf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2wyroylhx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2apmjshif.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2ndcfnmhw.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2bquitnuq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2sotjxwdm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ajvahvwo.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qdevkzkj.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2hmqklaeh.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2gmfxegzt.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2hybfmndq.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dqfrwfss.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2wnfznmom.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mhjpbcxs.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2pjixfnih.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2kybscgna.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2mensnyju.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2lnuneiws.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aadgxukr.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ltbpgesv.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2byjfinto.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2lhbxjhsu.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2igjefhvr.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2cbonjtoa.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt2kwkgaxzy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2bxrugrte.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2hrfgwjwg.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2wfhyvgim.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2kmuirwre.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt2dyrbfcsi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2fpmodsdo.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2uehdzrcz.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2pkgbxpis.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uprdixsm.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2xnnifacl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xwpkmfzn.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2vkjgfpfy.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2mirteplh.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2alomoizl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2nukorgsj.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2gtbytfgr.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dsstbwly.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2qajlpaky.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2ensksjgu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dfysmgik.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jhklwofp.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2wshjbzdq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2ednmddzk.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2ffpucgqs.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2lpmzasyj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2dqcdnrop.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2blpaazrv.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2vzomizzc.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2cdkecufj.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2quommorr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2pxdwegid.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2ajgnzamr.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2mldlzqet.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2wyaqqqwz.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2mpkhamst.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2mtqmrkiu.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2uvavzmdi.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2irawxeye.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2advlxptt.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2njuvoqea.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hxobcswk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2vrfzlrnk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uwlnmdiq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2roywawlg.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2rrmvrecx.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2nkjsfjhf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fjmldqur.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2swydqpbn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ibohhwiw.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2plabhgro.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mxjanrnu.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2gklzokav.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2aplzafqk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2pduhqves.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt2vcgrsjlg.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2oolgqcjx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2rkuffnsi.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kmzhelhb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qwyoekxa.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2cuytjvgp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2qhxvmwhu.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2efbwsyvr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2qfavoltr.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2dqsebket.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rrxekfwp.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2slpjntxl.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2ehhsawxl.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yomexyft.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2qayxtgts.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2szfcpqfo.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2kbjvrhuj.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pkxjcgwc.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2xhvkqpwx.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2qsgnjzay.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ehtirzgo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2jsybxutt.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hcmgdrpl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2baqzvbkf.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2mygzfrsc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uzhwjsoo.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2eqphpupm.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zfwzmvjc.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2didtktfc.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2oixdmpnz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jpurebuv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dqxiuhwa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2aofyatgl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2zpfvngkh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2znrgekhp.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2pvwibqwi.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2xlaeahku.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2lyyeoxlz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2yeoxdlzz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2zfcmwdjh.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2kaipefyc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2doywsstt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2nbmzicdd.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2omzeqbxy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2hbraeomo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2hbbryenj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ghixxvjt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2htcdkvkg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2suofqbyx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2lbruwjxa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2xwakwjdd.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ppohcszk.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ttepueuh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vnscmmaj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2zmmpuabf.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2zxufgcdf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bolpiipf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2rguygywg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2dkbaqxdr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2dzvpslen.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2dabobtvk.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2fpdhkiax.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2dkxpioyy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2slcmvzfe.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2wunuiztr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2pencgubl.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gnnqdyvy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2wohoiwxw.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2ofkfsfay.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2eusfnnpo.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qkouqatd.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmozsqpk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2uxplbvjd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cmmqjfya.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2hgavqqbd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2iuqelwpd.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2hhrhoalm.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2gdutailp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2rnsrocbq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2idxthvbd.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2okrkspff.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2gcdlaymd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zhyalkcf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2caiofjyf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xjufftdk.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hhsrbjix.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2jcaamrqz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mjbwcmuv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2uyvxhdfx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2guithpwl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2pcahsvlm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2frvganas.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gdlcduaz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bsaclnmh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qtaeqjyn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qwpwidlp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2glzhdvpy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2tetplixs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ugtkbpmw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2gxoyjbkl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2nbdyounc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2arcrsmtp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kntjpgpx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2nljejpgz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zoridsps.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2wdmuzwjw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2blgvfprb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2edwioaly.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2awqelkyx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2arxujrzi.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2koytsiyw.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2acoqvfbr.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kucrdubz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hzwdzklm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2rhvehdaf.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2auwkronn.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2dbyysgbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gfqpanmd.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2klibmgte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwqbixnb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2otpsamuj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2oketansc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jgucfdtj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rhctqtjj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2sqahohgj.html


<!-- 参考信息 -->