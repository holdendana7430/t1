代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://www.ydjk.org.cn/Article/details/gt3stusjixr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://www.ydjk.org.cn/Article/details/gt3mivalnoy.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://www.52xcode.cn/Article/details/gt3ywjdbyek.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://www.52xcode.cn/Article/details/gt3ewujlbgv.html

[C10] 变量作用域
来源：http://www.ydjk.org.cn/Article/details/gt3hsfrfjfz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://www.52xcode.cn/Article/details/gt3qfzxfqip.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://www.ydjk.org.cn/Article/details/gt3zstcqedv.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://www.52xcode.cn/Article/details/gt3fptfcpda.html

TS:   同 JS
来源：http://www.52xcode.cn/Article/details/gt3digxwjmq.html

Java: 方法内为块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3vlwkeiqo.html

Go:   花括号块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3qjqlvmxw.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://www.52xcode.cn/Article/details/gt3yqljegyx.html

C#:   块级作用域
来源：http://www.ydjk.org.cn/Article/details/gt3dmgmpgjp.html

[C11] 模块导入与导出
来源：http://www.ydjk.org.cn/Article/details/gt3gdohoilr.html

Py:   from module import func
来源：http://www.ydjk.org.cn/Article/details/gt3aidcnwrc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://www.52xcode.cn/Article/details/gt3rbvmjzku.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.ydjk.org.cn/Article/details/gt3gnsvmekj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.ydjk.org.cn/Article/details/gt3uwzowjed.html

Java: import java.util.List;
来源：http://www.52xcode.cn/Article/details/gt3wygonqkz.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.ydjk.org.cn/Article/details/gt3evvmeotb.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3ncqvwwbt.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3imliniey.html

[C12] 立即执行函数 IIFE
来源：http://www.52xcode.cn/Article/details/gt3hfggkcaz.html

Py:   (lambda: print("run"))()
来源：http://www.ydjk.org.cn/Article/details/gt3vfhpyazy.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3pxdacmvr.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3ncjavhan.html

TS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3fxwwzavu.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.ydjk.org.cn/Article/details/gt3oevakaxq.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3zkhnjsuv.html

Ruby: -> { puts "run" }.call
来源：http://www.52xcode.cn/Article/details/gt3kulvmbtu.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3grbgwnzs.html

[C13] 类型声明 / 类型注解
来源：http://www.ydjk.org.cn/Article/details/gt3cvfbvyfd.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3bzrpzxdy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3nyvatrju.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3unevwfjk.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3umullzcd.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfyydnrb.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3suyajicm.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3mcemlmga.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt3svkcchga.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3bghdgbwk.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3euprwuld.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3hcddrqty.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3nlaljdlf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjnxietc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3bghchxwy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3kdgeebek.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3msnhxqwu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3kksyygfm.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3flwzpzno.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt3zkdoemkv.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3dnotaber.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3adlhwcby.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3krracnep.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3unfxazdd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3hqovxflp.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3awloupsl.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3zrxldvfo.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3nkwygrjl.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3ydvtfolu.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3kpzosclc.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt3xrlrejyo.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3kzqhonlt.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3djdfxnvw.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3rksfgddv.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3sogfvzux.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kdlmkzii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tyejnxjw.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3sttjaffq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3usdlarkg.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt3gzsrvyua.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.52xcode.cn/Article/details/gt3yfqcaphe.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3rrhzuqqq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3migeuxbd.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt3sziedwrr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.52xcode.cn/Article/details/gt3kxfxqpdl.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3hvtbfnpo.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3iasaucyv.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3rnbgcetu.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt3slujuzxn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3dsmtkkml.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3nwgdpitg.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ljwgkyxd.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3ilpeente.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ktrpqcpn.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nziiymnj.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3zogkeymr.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3zinhzwev.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3tihrerea.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xrlrrgny.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.ydjk.org.cn/Article/details/gt3tyimewnt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt3stjplbqd.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3klskbcvd.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3gqzfvvqa.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gqjvvawh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3knwzkrnl.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3vnwwqbdo.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3djtrmojh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt3jggzfjfk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3judausks.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3fhrhudxg.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3gdpeeppi.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3isahrmrq.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3lzvqvoln.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hgekfrii.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3ajflkyxv.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3tdvpvrrj.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3rnrxxmbx.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ulowtasr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3icdsmwru.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3giyrzxno.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3ajddinrx.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3lpgnwbrr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3klvvapmo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3ibijeyap.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3pwhleacr.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3cevhgrbl.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qttgxawf.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3eknenpwu.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3skrzfswg.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3heczgvsq.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3azrjcijm.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3hwdmofzp.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3dnulnode.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3hzqzmikn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3ydsqvghb.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3lmdqgted.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3cwgnzwlf.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3vcdmlnpb.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3zqpmexlu.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3oikwlrec.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3aeuosgdl.html

C#:   list.GetRange(1, 3);
来源：http://www.52xcode.cn/Article/details/gt3zwrfbgem.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3jjdouwyk.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3yaqbgwvr.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3osytvyoi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.ydjk.org.cn/Article/details/gt3ntjwxgif.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3wtnikrsc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3cvgprzok.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3szcztgiq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uozqlnkr.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zmtogyjy.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3oflhylpp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ypjrvwvf.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3twwnreuq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3iicyyell.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3svxtyhox.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3bcmiqvdg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3cjioxecg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3srifpnkh.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3itnnvuvk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3jlhkvbny.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3cwqxcejh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3ugrmylos.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3tiufmrkf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3qbymnrae.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3jibgqsdy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3qbuizyen.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3axzwuncf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3ibkicfvp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3tjziuliv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3dtlikqhf.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qtcuknnj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3pziflzzg.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3amihoars.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3erpawpvy.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3lymryjvi.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tmlwoxol.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3gzscjqeq.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3fqdgocxf.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3vqwabysm.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3zhxksfpd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3gogitphf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3osrjrcpz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3rnwxidgh.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zdbtphta.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3amaxmdtk.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3aonhmdxk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3fuompbhx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3hbbiptbb.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3kjjpcats.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3gnxvmujr.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lywswrbq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zetrhshb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3aehzoqcb.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3gzfsicuq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3znelphcy.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3vfioqzmv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xbdbmoao.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3bcqqckcg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gfjshzwj.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3drnxcord.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kwhtgynp.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3snqhnvzk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vwntgqyd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3uevvgtfc.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ohydhthy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3zviosuab.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3jwmlasjz.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ojdythvu.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3nrsjsybp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3apnzrnec.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3fopacqjr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3lqvpdosp.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3dtevddog.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3iblmlfzs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3wdtcnkxh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3mnwgwrgn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3qofslthi.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cqizagaz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3ahhsflhv.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3etroxbis.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xftqkkcx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3ydcmcped.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ymeskggp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ofwhpbzd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3cvaulozc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ofveixri.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dongrqgy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3zienjnor.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lwrvbkjq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3uhpkwwgc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3avausdlq.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3sjztwjsk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3fzvekqqj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3svmvqavt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3lirxzcro.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3bmswinqf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3drpnkxmn.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3xucfgufi.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ympotfip.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vapxvycd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wvapabwe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qkloqmqi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3eosvrifv.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3dggnllmk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3uanroxjy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3fcbdegaw.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3dtqzizil.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3jsuyainw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3kktkvrfj.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xzfctcqw.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hgssnith.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ggmjpmsv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wsdmsivy.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3xxhqojha.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3hbdnhwjg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3fxkikftw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3hyqibztx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3htanfpgh.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3xfotmrtp.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3ogsuxgom.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3sebirwof.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vsxggypm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wfvoiasb.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zpszjyxp.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fucjvlom.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nzzbkazz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cmhhkuuv.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ausakfzp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3humbmnef.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3pzwyxnoz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dueoizaz.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3ohcpkiwg.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3chbhuwtc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3hfkptovl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hcqxgkrk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ybttihhh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3qsntszmr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jnaihnqi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3jnlatqww.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3xzjduxdh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3mxhsisnm.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3jidvssuw.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ipayopzb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3sxyujypy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3mbnpqlzx.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3zzpgjkzo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3oyetboyk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3rrkrqvby.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3jpamkqli.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hdwgxylh.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3eujpwsfe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3qqtvzhbt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yqvdcuwh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3bbdggzdv.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3drmdcltg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3vgnwzeit.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3qviemjja.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3yvvexpzg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vxfpbqxu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3zmoswrya.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3xzojvtqe.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3nnyxdueb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ygfzpsao.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tsqrtffk.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3twtinolg.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3cbtngbny.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hcjhygjl.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3btlpqbol.html


<!-- 参考信息 -->