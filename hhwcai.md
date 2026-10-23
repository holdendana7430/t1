代发 wailian999

PHP:  sort($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nahbiuxx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3efuwmkbp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.52xcode.cn/Article/details/gt3gzpwokhr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3ddhhfqmh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3msfqoulc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tmauatxc.html

C#:   list.Sort();
来源：http://www.ydjk.org.cn/Article/details/gt3nlsmwawu.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3xwpzdhro.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3syqvwuwj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jxyvrrzi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3lvbyjwul.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3kdwdmxgr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.52xcode.cn/Article/details/gt3zjfnxrgg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.ydjk.org.cn/Article/details/gt3hbvdaymg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3mffbzsav.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3rzdpboqf.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3lpijrdta.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3odwgconw.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3gevsgstu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3shgdrfbi.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3gvfmnhns.html

Java: Collections.reverse(list);
来源：http://www.52xcode.cn/Article/details/gt3muujarqc.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3nzqidmva.html

Ruby: arr.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ztcttded.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3xorxbqgs.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3nzulahgr.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3jcpqozve.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bwbdvlip.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3opsswhjd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jhghxbha.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3anajbbrw.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3avirohhi.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3sduertvn.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3chvfjerk.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3phawbgfw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3itrvennm.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ykcvbanf.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3eixtvmgf.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3jxhuyttx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jsskevzc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ijppboap.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3ittuiljr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3bwojvedp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3vmuxzpav.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3kfsyaogc.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ewjmgpsf.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3lruwfmqr.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3vccbkpbu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yovmuchi.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3glzklhif.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ocbnzdwc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3uaufxwxz.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3odxfsspe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ghvlsgrz.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cxksmhhz.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bjxhuoeg.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3emmoijvo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3lsguagey.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3pzhrtcvz.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3mdyhzria.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3kqfgskhm.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3uzzacpqj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3mvoamirw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mysucxjw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3ezokdmwf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dtzqmozt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3vnlzqbnr.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3qhmrknmh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3yqkdurxf.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3auecbsnw.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3enzsjtif.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3funwdxug.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3iwynkezg.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xvsoefam.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3hjdvxoin.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3lrxvcfox.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3knghxbeq.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3iujngblj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3jhysnbjn.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3setietyw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3peaamxwz.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3fctfykvh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ozwoatlc.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3vqwwtvls.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ssxrmlvc.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3moywmxey.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3magezwog.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3cncmkhol.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3scqmfmza.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3jhbtipau.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3vixmkybi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3iylblsap.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3stqxjmun.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3xfzugmvk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3etpvzpzx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3kymzqjrj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3egjdybrc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3zvuxhsyf.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xwyhkuni.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3szxgtjfz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ymidxooh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qaiphbre.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ospjfofv.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3blnxcmsu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3bokbzyzk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qratmltl.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hmlgsmnt.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3gpbnqafz.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xrbogmxz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hnlyoxos.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3xnnrjqsu.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bjwphkeb.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yejvkorl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3wvsipfho.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3ackhuybl.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3gmdnfopr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3foptvxiq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3btxrbxot.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3kdkqqjkk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3nouhddia.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3plsjqgwe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3kxfdcocf.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3locndrov.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3iccfjpsk.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3ywwokmij.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3oxalkosv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3yiskrntq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rlhnmwde.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pwohmdaf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3tpkblmpg.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3iwciqqad.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3hcuzgkiv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3affysmuk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3opebshga.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vkfvurav.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3liyuifhe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jemarico.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ydiolctc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3opufonkq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3acshbvxr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3rebyuhbk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3qkblhglj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3kyuzicbu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3ejzedblv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3rrazdekr.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3kcqnebjl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3sqrchlsg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ppljanqw.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3grzbrxql.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ivsyojga.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qzxrwasw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vmbqpopj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3djfqfpiz.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sppdogbz.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ftuaftgt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uryikpqc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3dsyrkmmz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3cvymemfe.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dswonwqd.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3mkfqtxnh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rxdbxldj.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3ovwedmgg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uemqsjdb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bcqwihvn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3qdhbldkw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gezcaubf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3jtruuoqj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3yjovcniz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3fpxfelyx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fbwgjirs.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3tpfzhsae.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ivmynetx.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zqwggcdd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kpitsagv.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jyzpigug.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3kdwrjrqr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3chcwlsic.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3cifhulja.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xsvudiql.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hoommqjn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ecruqevn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nmucbhpw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3gklelqxi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rbkdrzdt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tywbbyeo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rybzfymn.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dyeowbrh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3oxlteqml.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3zannlbeg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3wsekeszk.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3gycjlift.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jzlskpwz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3kqgspjxy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3gtojflya.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3iqebdsdl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xughqexz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3nqazzfub.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jpdsnpbj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ghuclmvy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3dxcyvhwx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3towrhibt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3eqztsmpx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mspktmrf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mlzepalx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hqioyujv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3zdkasjst.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bwwszkbx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bjcjqbii.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3clxfzvrj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wazgfeuo.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fdkommeb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gkaionml.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qeubijvd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mjiownru.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3azspnhlb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pxjvmiaq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kyitvjnr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3swwfpzeo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3awkusbty.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dpqncpoh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3iqsvsmji.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hzsjeixb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3roioatcb.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gmurnbbg.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3wjrakgli.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rpswwcfg.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ssutogxu.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3znecsshx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3cxpjrxks.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pvoiaywp.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rvupoidn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3souaihly.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3esbbyorz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nbnvoaly.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xzcwylok.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jateegoy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3rhhdtmax.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3qvwxboal.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uqyoqpbg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dgmaqsth.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3phemmpgt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3jpobvsuu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3osxhmztk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3fnzsfutc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xvmkgpap.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3byrvugnt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zgodhhux.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3cojnqdcw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mqwshygh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jxocwnjx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rrmncjja.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wmcxoimq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3tkekojkp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bldoeblb.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3zyqbrgfh.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ohwvtosh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rjsvzgsu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mrmviuij.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3icfulkaq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ibkdwlgf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3glaglrli.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yaqzvmlb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3nzvnqugu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wztcadts.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3uwbqnray.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3eexrtdcm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3qkxtckcr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3igmtyntj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3sxwfdico.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3nolyjexe.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3pmydkhqp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3mloqozvv.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3exjarfqm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3flbmhxzk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aasgwxoy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywpsdvhx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3yisdzpbq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ivelhxdu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ljeiwpba.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kikzdfdw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3mipqzrlq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3gjkrmxyc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ezyabskj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3bdjmuarf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3csiqyrjh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gdvozqcf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vvtehmis.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3wnvourzw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vsdtfbip.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3khiohrid.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3asmjckrf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3zlaeqepx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lxtymzda.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3uijulkvy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qjlcffzk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3hevytczq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3dqldusvo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tyspunvy.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3abpldbhl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3erqjvwkl.html


<!-- 参考信息 -->