代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jrqjeztp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://www.52xcode.cn/Article/details/gt3bsiyngbs.html

[D05] 访问与修改元素
来源：http://www.52xcode.cn/Article/details/gt3mdacadnl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3khmjmxhq.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://www.52xcode.cn/Article/details/gt3nmgnxhqb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3xplyhssu.html

TS:   arr[0]; arr.at(-1);
来源：http://www.ydjk.org.cn/Article/details/gt3vtcfrweb.html

Java: list.get(0); list.set(0, 9);
来源：http://www.ydjk.org.cn/Article/details/gt3cfiwlptl.html

Go:   arr[0]; arr[0] = 9
来源：http://www.ydjk.org.cn/Article/details/gt3igftwywc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://www.52xcode.cn/Article/details/gt3spnxcsva.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://www.ydjk.org.cn/Article/details/gt3ofiihxju.html

[D06] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hertddxg.html

Py:   len(arr)
来源：http://www.52xcode.cn/Article/details/gt3sfgjmflw.html

PHP:  count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cfueadop.html

JS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3jlgpfivd.html

TS:   arr.length
来源：http://www.ydjk.org.cn/Article/details/gt3gmkjfmto.html

Java: list.size();
来源：http://www.ydjk.org.cn/Article/details/gt3oezkbrhd.html

Go:   len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dskxqdvc.html

Ruby: arr.length; arr.size
来源：http://www.52xcode.cn/Article/details/gt3fjcudzry.html

C#:   list.Count;
来源：http://www.ydjk.org.cn/Article/details/gt3fxkihunc.html

[D07] 切片 / 取子数组
来源：http://www.52xcode.cn/Article/details/gt3nluizdqd.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.ydjk.org.cn/Article/details/gt3bictnrag.html

PHP:  array_slice($arr, 1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ehhavxok.html

JS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3mmzblmtu.html

TS:   arr.slice(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ripdwvst.html

Java: list.subList(1, 4);
来源：http://www.52xcode.cn/Article/details/gt3ksrtdrim.html

Go:   arr[1:4]
来源：http://www.52xcode.cn/Article/details/gt3qyzgvzmp.html

Ruby: arr[1, 3]
来源：http://www.ydjk.org.cn/Article/details/gt3vbrwqmsy.html

C#:   list.GetRange(1, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3khfofuww.html

[D08] 合并两个数组
来源：http://www.52xcode.cn/Article/details/gt3idlqzmdr.html

Py:   a + b;  a.extend(b)
来源：http://www.ydjk.org.cn/Article/details/gt3wqkczeil.html

PHP:  array_merge($a, $b);
来源：http://www.52xcode.cn/Article/details/gt3hzzlzjfx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://www.52xcode.cn/Article/details/gt3psaapiea.html

TS:   [...a, ...b];
来源：http://www.ydjk.org.cn/Article/details/gt3gnknroby.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://www.52xcode.cn/Article/details/gt3rlrqwymg.html

Go:   append(a, b...)
来源：http://www.52xcode.cn/Article/details/gt3nunrvitd.html

Ruby: a + b;  a.concat(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bbividgv.html

C#:   a.Concat(b).ToList()
来源：http://www.52xcode.cn/Article/details/gt3znvqcetp.html

[D09] 排序（升序）
来源：http://www.ydjk.org.cn/Article/details/gt3qjxwqnvr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cfdzmnni.html

PHP:  sort($arr);
来源：http://www.52xcode.cn/Article/details/gt3bdcdzwoq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.ydjk.org.cn/Article/details/gt3fdcfyovy.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.ydjk.org.cn/Article/details/gt3eubmzvmt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://www.ydjk.org.cn/Article/details/gt3nabssohe.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ngtdudyp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3vgnsxxkn.html

C#:   list.Sort();
来源：http://www.52xcode.cn/Article/details/gt3wllgovrr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.52xcode.cn/Article/details/gt3szyuupvz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.52xcode.cn/Article/details/gt3nuhrmlct.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.52xcode.cn/Article/details/gt3jqkkndoq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3ixkuexpg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.52xcode.cn/Article/details/gt3exozkwem.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.ydjk.org.cn/Article/details/gt3zxhrjvwa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.52xcode.cn/Article/details/gt3uwryditr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.ydjk.org.cn/Article/details/gt3ixngyrnh.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.52xcode.cn/Article/details/gt3bkeowkzv.html

[D11] 反转数组
来源：http://www.52xcode.cn/Article/details/gt3kglzyrem.html

Py:   arr[::-1];  arr.reverse()
来源：http://www.52xcode.cn/Article/details/gt3piebpwvg.html

PHP:  array_reverse($arr);
来源：http://www.52xcode.cn/Article/details/gt3jhtyipst.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.ydjk.org.cn/Article/details/gt3uddkdoxs.html

TS:   [...arr].reverse();
来源：http://www.ydjk.org.cn/Article/details/gt3tfuuqpxg.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt3eyxlugcv.html

Go:   slices.Reverse(arr)
来源：http://www.52xcode.cn/Article/details/gt3ywzcsibc.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt3wvgfjgaw.html

C#:   list.Reverse();
来源：http://www.52xcode.cn/Article/details/gt3qeqdvtwo.html

[D12] 查找元素下标
来源：http://www.ydjk.org.cn/Article/details/gt3tnjveego.html

Py:   arr.index(x);  x in arr
来源：http://www.52xcode.cn/Article/details/gt3tfjpdyef.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pzvyqwrz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.52xcode.cn/Article/details/gt3svaamwkt.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mnoimrsk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt3lhrdtcqx.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yvjeuxje.html

Ruby: arr.index(x)
来源：http://www.ydjk.org.cn/Article/details/gt3bzgsdkka.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt3cogojsbl.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt3ennfqxvv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt3ihjdsqca.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt3agguptdu.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3flpquzqs.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ekmqzexp.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pcrtjpdb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3vllryibs.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3fhpcxvmd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3zcdmfecu.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3pjzejkag.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3bljulmnu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xwmmrcxe.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3voxgfdnl.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ykogltll.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ugbrmyyo.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ulltgqru.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3roygprqr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3bsfihmfk.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rmuluvkv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3gghojhvj.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3yehmeeet.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3beyurrge.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3qtdwsyyp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3atrodlsz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3tnzmeyws.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3jrzwcurh.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3phuhiyak.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3opgplwyb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3auktrvnz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ltqnvibe.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3kbcbzykm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rdwoptys.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3fggpwrkt.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3cubxsyoz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3eevpdmur.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3gmeodxde.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mlsahfol.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fkdsxlmi.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tilsydkv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qkhambpb.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ezrxblqj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3bepqwcad.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gxpedhjf.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3mhrmsaze.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3zdeicvbm.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3yvqfmbst.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3fimelqtb.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3vnrubwqb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3flbeiumd.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3frgwbzhj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dndpocoe.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jbwixkrs.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3mastrqid.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3rbavgddh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3jljrsmzb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uksorgag.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3hikzmtof.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3jjqpadkt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3pygqgifh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3frqmywed.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3jtwhavfw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3wwfwamzh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3hwzbxhvi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jpqdtqws.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3gtvejvby.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3mtolyfsa.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pzzwzebt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3aqucpmsb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3utjtwpgr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3dcrmhpfc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3opoqvesv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3dyynnlbu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3fbqedsfh.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3bgrdnjpv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3biuzwjwg.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ultdhxjh.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3apujpxbj.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3thluigmr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uxoglifg.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lseodwyw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uowaortw.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3oqyfzhny.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3doypletn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3epcwnsbc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bbrfwrxn.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3gwhdfcgx.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3qxnlhpmc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3facpxayj.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ldcsdwnv.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ayhvtspo.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3dxdxemiv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3pohggxnw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3gbqpodmg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3ucfwcxrc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3awrlldbw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3xroerenm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3znnrpmln.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3mjywiwxl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3dmapzdxs.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3aqqioigz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3vhcyqchf.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3gkqinpew.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3qgyzrkrx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3skuwkgfw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3bjkcnbqp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3dzrkyshz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3buvrtzsn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3succeeco.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3vivjdbnd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3elxdfsil.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hamgkdvy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3edyozxvn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3izovkkpf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xcdbeohj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3tsrfnxrs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jwewtele.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hpmlyltx.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jojatsmx.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3uiyiwunk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tpkwssjh.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gpchwbtt.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3bdeetjsf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qoyfeefr.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3nytehitw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mrqsbtjx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wagrvrpo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3esgyqjpl.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ezionyji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gicyxerj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hagsloqq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3afqqalun.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cwponwid.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ovyyyuqx.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3doxjswzu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3zenkahfw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wedfamhv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3fwidsztc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3biistwvw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3anboibwi.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ggdotrap.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cfvyjbzg.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sljofbsx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3golrodmv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fluihavh.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3alyymeyb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3dzbeziaf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3sphctvqb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qjumnjre.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3hmrsxiob.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gdgplrpa.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tniandey.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3awgimebk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hnxgomov.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3zshyrfac.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3zldwfved.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mepfqpfv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3jlinhzfd.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3crmlpuut.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3jqsqwono.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3nmjqatyy.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qtopooka.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uuvjobqe.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3nspmrfge.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3auyaifsg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ncjrhaff.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3jmsgvxom.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ucnhxaci.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ufaqrcyz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vlihreib.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mgytvgvl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3seziwllt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3kxduyjls.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3nsjqhfrt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3scqigtdl.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3brbvzblf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lnpxioiq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vzsohnhh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yusgqwzn.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uokxrral.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zecnmqyo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lomfmtsz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lsvjvyiq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3sohqtivn.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nqiyrmtv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3shpopmyq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qpikcjus.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3gpjpdyrj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mngttajv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3fxgtxvpq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3emlfkexv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3dnzdtbwg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ujrzqxlu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ysxauwcs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3stxcswot.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3cabkgyty.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mrqpjzwo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bqeqlbjv.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3onvjcjsm.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3qspmxpwe.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gzbvfmuz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3osqljfii.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3abfgvyxq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ihsbtuwc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vwsaecll.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3pwrtejha.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qeznkkzn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3qhsfxawi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3oxyobarh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zsppnmuo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3niqychoc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qslcsrij.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dnjmfwbj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hfrgfpzu.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3utndshqt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nbzpebwz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ojqwffll.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ukhwkwux.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rklcylxe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3wyveofdo.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kiexlbuz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kbbxtiyf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pelrmrdh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3speoqasy.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ayzrgihj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3aupbxnqo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qxptoicz.html


<!-- 参考信息 -->