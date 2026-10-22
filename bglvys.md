代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.52xcode.cn/Article/details/gt2ddvkydva.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2hnlpzgxv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.ydjk.org.cn/Article/details/gt2tmdnzaxo.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcdzlfxc.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.ydjk.org.cn/Article/details/gt2syidzfdi.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt2qooeswty.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt2ayptxeze.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2iuclgher.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt2mvxshgto.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt2juzcwkse.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2isylnvlf.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2moncxhpe.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hotcxalr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2uxklhrod.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.52xcode.cn/Article/details/gt2eqcaeawq.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2ispqgnpw.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.52xcode.cn/Article/details/gt2pdytkpdi.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ttsdtapg.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2vreqicii.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2prvgnifg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uefazkml.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.52xcode.cn/Article/details/gt2fjlckznd.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2mikvjptc.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2vwupawqc.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2adotnyad.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt2sqyulcxn.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2opezkehb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.52xcode.cn/Article/details/gt2ostfwdzo.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt2foznosrn.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.ydjk.org.cn/Article/details/gt2bkmzljlv.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2otlxwuev.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt2upqgafzw.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2wtgfnphs.html

Ruby: # 无重载：靠动态参数
来源：http://www.ydjk.org.cn/Article/details/gt2hdufbubh.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhdhxbeu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spxokdmd.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt2faejuivd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cayhmsqz.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt2veczbnwn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2ghqdvesi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.ydjk.org.cn/Article/details/gt2vzqbqcyb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2lwvaxewh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2hkkrspnz.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2amlkvkpr.html

Go:   arr := []int{1, 2, 3}
来源：http://www.52xcode.cn/Article/details/gt2hdbennck.html

Ruby: arr = [1, 2, 3]
来源：http://www.52xcode.cn/Article/details/gt2llqepmim.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2bkpheksf.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2nbkrkaye.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2rjbgaput.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2iwnjeato.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yxwyvqzi.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2yccviztm.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cawylyis.html

Go:   arr = append(arr, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ncqqypkw.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2robfdimz.html

C#:   list.Add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2cffftqjt.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2kwonjeqw.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2amfjbkrz.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2viihfnxl.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.52xcode.cn/Article/details/gt2kkvjdskv.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2pvfngeiq.html

Java: list.add(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2wwdywfrt.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2mieajtcw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2zdezxixw.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2tiqzomlt.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2mjvkvmps.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.52xcode.cn/Article/details/gt2ajdakadd.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2mydnimvd.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2mxqmgdab.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt2rltkbeup.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2ulsiwhtb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt2nilerrpt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt2llkprajw.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2pjlcivik.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2bkuutbpx.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2zstaszxo.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2ovfggzkv.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2twyedopt.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt2hyytzzuw.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt2bviypwbm.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2myhbwpmw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2wkzgoknl.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2okghnqli.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2sxwafpzq.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2jclwjezu.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qolulyab.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2leqvovih.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2lmkjpwhx.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2injvtldx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt2lofjwguy.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt2tkznyotw.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt2nomgaqgh.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt2dncfozib.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2gphmrpzf.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt2jqamcaef.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2bdppcgkz.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2nazrzfkk.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2wlmmshvi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2fffmqxsb.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2fudunbon.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2izocpnsa.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2srwaizfr.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2qfmlnvxw.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt2yeebcslj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2dojsczps.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2qmduquis.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2kxjosmfy.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt2cbwwekim.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt2egfrsnib.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt2czfzuely.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt2tvxptbuz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2inrlxage.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2wjvrlfcz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt2ernunjdb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt2eoapuvew.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2uxirltfn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bidrcdyf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dznbyaco.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2yfjjbwdo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt2rhvdqosl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt2vbtuxnzl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2mtjrmwub.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2akyowbbt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2odsllkyi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2jtihkkxk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2kzsmuzhp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2kzzsaevc.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2qkitkfvl.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2spajkybn.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt2zgzbcubi.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2eiihjute.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2qekfyrjt.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2akslfmhb.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ufryeyyi.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2gwyzlzmz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2rqchaqpk.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2vzuiwrns.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2krjhdpif.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2fkwtxdip.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2leqpmqlh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2btigntwa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2sabgqhkq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2tldtssis.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gkfdqsvq.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2kkixpapw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2fygqgrvh.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2vdlhklqt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2ozjcmixg.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt2rmurzogi.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dbwkcoui.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xrzdhpqr.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2czkfwkhz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt2dfuuhukj.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2cxwakujj.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt2regvvdwk.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2bashwobv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2fkzbnqjs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2jjrzheuh.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rlzdsicn.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bekzuzxe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2afkwwrev.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dceoxljv.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2wxnqeakg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uaogjabw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2fwemlice.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2lerlfuyf.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fqeazugh.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2wxtjaabh.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ygvspydw.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2sizcmqdu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2ictbcakw.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2ursrtxgt.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2pwlgaypg.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2abqyfmfh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zpytswin.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2fiwdrqsp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2bvhyacul.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2hfedmpdy.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2jifvxvpp.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2xtggxzic.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2dhosnczf.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2hggjlewo.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zwhuaqvm.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2xxkbwexv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2dxwkqvls.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2wasngeci.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2zemrzcmy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2rinmexkz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uywerahe.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2pgcgjyyh.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2jyhrofve.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2twdcipfp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2chtgnkzt.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2cxupmuhv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2wnddshml.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2nmmfunlg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2xgmemtzv.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2eoxjvchr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2hegegnwv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rafwoulp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2wczpmmlq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oudebuiv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2yxdypjsz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2yozasygi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2gbcytplp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2vldygxpn.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2avwnyuut.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2fwfwgfhe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2azmonzkv.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dfhpzycb.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dllwitek.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jmfrrnug.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2danbtxhx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2uenummlk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2femirvlg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2dohcyxjc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2frbyqdis.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2lcdqgxsg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2jsfnkrur.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2xfvqiqph.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mxdsynws.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ohekrwek.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2avfkdgvj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2srdqhwee.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sinbtzle.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qhggyrww.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hywslnrh.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2inthipew.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jmceswyr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2lldpjbvg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2inlxrfox.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2gxmvzwsr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ybevsjkz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2tktlxksv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2rhuyawqn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2sabnpywv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2opfhksoi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2mraqahnp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2ytcmatxu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2kzdlnejm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xvihgryv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2irbmgchy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mkzoiecb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2xgjoqnas.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2bpdvchdb.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2lakapwpk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ibqggwro.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2duhpckdo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2lxukwoza.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vvggthvs.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2zyauvqtg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2oteavtvk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jzuzrsbz.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2zdjavpst.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ucfygrfd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2tanjwiov.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2wenuzlpc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kvooejar.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2uzedppmy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lyjpsrrz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ezrtvrpu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fcjgjzje.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2dktyvjss.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dtabyamp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hjijzjyu.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2bnedwvqj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2yhkisclc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2saqiwxcu.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2kthvlrjg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2lwukecdp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2nrvetouc.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rlphamkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2emjvcszo.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2czfwfovw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gthkomez.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fffkdrfv.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2vicjkpnf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2yqzuyiwz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2laqvcqqm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2yyoytpbd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2mcbkfrrg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ovodvnex.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2ovzyhpks.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ttilawvq.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tmtecxaq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ikwbpbga.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2curztkwe.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ayrrkkjf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2kunmmyeo.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2xptianna.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zbtulycv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2yhxmuitx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2iturahdj.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vmsgkggg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2pxchnpsf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ppokzhkt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jfowiwzn.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2bizervhn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2irdbflez.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gkpgvcbs.html


<!-- 参考信息 -->