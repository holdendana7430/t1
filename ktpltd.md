代发 wailian999

Java: int add(int a, int b) { return a + b; }
来源：http://www.52xcode.cn/Article/details/gt3mnfwaldc.html

Go:   func add(a, b int) int
来源：http://www.ydjk.org.cn/Article/details/gt3ixflplyb.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://www.ydjk.org.cn/Article/details/gt3pxwerlfi.html

C#:   int Add(int a, int b) => a + b;
来源：http://www.52xcode.cn/Article/details/gt3whxhvitz.html

[C14] 泛型函数
来源：http://www.ydjk.org.cn/Article/details/gt3nuvdxnul.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://www.52xcode.cn/Article/details/gt3nouwqdkm.html

PHP:  // 无泛型
来源：http://www.ydjk.org.cn/Article/details/gt3vrtzctll.html

JS:   // 无泛型
来源：http://www.52xcode.cn/Article/details/gt3eltozxtq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbbccjfz.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://www.52xcode.cn/Article/details/gt3flnhpcon.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://www.ydjk.org.cn/Article/details/gt3dayarjnl.html

Ruby: # 无泛型
来源：http://www.52xcode.cn/Article/details/gt3ywrsmvph.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://www.ydjk.org.cn/Article/details/gt3ywosdekp.html

[C15] 解构 / 展开参数
来源：http://www.52xcode.cn/Article/details/gt3vrhdhref.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://www.ydjk.org.cn/Article/details/gt3uncpzmms.html

PHP:  [$a, $b] = $pair;
来源：http://www.52xcode.cn/Article/details/gt3jdafqnga.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mbzdqvzg.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rckinnxk.html

Java: // 无解构
来源：http://www.52xcode.cn/Article/details/gt3ffcblown.html

Go:   // 无解构
来源：http://www.ydjk.org.cn/Article/details/gt3zdjaxhyj.html

Ruby: a, b = pair
来源：http://www.52xcode.cn/Article/details/gt3vpgogyxi.html

C#:   var (a, b) = pair;
来源：http://www.ydjk.org.cn/Article/details/gt3uemfzuij.html

[C16] 函数 / 方法重载
来源：http://www.ydjk.org.cn/Article/details/gt3cibvqvzk.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rfdwnulu.html

PHP:  // 无重载
来源：http://www.52xcode.cn/Article/details/gt3cfgnynki.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://www.52xcode.cn/Article/details/gt3xichudfr.html

TS:   // 用联合类型或重载签名声明
来源：http://www.52xcode.cn/Article/details/gt3isibycgb.html

Java: void f(int a) {}  void f(String a) {}
来源：http://www.52xcode.cn/Article/details/gt3buaycxaf.html

Go:   // 无重载：用不同函数名
来源：http://www.52xcode.cn/Article/details/gt3uztgunnn.html

Ruby: # 无重载：靠动态参数
来源：http://www.52xcode.cn/Article/details/gt3gwnncdqf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://www.52xcode.cn/Article/details/gt3feywfjpc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wshxczuk.html

D. 数组 / 列表 / 集合
来源：http://www.ydjk.org.cn/Article/details/gt3wgfzbjur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffrccbqd.html

[D01] 创建数组 / 列表
来源：http://www.ydjk.org.cn/Article/details/gt3nsjpcnfk.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://www.ydjk.org.cn/Article/details/gt3xldnabva.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://www.52xcode.cn/Article/details/gt3iyzuzvxf.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://www.52xcode.cn/Article/details/gt3sximjibk.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://www.ydjk.org.cn/Article/details/gt3jmlsehyn.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://www.ydjk.org.cn/Article/details/gt3fftpslfm.html

Go:   arr := []int{1, 2, 3}
来源：http://www.ydjk.org.cn/Article/details/gt3vilhihaj.html

Ruby: arr = [1, 2, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3shlsgigk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://www.52xcode.cn/Article/details/gt3ebtwxqgx.html

[D02] 追加元素到末尾
来源：http://www.52xcode.cn/Article/details/gt3lpqubxeg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://www.52xcode.cn/Article/details/gt3lmanlkcd.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3giwsqjli.html

JS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pathhiqv.html

TS:   arr.push(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qhatbone.html

Java: list.add(4);
来源：http://www.52xcode.cn/Article/details/gt3ovdgrpyi.html

Go:   arr = append(arr, 4)
来源：http://www.52xcode.cn/Article/details/gt3esoeetol.html

Ruby: arr << 4; arr.push(5)
来源：http://www.52xcode.cn/Article/details/gt3dqxiszbp.html

C#:   list.Add(4);
来源：http://www.52xcode.cn/Article/details/gt3teclqcjz.html

[D03] 在指定位置插入元素
来源：http://www.ydjk.org.cn/Article/details/gt3dxhpwldk.html

Py:   arr.insert(0, 0)
来源：http://www.52xcode.cn/Article/details/gt3evqgfptg.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://www.52xcode.cn/Article/details/gt3eopabrws.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://www.ydjk.org.cn/Article/details/gt3touvcgyk.html

TS:   arr.splice(0, 0, 0);
来源：http://www.52xcode.cn/Article/details/gt3guqkmbpa.html

Java: list.add(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zvextzzh.html

Go:   arr = append([]int{0}, arr...)
来源：http://www.52xcode.cn/Article/details/gt3ffpunzao.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://www.ydjk.org.cn/Article/details/gt3cpgqmkzs.html

C#:   list.Insert(0, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3fxobhgdj.html

[D04] 删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3isabmlwf.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://www.ydjk.org.cn/Article/details/gt3dxxcsbpw.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://www.52xcode.cn/Article/details/gt3ugnbtula.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://www.52xcode.cn/Article/details/gt3ndoyvzfn.html

TS:   arr.splice(0, 1);
来源：http://www.ydjk.org.cn/Article/details/gt3tvweedtp.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://www.ydjk.org.cn/Article/details/gt3qubfduhd.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://www.ydjk.org.cn/Article/details/gt3ssmgtjvl.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bzxrrqxa.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3utsjzzqb.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3uishanua.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3xadsrbzs.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3yhyskqsd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3tyetaeyn.html

TS:   arr[0]; arr.at(-1);
来源：http://www.52xcode.cn/Article/details/gt3vsypplaq.html

Java: list.get(0); list.set(0, 9);
来源：http://www.52xcode.cn/Article/details/gt3movvyxul.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3bitqaxmj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3wolzowpi.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xwthuksr.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3fitlezir.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3xlkidhnq.html

PHP:  count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rnktugru.html

JS:   arr.length
来源：http://www.52xcode.cn/Article/details/gt3xrjmzmkh.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3ofmamkkc.html

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3zilljjss.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rejirkao.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3tqfommyt.html

C#:   list.Count;
来源：http://www.52xcode.cn/Article/details/gt3gycmnzkw.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3meaiqqpj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3dhoymdkn.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hzpwthic.html

JS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3exyjdphb.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ryqapocn.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3jcgvbwzi.html

Go:   arr[1:4]
来源：http://www.ydjk.org.cn/Article/details/gt3vbikuonz.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3awokbbps.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3epxqasxj.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3vnyxvpcd.html

Py:   a + b;  a.extend(b)
来源：http://www.52xcode.cn/Article/details/gt3tzjhirqy.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3odgzzuwb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3xgwvkwov.html

TS:   [...a, ...b];
来源：http://www.52xcode.cn/Article/details/gt3dbpcrrqd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ftldzpgh.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3nfzgfwrn.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fktsndbv.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3siefvtlt.html

[D09] 排序（升序）
来源：http://www.52xcode.cn/Article/details/gt3pcbddsbl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ledszlka.html

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ywgutwse.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3gnnmkspg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3uueaxuna.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3xoyudzgv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3csheabog.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tbcypaof.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3ikhuprox.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt3jencwbxh.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sgzoxgbt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3azzdefmm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3nnroichv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt3irmtcyfd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3mrpuwcej.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3prynmygn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.52xcode.cn/Article/details/gt3nvlpouze.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3bpjuokuc.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3wauhtnra.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt3xbwfsyec.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3yvjkifyv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt3lwycmeie.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3pflawhrh.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3watnylpa.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tyywmfyc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3ygryltyf.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3fwqjkeof.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3ytorxjms.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3eultqnnw.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pwbppekg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3qjqgvyof.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3hqwdlruo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3gdliaycs.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eutufnqu.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3rhgcfltr.html

C#:   list.IndexOf(x);
来源：http://www.ydjk.org.cn/Article/details/gt3cpniiabr.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ypyfjqau.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3amyncgmf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dcnpejcg.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3slhwfchv.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jacunenz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt3cokkgbxl.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3zlqyzqbt.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3wbdebnlz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3yfpbpufs.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3sjqkipln.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3gutjdnee.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3jipuqjsv.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hlvbgznd.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3fkbyretb.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jrqhvnxe.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3khofhlyr.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xltxztga.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3paibxoqs.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3timgohgx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3qqkvcqoh.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3owokaofk.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3ecocxcod.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3uphxyafm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3rgnkqrob.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3udfgmksu.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3vntzjrck.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vzellqph.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3bjfgnpok.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rsbhxzoo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3qxhqsuyv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kfkcvvcd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vozkvmuq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3zomrmdzx.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3bxtlzjiy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3nrxkuagg.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3qzwyixvj.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ktcmmzsq.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3qbthcfnq.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3rhquxgqo.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3btsehorg.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dfpkbxmc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ptwhzskq.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3cdnprnwr.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3qcnpbxna.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ftgqxzxn.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3qmaummss.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3xiozvvwp.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3zlczwcmq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3gkkffnrr.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3jknlcmdj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wnxnnbju.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ctxknsqv.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3jtdvoisp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ihziacxp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tvfnipjm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zbimcfei.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3yhadtpur.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3vwnfvima.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3gkwgbqkk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3tbdiirkx.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3pcigljmb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3pgvjmtzq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3detiszer.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3khshprrr.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vjcspvxu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3wuthvdpl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3mrsswtve.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3tkuwbkjh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3jehgmzkh.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3azierflo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3gssgwalf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3mnecdiwv.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3luvnqxiz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3scbnucwt.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3kfxdrdvb.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jbhqkthk.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3usbypdrt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kaluhlsd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nndchuek.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3nrajqcwa.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xuhnmwwh.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3difqibhp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gubnzqug.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mcofrept.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fpcvygcu.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3qfyqxugb.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3fpheuxrt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3inkloyhn.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3veolcpli.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qntyidme.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3xsameklv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3plqzvfcc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3qpzalkoe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3iujufvyd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3lwrlfdrw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3wphponso.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3fwtnmbkf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3tnpleboi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3uardhndh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3thtczqti.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3rzqlpbau.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3svbdlvip.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3cerojfzd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cvvetnki.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yojsjedm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ewqqtbke.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wtirbjxj.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3fybsuiyf.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3pragcrqv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3hpfunagx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3veqrratl.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3bhmpvqwt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3tigzfzwu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ijhikiul.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3kissdngv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3zdcecari.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcturdgk.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3yzqgwwgw.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3jwbbusdb.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3sbxenkdq.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vefydtdf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ovmzsbcb.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3vipkdbkr.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3kglukfzs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3augggamv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ajpueyqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ttxtuzzv.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3nrklsbub.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkvglybj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3drbzdbxh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3cnzvkfmi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ypyqoziw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hdmpuvxe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ixbiffsd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vbgqutbi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ptzsqgib.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3kakftljz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rxjpapfo.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vrxffmrm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qunpuksn.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3nzceseca.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kobweodz.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ucxdkosh.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3juviyvwx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3oumgfbhg.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3wlkzzqgv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3leyiroqa.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rfhnxxng.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3otjklsij.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ftbqweca.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jpqzxkqx.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3frvasixs.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3turixfle.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hbayvodx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ufffagxm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vkwbulzk.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3roftwrmu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3oxdelskh.html


<!-- 参考信息 -->