代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://www.52xcode.cn/Article/details/gt3yqohmowy.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://www.52xcode.cn/Article/details/gt3rafljmfa.html

Java: import java.util.List;
来源：http://www.ydjk.org.cn/Article/details/gt3jvtvpbib.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://www.52xcode.cn/Article/details/gt3cafalidw.html

Ruby: require "json"; require_relative "./util"
来源：http://www.ydjk.org.cn/Article/details/gt3wujjvaux.html

C#:   using System.Text;
来源：http://www.52xcode.cn/Article/details/gt3scxwcyzk.html

[C12] 立即执行函数 IIFE
来源：http://www.ydjk.org.cn/Article/details/gt3iejosykt.html

Py:   (lambda: print("run"))()
来源：http://www.52xcode.cn/Article/details/gt3ckwlthil.html

PHP:  (function () { echo "run"; })();
来源：http://www.ydjk.org.cn/Article/details/gt3oibhkuvh.html

JS:   (() => { console.log("run"); })();
来源：http://www.52xcode.cn/Article/details/gt3mboyfyct.html

TS:   (() => { console.log("run"); })();
来源：http://www.ydjk.org.cn/Article/details/gt3mwhcphki.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://www.52xcode.cn/Article/details/gt3vhuitcsr.html

Go:   func() { fmt.Println("run") }()
来源：http://www.52xcode.cn/Article/details/gt3uyxqmtcc.html

Ruby: -> { puts "run" }.call
来源：http://www.ydjk.org.cn/Article/details/gt3yzivykph.html

C#:   // 无 IIFE：用静态构造函数
来源：http://www.52xcode.cn/Article/details/gt3vzqicvua.html

[C13] 类型声明 / 类型注解
来源：http://www.52xcode.cn/Article/details/gt3ryylqwua.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt3azanscjl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3jmixlpxg.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt3fqpgbpsc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3hegfpcrb.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbtcbzag.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ckxxeumw.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3nchbtrzi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3vgwodrte.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3flhcbvjf.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt3hnkmqdgp.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3pxkmhgex.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3jceewwoa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.52xcode.cn/Article/details/gt3pmitemri.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztbwgdwl.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt3nxuwtgwj.html

Ruby: # 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3gdwrpkbb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt3jkqqxepk.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt3clvsdytt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3apfullvm.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt3txhhhsxt.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt3lfuntrdy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt3bjxzptty.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3vhfltqtv.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt3nqyxyskh.html

Ruby: a, b = pair
来源：http://www.ydjk.org.cn/Article/details/gt3jpqomxae.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt3ecmfvzuj.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt3klbyebed.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt3zcnrarit.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt3ftczwxpg.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3qpuvikvt.html

TS:   // 用联合类型或重载签名声明
来源：http://www.ydjk.org.cn/Article/details/gt3frsgithn.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3insfyhye.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3ljhhazyl.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3pcyxzvas.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iihhnhpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3avfcfnhj.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt3lijotbxh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ujvtgyyc.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3qfeakbzr.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3nvamntjl.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3kwfeklgz.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt3vkkdeicf.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3mlzeghsq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3apjahxuu.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt3itjgzeow.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3toqlqoel.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ylkbfyyy.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3znvbihrs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3zzmhxvic.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt3dqgbxsqz.html

JS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3owqxnxpv.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt3eltfwdrh.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3hzyzlmwt.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3dtbumifn.html

Ruby: arr << 4; arr.push(5)
来源：http://www.ydjk.org.cn/Article/details/gt3yswxuyak.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt3olkqddhh.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3mukbkcia.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3iumoeaji.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3ulbxqdoo.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3yftbjjhy.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3bsfbdtji.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt3xzqkjxjp.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3gjomvuyu.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3qreugffl.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oxknxash.html

[D04] 删除元素
来源：http://www.52xcode.cn/Article/details/gt3lmaknjjy.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nupjenso.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gkwqykpe.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3amrmgcej.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3klgrdukd.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zxotfpmn.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3jdbhmqss.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt3euvinuhf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt3lsvrnjpo.html

[D05] 访问与修改元素
来源：http://www.ydjk.org.cn/Article/details/gt3moqqfzip.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3riwxvpfn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3denxccvk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3eybkpttx.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3btdzfhqh.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3xtgoqniy.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3gffaldun.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3cncetwft.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3gixltzbl.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3axeijybx.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3lggdoavg.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3tjdndhoz.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3lkutcqrb.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3opeozeqs.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3hcoamhqp.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ckjvhftb.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3lhnarebn.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3yuxcxwuf.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3mqtavvxz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3hyptwklx.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3vxubmkym.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3wxwgfkpx.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ovcjfkge.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3yjwhoezb.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3dzfjjrbj.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3aqlrpmyr.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3bjyyxxxy.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3bjugnejm.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fikepqug.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3ykqujhoh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3yakeyypc.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3rygqwvrm.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3urgszrge.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3ideytvkf.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pkwoyngz.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jyheslqv.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3ycrytrkg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3hcwujoli.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3idoieile.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3ufqrjfyw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3vrzthulh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3rblxhajx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hskbzgxx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hcfbffba.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3sezapsnn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3youaufoz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3mibqeohp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3outypkpe.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kaccpzql.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3lcxkmces.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3wogqhyny.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3xhesowsu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3yqmlqvzz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3dbpqwgjp.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3pmsecgfl.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3wlwnehsn.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gkraozbp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3roayotpb.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3ebjyukoq.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3cswceszi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3vczfhssx.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3revkoxyq.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3yfussvia.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt3bftnzyrs.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3humxwkqj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt3bhmglxsl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wemyfhgy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cjemgxhe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3xmmuhtnk.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zoqvlvgf.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gehjmtoq.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3gftcnvzg.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3ejveklau.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nwdgetvx.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3yxdmkmao.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3gjqvrmdd.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3rwardurz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3sgzznrxs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3ksxrmmfk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3cxrlagsa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3elvjreli.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3rnhtaklv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3bnrgtszt.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3frsvknfg.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mhtxhszp.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oiedskph.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3cennamuw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rkbofzrg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3itfwksyd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3okimomjt.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3tciqfvlr.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3dldvyyuk.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3zvkqcoik.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3enmlievj.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zqmxplfk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3bungpefw.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3rzoljiaq.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3gvjaptna.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nuenlaln.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3xyavumic.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dwztdedx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3kssnclly.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3etmlrhfa.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cxgwwdil.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nmmkuwvl.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3ybkknodc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nhuulaqt.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dlohtoda.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3xwxtxrzv.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vhblidsl.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3cggrxlze.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3wdvzjbbs.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3davrfjwq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3yhacxzdo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fukuvkge.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3qzmjnlzo.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3olfxaxgi.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3klnrwynl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3zqrkgjbu.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3pbsdlzyk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3dfginyib.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3ghhjvecl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3acqsyhoe.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qrlxzlvm.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3lhekqqvy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3gfypkunk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3lwtfdogx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3gncfhley.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3yfrzuhwt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3ftdakfrs.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3pjgvvpmn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3oozdbltg.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3saxudvkh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3sekwucvd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ayqavtcy.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3awazsuok.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3pibveycm.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3utxjvnvs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3eluidjqu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3epbqkbjs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3lbaptxdt.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ytayhcpc.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3nztxvppr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3thowgygb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3vjworbad.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3shmyswtb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3kefnopps.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qaltzoll.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uefwjryg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qjjsfkfq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3udzflnzn.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3frlnlnnb.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qvwkmyuy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3ligktdvj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ipzocsev.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3pfwqujhw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rahtveyi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ljetlryu.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3kcsnrhnx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3rakufdgj.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3oenbfldv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xaeggctt.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ejnybkdp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3yaetytdv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3pnufuttk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3bywdshze.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wmlhxrfq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3dynnrwhz.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3huazydhc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3urrxmnmz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3hrdacyzo.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3qadiodpx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jtnvmurr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3nmmqjegb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xculuqzv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3wndntnur.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3uzdeslrr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3snwjvdeq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3vaqavqaz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3olizsvke.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ogxmqahg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3vxapiqxi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3evsmxtws.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3tpkpmurz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3leeewwei.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3opvsdeag.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3uceafssg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vptvudgk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ivrwwbih.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3eghyvggk.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3mppantnu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3lwskpxkk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3rbjgxbfe.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mpnqjnij.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3spvycvib.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3eynooava.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yjnwjuml.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3lfpplvue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crwfvhen.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3skumhqrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3amakhdtf.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3sxfjkpxd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ckayszek.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ijgqtcda.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wncnnshf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3lsneclpz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vdfowocn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lfnrbymg.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3njergwis.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fmkyxjew.html


<!-- 参考信息 -->