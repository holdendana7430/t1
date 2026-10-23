代发 wailian999

Java: list.size();
来源：http://www.52xcode.cn/Article/details/gt3qdcixxyx.html

Go:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3japodubz.html

Ruby: arr.length; arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dvvwkzxv.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3llvwrtys.html

[D07] 切片 / 取子数组
来源：http://www.ydjk.org.cn/Article/details/gt3tnrhpixw.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.52xcode.cn/Article/details/gt3eqlojnpt.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.52xcode.cn/Article/details/gt3fkjzyagu.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3obhlbcwf.html

TS:   arr.slice(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3oscghcne.html

Java: list.subList(1, 4);
来源：http://www.ydjk.org.cn/Article/details/gt3ylijjfej.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3yaykiauo.html

Ruby: arr[1, 3]
来源：http://www.52xcode.cn/Article/details/gt3groeucan.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pnqinman.html

[D08] 合并两个数组
来源：http://www.ydjk.org.cn/Article/details/gt3iwqohemw.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rijlzspg.html

PHP:  array_merge($a, $b);
来源：http://www.ydjk.org.cn/Article/details/gt3mapuyxhi.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3mjdpwmjh.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3ifmbkgud.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3yvnjyebl.html

Go:   append(a, b...)
来源：http://www.ydjk.org.cn/Article/details/gt3wdqipyqq.html

Ruby: a + b;  a.concat(b)
来源：http://www.52xcode.cn/Article/details/gt3lheiiewo.html

C#:   a.Concat(b).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3sokinuru.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3lvckjvef.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ihszjmvq.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3jiuivzna.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.52xcode.cn/Article/details/gt3bfztkgrc.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3aivquszf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.52xcode.cn/Article/details/gt3sbokdqjg.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rbwvnscz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ljwmpdmx.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3ahpohybk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3wkmrsotv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qbeyiniw.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vlrnuexf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3pimtiyrj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3aeakszne.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3qwvvhouq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3wsgcjhne.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3beoiaius.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.ydjk.org.cn/Article/details/gt3gyeurpte.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3jnvofzkv.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3dinipkwh.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3sksrkooo.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3xhqtjvmm.html

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt3weoimaps.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lawjbwku.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3pejsrrzo.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3fcranewd.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3vkuqrzdr.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3pvgvglss.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3ohtdyxbe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dfvvmnfk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3qehyiuir.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3igsamaff.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.52xcode.cn/Article/details/gt3yzzbzehr.html

Go:   slices.Index(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3npqsehdh.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt3ijctnyfd.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3dpxaeiyx.html

[D13] 过滤（保留满足条件的）
来源：http://www.ydjk.org.cn/Article/details/gt3vlrzcyys.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3gaxvffig.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gqeqoaza.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sphleemn.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rdchzaxe.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zkpjkvjg.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3yttbsugm.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3ibiwjxeb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3yshzqhlj.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3zuszgwun.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3bvhdiybe.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3qdnhhcgr.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3ueqxqljb.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kylqnyql.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3ezqpcrkh.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3vpmyxmgq.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yinquhoi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3mcnoibra.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3jkqwgwel.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gbvpicwy.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3exnsscjm.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3slllmctd.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3fldqtyyx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3gqzseeqr.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3asluhutj.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3udlaauow.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3vwlwpxnt.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3dugakcdr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3htsqnppz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hfdzkegv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3wvtgporq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rkyxnafg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3nkfxzwzt.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3jbydepnp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3gupdboom.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3updporog.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3yfxxmlcw.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ublwltjy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vduefila.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tkvlubqs.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3aqabdelk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3qxbjftdf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jurndnyr.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3hvnepunn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3wyykngha.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3pvachgnm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nzivfaab.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3qrjkphsv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3qilbevdt.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3opcychxu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3eofvsngt.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3giwdkhfl.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3aahiifhz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3umujyvjg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3uyuqpywj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3hwwbedrp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3umqibvvp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3flzniyvx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3tkqsaeuq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3hctskfwa.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3aykzzuwc.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3nvntpuhw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3kaokwroh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zfaudviq.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3zdnkoqxx.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3mexzaiab.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3reubobur.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3otzodojz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3eqgybebd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3qyjxrtrx.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3chdmbaul.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3rjkgjaaw.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3uhczvkxw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3pyjrjdoy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3sxrrlcox.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ubichldo.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qzqguuly.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3woykkaoc.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hlwpcdmm.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ahguvgwi.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vosczttw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3krpsuwhy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vwhmpcor.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3mxsavnid.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kffecwol.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3reeedgod.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pqkqfshj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dquvqycf.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3weecegcd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ucidvimb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3widqsfko.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3clffajct.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iohkgexb.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xasqycto.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jkpzwico.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3bxqkcrxk.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3osfyueew.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3cpbyznan.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3fewviwnm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3fdzlrnir.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3ogimaxpr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3agcnqshm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mminxtoo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3izashwdx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3akmotjbl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3vpvpyxjy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3hjbzdzhx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gtitnoqh.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3uclrwxli.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3zubapvhc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3pvajggej.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xgvgelps.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3wsckvjop.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3vdwwtzwj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3aucxbkkh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jzikftuv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3olxgaoim.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3doejapni.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3vcsmgbfj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mskkpamz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zsfwwqfd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3yogjjiue.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3jmjcydqt.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3igpgvxwm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ruoiwwlb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gpycejky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cidhmdtf.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3keqfpswu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hogmvsiu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ggzudult.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3alrplnsp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cphtagxi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cafpmecf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vfhxxagy.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3iotrajuj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wqnmlxst.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3bfogggwk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tdkhqhct.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3qgntfzju.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ojlffxhr.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3zllbdzbx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3pidmsyti.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yyowbbrh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3msylgyso.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3sxuaifdp.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3mrtvmzqi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3giqghoxt.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3josqyihs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bfgsawao.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3blzjtgsw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wxbdmthl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ngydijio.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3yjknpudl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vmfvpoqr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3areeeqvw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3asqrmvbu.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3tkzactks.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ozzjzwys.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3pjsvpmos.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3gbwujwhx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3stwnjmss.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mzesivua.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3psagcprb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wxhtjxdx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gujavirz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3fulvchvj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3crramdkw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3qeodyaep.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zwgdxeyy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3bxsniura.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3egusmtfd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3hncetjgp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ssqklvbe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vkwbtofm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3idbqznnj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgyruqck.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kkdaowfh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3swwlcaax.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lwhccvbj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ccgwbkus.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pmpkdctw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uqaugilm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ddjktjuz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3utlmsauk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3ekhiecjv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3knvljfyy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3momwrfxe.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3eavyzxnb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3pniybupj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3bxyvazhp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3boozlkwj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3pynpgzav.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3bqkbinew.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3loglfqau.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3huyxcvos.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cdwfussh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fagqkepz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3szelvprf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3kbmxzrzb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gsuzpsol.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vricrufv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ttgcdigk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3oqgpvapz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3frelecct.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3futfxrml.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bgacjwei.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3jtxppatd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ytgxeetg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vodzxxej.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lxqmaevr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3otwxhgrd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pxkvyjzn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hmhejbvq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aknxklyu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3thjrukdx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jzuqwwox.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3smmtqfiy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wmdomdqm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3bkmtmjfj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3nlzovdvr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3gwyweeiy.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bviwpbeg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ovydtdvz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xrdppleu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3srvyhdft.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hjuboyto.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yjrmfdzq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tpygdolr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3efpezndi.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ryzmtgmz.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wkeedphe.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ntikyxzw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tsnklmxo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3rxosyhmt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3seyrormq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3sqomkvhf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ezfgcngu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3xrqfdekg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3llvfsbmo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3obzwzona.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pixnwtvp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vjwdjtnp.html


<!-- 参考信息 -->