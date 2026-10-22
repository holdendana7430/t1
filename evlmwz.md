代发 wailian999

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://www.ydjk.org.cn/Article/details/gt2mpurzmux.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2tlgjykfu.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://www.52xcode.cn/Article/details/gt2btrkoedc.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2atoevrzr.html

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt2dytavdgy.html

Go:   func add(a, b int) int
来源：http://www.52xcode.cn/Article/details/gt2tjllldpi.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.52xcode.cn/Article/details/gt2bsxnoboz.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.ydjk.org.cn/Article/details/gt2yrcjjxmw.html

[C14] 泛型函数
来源：http://www.52xcode.cn/Article/details/gt2xrvdmonc.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.ydjk.org.cn/Article/details/gt2mcagixtv.html

PHP:  // 无泛型
来源：http://www.52xcode.cn/Article/details/gt2hekajfvk.html

JS:   // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt2bgbglkex.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezsrkbsw.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgfedxxd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt2diyhigwy.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt2cvyhaocp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt2svksrczz.html

[C15] 解构 / 展开参数
来源：http://www.ydjk.org.cn/Article/details/gt2ntixqcof.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.52xcode.cn/Article/details/gt2yvhgvjwb.html

PHP:  [$a, $b] = $pair;
来源：http://www.ydjk.org.cn/Article/details/gt2vqonbjuf.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.52xcode.cn/Article/details/gt2esgtlvxv.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nocvevih.html

Java: // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt2szmglojd.html

Go:   // 无解构
来源：http://www.52xcode.cn/Article/details/gt2yirsirdi.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt2pxxraobg.html

C#:   var (a, b) = pair;
来源：http://www.52xcode.cn/Article/details/gt2xjevvnvd.html

[C16] 函数 / 方法重载
来源：http://www.52xcode.cn/Article/details/gt2ooybcpxb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt2jufzllfs.html

PHP:  // 无重载
来源：http://www.ydjk.org.cn/Article/details/gt2auohjwdo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt2gbvilmbi.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt2zaiupzru.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wihftlfi.html

Go:   // 无重载：用不同函数名
来源：http://www.ydjk.org.cn/Article/details/gt2khspgnfo.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt2nuegaara.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsyyhzwl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2anodrouv.html

D. 数组 / 列表 / 集合
来源：http://www.52xcode.cn/Article/details/gt2lhjjjdzf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zumpqbyw.html

[D01] 创建数组 / 列表
来源：http://www.52xcode.cn/Article/details/gt2kbgzgwid.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt2blgnqbyy.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt2ujconevb.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt2cjazyxmm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.52xcode.cn/Article/details/gt2fdcrvvme.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt2ruithbxd.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt2sajlhqsy.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt2gxxmhlzt.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt2hyioppyj.html

[D02] 追加元素到末尾
来源：http://www.ydjk.org.cn/Article/details/gt2xyioeftn.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt2gsnzcrtr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.52xcode.cn/Article/details/gt2pscaxeou.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt2fxcjyrpg.html

TS:   arr.push(4);
来源：http://www.52xcode.cn/Article/details/gt2opycknay.html

Java: list.add(4);
来源：http://www.ydjk.org.cn/Article/details/gt2kpbmxwax.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt2wnxjemsh.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt2gzblteez.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt2zgqorsav.html

[D03] 在指定位置插入元素
来源：http://www.52xcode.cn/Article/details/gt2qnbjjqot.html

Py:   arr.insert(0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ahugwtld.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt2qlydhqsh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt2usdgcmfw.html

TS:   arr.splice(0, 0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2bnmvwptb.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2vpaffeal.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt2mvsboepg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.52xcode.cn/Article/details/gt2gdmhdmqv.html

C#:   list.Insert(0, 0);
来源：http://www.52xcode.cn/Article/details/gt2ylhlanlq.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2yrlyamch.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lbvvotbk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nxceialt.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt2dotnxlcv.html

TS:   arr.splice(0, 1);
来源：http://www.52xcode.cn/Article/details/gt2solcearg.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.52xcode.cn/Article/details/gt2tebqqgls.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.52xcode.cn/Article/details/gt2bzkdpbls.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.52xcode.cn/Article/details/gt2kxkltzex.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.ydjk.org.cn/Article/details/gt2ordsgiyq.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt2ltszroar.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2qysejnvg.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt2zplvyzdo.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2uwqnppsy.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt2ifcpkukg.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt2zczjgitz.html

Go:   arr[0]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt2mooaoaeh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt2bqcpbqpn.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt2bguncxzy.html

[D06] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2fnbvulyf.html

Py:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kwjlrroy.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt2cbcvxxhu.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt2dusvlvrw.html

TS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt2rnqmkdam.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt2oyrsggkm.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jxqhhsuw.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2sgxomcjk.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt2vsbsydxz.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt2kxyhrcqt.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt2euvbfubl.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wyincxcw.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt2ebkokmgl.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2xbscazae.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt2akjdcuna.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt2vpcfowdh.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt2vkwvqhkf.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2pamroeqe.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt2kwascmoc.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt2fyaqxssw.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt2bhbujlpo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt2tfptimap.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt2owllvcez.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt2tuovbloo.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt2rhsedjxq.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xzaepifm.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2fdhasonn.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt2wwxdtdfb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2baxqyqqc.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt2fahfeois.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt2wxhpwxvv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt2hnbnhqcs.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt2drjltydl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gqqkiwxv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vhbxnryr.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2tcicksvm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2jqjlzjtq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wkooruda.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2fhljtqlq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2pykqjhcc.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2gcnrjjzg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt2quhgziec.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt2wvdrngts.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt2zvfyefzm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt2zfjauvay.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt2teduspzu.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2lvjoanpq.html

PHP:  array_reverse($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2sygppbrj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt2uwxidelo.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2apmsubdu.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt2vieiwzle.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2mcqqzusa.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2kjrhtptl.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2sssmnops.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt2qhxzzpbg.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2anmenopk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2tqugmxeq.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2gqmlygld.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cvogmfxe.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2ztroswvi.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wuwwyset.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdzhrffu.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt2pxhevtby.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2noiatviw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2kvrkpzan.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qbmzqyfn.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aqvsfxpu.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zyaooyaz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2sfdbmmjl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2uunuhghk.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt2lxwqgxpb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2rphuhchf.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2wccjrcfd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2txvjrmpn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2utstfnly.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cpqufkbt.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2iuoxuqge.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vcnwahey.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2tqzijjjs.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2inasbsfm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jedhfczj.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2vsowejay.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2owobqdlw.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rxmxauvu.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lylhkwir.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2cvlzvodl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2omhhyfkf.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2pwstampz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2ojdfcasc.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wgiddwca.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2umwjjvfm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2tlngqxug.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qxancvkh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2rfcszyxf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2qpetrfgd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2xdaqxouz.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2fyrmrxes.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2htgtulfa.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2jqzaxmfq.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2wazxjsem.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sjmvmjms.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2qgkavkza.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2xmavwanw.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2dpzfaqyn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2ororcsrm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2nfjnopbh.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2rhvhuqgv.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2wrsgfhrp.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2feomrxiz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2sjdagdin.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2aonycwbr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2ffaqlzuc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2ivyubxmo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2ptjtwovi.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2kyihobvq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2sdikyusw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2jqxgqdjq.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2sbdqwdxg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2gioibvje.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2zqooctpn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2pumwvhlm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2njpweplo.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2vfvnfztk.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2fwyxblaq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2dewsprjc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2tbgcnhkl.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2cavceqjg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2zygrtolf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qpspriuu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2jddnxlwp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2abawdukc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2drgxdmka.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2kjdsulpd.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2mftiksqb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2spkwzeac.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2zjteafjd.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ewruvfcr.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2lnhiqjwe.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2sxnsuieg.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2aoqmknoo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2osnbtpdh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2orgyizkd.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pmchloxu.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qyhkdqyx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2dgbgbtjj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dwkndcwb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2lzyoxovx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2tqmvdcea.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2ctogoixd.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2jjmcxtbm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2byuczssl.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2fhvdqgfj.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ufxruiox.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2btcxedhp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ioavvcfr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xyjefcxr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2icurwqtw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2rbvlomjx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2pfajgdmy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2lqxqixey.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2xzhckyrr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2asognwed.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ryudjfgu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2otzdbegw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mcsyscii.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rhtymplh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2njxudwmi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2jnmfybym.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2mdmbivvt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2nlzeruvk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2whsljwra.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2xrlcbtod.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2zuypwxva.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2lfhlxxzj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kyknosop.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2noltdqdr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2kyuucvgz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2vprdoqiq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2nsnunhvb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bwkebqma.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2iwzqelqv.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hiwjaely.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2yimjqgds.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2aeifcryo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2rmxarkcx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2vynvldfp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2asimcvbp.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2sbqpjlmj.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2zjqnpfrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owujqzdi.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2itkidbuc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aktklbmu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2owsrgpai.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2epxoimks.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xrnqhlny.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wbcoyzvf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fnyndjzg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2adydjjlo.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gwdfgjum.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2grwadghs.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tkhljosj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pectmyqb.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tyqdzgwk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2wlwctaon.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lfimaqpd.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2rxfqssti.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nsqwaibh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2ygqubxrg.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wmhniusu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2vvkmlcdd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2atayrfrg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ysswbput.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ucrnjicu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kziqzutq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yvnfbrxa.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2rpxsakac.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kztynnce.html


<!-- 参考信息 -->