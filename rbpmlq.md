代发 wailian999

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2bjsxtrfy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mxxyldkq.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt2emhravnd.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.ydjk.org.cn/Article/details/gt2pwnbmqdo.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vyuxudzw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt2qauouyzg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.ydjk.org.cn/Article/details/gt2zeclztvi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt2qsdtkrvs.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt2hnfayklr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt2bolormhd.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt2smvsavtm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt2owigtxyp.html

[D11] 反转数组
来源：http://www.ydjk.org.cn/Article/details/gt2clfghiwz.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.ydjk.org.cn/Article/details/gt2brjfhqol.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt2jcwggozg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.52xcode.cn/Article/details/gt2walvngbf.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2tkksgmzd.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kaaaaxgr.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt2suaekqax.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qcoxvwzb.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt2tlphjhdl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2rvmylgff.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt2kgmqapjy.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.52xcode.cn/Article/details/gt2kduvpdhm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2kljnmemv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt2ftkphaqw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt2pezjetql.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mqwzihgs.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt2iggalljw.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2tmrskdkm.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt2oiaxctrp.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2uqpyjawo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fmdrwurr.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2cfnggnfy.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt2dvhlbzwc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xcixlkzf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2bffxgipu.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2obvskfsp.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2mesinojd.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2aypnship.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2uemmriin.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ibxdzpgy.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2dorpjyff.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2zwqtpabz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2owvmibgi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2ayzndvjn.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oibyckaq.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2adgvgjdy.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2nddzpgdt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2rbazqgzn.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2npeesvev.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2lewooklx.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2moojqvtm.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2odndecsi.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2lflmzllt.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2snrynaxb.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2vymlkcad.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2jgioxbbl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gllufqin.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2ettyciif.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dtkgudtx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2trtsoyrd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2yeznqyan.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2qspuuxyh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2favswwsm.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2backfamk.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2nkjzszpx.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ctborhge.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2zjanwytg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vrrkopcq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2kfspuaxy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2wjiehdjl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2sraljuyq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2asoljncw.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2yovzmmrb.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ewnlhwow.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2yflgebof.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2gpjohgdt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ylovftey.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2salwajvu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fwwqxtre.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2gwxbxspe.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2yesowtkn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uhryakfo.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2hgcgqupn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fpvkigbn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ujltiynd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2leinrsxg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2pcstryxu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2lbsbkizk.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2nfrgudya.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2rpappqww.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ncowzudg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2mudgkhjh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2gpfielgn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2qlewbjlw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2njnrdufn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2azsjeoqx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2nuaddfib.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2cwxuocff.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2jmqpzect.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2mhtxfgxv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2vtdglttu.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ewvglkmh.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2cdnzajmn.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ybcbyclj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yndxvqma.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ucllacqg.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tsxjqnsn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfammypi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bngojnqg.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2foemgjgr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zjycpkyj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2lnfmwynh.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jbzxwnbr.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2omtmssjx.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2uugnpvgt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kdsmimxo.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2junboefx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2grdxugmw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ebeknebz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2aglkkagp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2uprgjkom.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2sywquzll.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2onqpessl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2xuqchzor.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mdswoqik.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2owxvauyd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2nnzyrywh.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2ebtrpvmo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2zrmiwtpv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2juvhjszp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2hsckijxx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zrswyyfb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2thqlvsjy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2unkjzxwz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2qtwwzjca.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2yagziseq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2ywbswiit.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2hbxsuakh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2gyvjuzjo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bimddgxj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2yddgocad.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2amafhmiy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2qdpznpyv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mlafybmk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nrnqapyn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kvoiimaz.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hngjoxty.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2iillluof.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2jbvqcaen.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kbqtnhhm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2xbxlfrcg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ydvxfkzv.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vlzvfvpu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2msrwhbns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2scbqbtvx.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2llytgbue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2awefcuat.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sdbtupif.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2tntrtilb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2bducupaa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2lkcxsxdw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qkgbmguv.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2xmisiuad.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2qlnhjlnc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2dxlnqcvl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zsxpfpuu.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2mflobqei.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vzvxkkxo.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2xtyrgfsg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qllzsmpf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2vacsrbxw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2uevoslcq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2fummnolj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2mxisogrr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2yjqjqhyi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nsggfxqv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2bssabcdt.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sulsmfum.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dhplshbm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dftpinsd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2yngvcwqg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ljelxvkw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2jdjbzhkm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2xiycbsqj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2torjlock.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hvwpgyev.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2rdmmzdue.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2myzloauh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nywuxfgc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iigwuqkt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ocyrqpta.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cveojwhh.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zvayoopb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2oawrlhik.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nzvthunv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ydqkphvt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bkcbmfos.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2kvuulmer.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2puqvfqhg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ffofpvms.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2qwlnrfqe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2btvhfsqf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hhchjzat.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2odenyrfx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rzopkujr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qrqjrdbd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rrbitmhg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sklnfqhf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vonrfuoy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ddfklcga.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ivjoerfm.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2accymjxg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2nzjfpcan.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2virzmvkh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zmegqwvt.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2eiboovuk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2xiamurla.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mdvqujng.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2xjbgcnmg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2akhqrfux.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2culktxqm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2hdhqmfby.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2fimxdelz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hrcxldcp.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pcqfaett.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2pnuwfhbt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2udwrmeiy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2enwecybw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2diejwtpl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2jvifeatb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2phyxdign.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2phceeuqv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ghzgfiiw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vedloldo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fkdwdcin.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2nyzjbltz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2uzxvssdm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rzrbaqkn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2nbeooqme.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hulhqtma.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2jpyckleg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fygbmwhs.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2foeubofe.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2abfthkts.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bcjuxkvb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xjycnzkd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2mlrwifnl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2swsertci.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xodmqkxq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2chzloapo.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jmmwkvbo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rnuuietc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2izoaqoio.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gxxqtfae.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dahenkhs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2idxzpkxb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2itojgrzi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jfwnzqac.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pjxyenbh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cqmakvey.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nhmsmmzj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qxsrzknf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2hdbiletx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cbyysocn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2tqospqgi.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gltiqwao.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2irtwpimu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2sgniaxkc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cuacwbrf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2czqulxdc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dnqwnhig.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kkxwvuyo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2wuhogvfh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfvewyoh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ewwmvpmh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ncgoyemp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2pugdtfre.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2csnmvarl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vpgjdgmr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2afzgdxyp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2xeluegmy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ginfozgy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2shesbayp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jtdeyyvt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2guepljut.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wqbbinjp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ifvrtnnz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ehceismq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2obiezaae.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sytixdva.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2uljcgcbe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ycwaglhz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2raquvzsj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2sofaaznx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2fjoenuav.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ztfcmeki.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2samhmqjx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2cjrpjfep.html


<!-- 参考信息 -->