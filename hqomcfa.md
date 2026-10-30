代发 wailian999

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gmtucrgmu.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://baike.zdbjq.cn/Article/details/gsfsfvfyp.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://mobile.fehbvm.com/Article/details/gedthtfop.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.hesvh.cn/Article/details/gdfmgqdmm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkjgglxe.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gddwmxauj.sHtML

C#:   list.Sort();
来源：http://m.share.zdbjq.cn/Article/details/gfbjmdeqc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.fehbvm.com/Article/details/glpkyhrjb.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gkytemgdk.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.fehbvm.com/Article/details/gucbytism.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gqhbyrlxp.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/gzudhvzfe.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gjruewlsw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://wap.hesvh.cn/Article/details/garrtahsk.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gesmnwdvt.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gioroecmo.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gdljobyxi.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gzyezegfe.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.zdbjq.cn/Article/details/gjjbktcux.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.hesvh.cn/Article/details/gslqhpgqg.sHtML

TS:   [...arr].reverse();
来源：http://www.share.hesvh.cn/Article/details/gixtxgbdd.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gtquidnxc.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.zdbjq.cn/Article/details/gaxngwkgd.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/ghectvydv.sHtML

C#:   list.Reverse();
来源：http://www.share.fehbvm.com/Article/details/grtirtjem.sHtML

[D12] 查找元素下标
来源：http://mobile.fehbvm.com/Article/details/ghguhucvz.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.hesvh.cn/Article/details/gpawzkmrc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.hesvh.cn/Article/details/gsqpzveyx.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.fehbvm.com/Article/details/gusonwsnh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gzauhcchr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.hesvh.cn/Article/details/gfiejazmc.sHtML

Go:   slices.Index(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gbldpbnyo.sHtML

Ruby: arr.index(x)
来源：http://www.blog.zdbjq.cn/Article/details/gkxdypres.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gisnowtnb.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.zdbjq.cn/Article/details/gxfnvwwbk.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/ggtpscfyy.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.m.share.hesvh.cn/Article/details/ghpufmskd.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gbhcqtcsr.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/ghlkwbhvf.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.hesvh.cn/Article/details/gixfmwcsy.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/geemyvbdj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gkhyqijuy.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://read.share.hesvh.cn/Article/details/ggjbapzhf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.fehbvm.com/Article/details/gkuzewznp.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/gmbrawuvp.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gzjigzlog.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.zdbjq.cn/Article/details/gzipoftns.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gpwkcrzww.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gvqffgajz.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gppkjryzs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.fehbvm.com/Article/details/gvxlqnqth.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.fehbvm.com/Article/details/gbwxieotz.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gaeymoyop.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gnaplogsm.sHtML

PHP:  array_unique($arr);
来源：http://baike.zdbjq.cn/Article/details/giiiareqy.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/ghjcsauvd.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gmnwlundt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gvxwftiqx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://blog.zdbjq.cn/Article/details/gitvylern.sHtML

Ruby: arr.uniq
来源：http://www.m.share.hesvh.cn/Article/details/gjtlcgnxt.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gqlhoohdj.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gckvywbda.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/gjuslgraa.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/glknsqgyh.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.zdbjq.cn/Article/details/gakkmjxnx.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/ghptrgafj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.zdbjq.cn/Article/details/gpcnulyet.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gewipfoad.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gxbvzqlvv.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gfkexaxcm.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gybybclvi.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gulhvsoda.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/ggryxwnjz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/gvpqoqmgk.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gwaeaaecq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gvqjgdiap.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/ggroewynf.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/gwfdtimfd.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.hesvh.cn/Article/details/gnsehgips.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.zdbjq.cn/Article/details/gnqerilcj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gbhpsudfi.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gmqgkoaji.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.hesvh.cn/Article/details/gnzqejkjn.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gejdsvrhd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gbufsqvcm.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/grwzwjqcn.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gsuivkutd.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gtutfpsij.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gkyykzkgd.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gcsairqlk.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fehbvm.com/Article/details/gunnmhdcd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.fehbvm.com/Article/details/gtmrgbiqm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.fehbvm.com/Article/details/grpetlznf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gppqdzrhl.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gmjdjkebr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.hesvh.cn/Article/details/gldkvceem.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gfevhxltc.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gktumfwqu.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gtumtthrc.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gggpzjpmg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gbnmoyhrb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gseqazgii.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/gboqjrchr.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gaglzygtw.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/grnmvcqnj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gmwrngnib.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gpfeuqugj.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/ghyuidbnb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gximqrqix.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gmnyxqhfh.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/glvkqwfka.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gcncymaeh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gyjnomemr.sHtML

Ruby: arr.include?(x)
来源：http://www.share.zdbjq.cn/Article/details/gmyusnzqk.sHtML

C#:   list.Contains(x)
来源：http://wap.fehbvm.com/Article/details/gbvhqvumw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gfjnrvclh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.hesvh.cn/Article/details/gcuppsybi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/grukremva.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gtnjblxkt.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gyoejmndj.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gwaflbcnm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gwxkhrkec.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/glstmuqoy.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gueazkcdz.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/ggcuroiaq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/ghosduvcg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gnywmzzke.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/grgyddwef.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gwykcuqiw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gocxcxfmg.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gckckixrm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gibnvhzje.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gkmvdbbix.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gzfkbpxej.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/girxlbdam.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gxwstrqea.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gnjjcdzqo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gngzwfnsw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gqrrqhsaj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/gxtjxkcrx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gnvezmwbw.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.zdbjq.cn/Article/details/gharmibpe.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.zdbjq.cn/Article/details/grpkgopvf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gmrivkumb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fehbvm.com/Article/details/giznwmzol.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gsgmrlwhg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gdbocddxq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gcbvnzwnc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gkbskdosw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gepovzrpp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/glcepsbns.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gyatjfrsm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/guktakams.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gbekxjamh.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gmhxqnosi.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gbfyyixtq.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gharvachq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gvundptcu.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gavcavdkk.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gmjvcajao.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gavwcwjbb.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gjlpffjyp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gvtvqhzbt.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gtzxrsnph.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.fehbvm.com/Article/details/gcxvhtewt.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gdzgpmcbj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gagvvgfww.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gqhucyjvx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/godjokgfs.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gkpahiald.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gatimnhyi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gqbkkpggx.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gqtavprbf.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gldnvgeag.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/gvqqvmpwc.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gglsndagy.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/ghehqvkyk.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gwwanvcrd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gcpnhdvmu.sHtML

Ruby: "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gvlnomauv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gdysdblvs.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/godvkowmn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gjgqklaoy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gvmireaxz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gztmafugv.sHtML

TS:   s.slice(1, 4)
来源：http://3g.hesvh.cn/Article/details/gkiatpcgc.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gnmdauogn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gxsjqhjcu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/grsfigecu.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/ghvaqgddy.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gtyypmryt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gtahuzwcc.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/govdavewx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gxlmarlym.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gddvndpns.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gtegchyvk.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/ghjsjlbxl.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/grklbsuvj.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gogwzsrtv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gqiflraij.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/grxhvyeop.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gflfxvqry.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gvrlvghgl.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gsljqrufp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gmchmgxkb.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/gcnuqglxa.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/geifimmwj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gsdoxvced.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gtdwxfnoq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gciptyvbq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gdotuyjfo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/guvjgsueb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gsbalwdnd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gsiyamuoj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.zdbjq.cn/Article/details/gzvsyjrwh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gzeiuukjz.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/ghakwsnoi.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/gnargtqbl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gpeavajhc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/ghuujmhte.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gwcerxohi.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/geubwqzhn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/gmennvmnt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/glmtccduk.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gprolazvd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/glkexbouv.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/gupagfkbw.sHtML

Py:   ",".join(items)
来源：http://wap.fehbvm.com/Article/details/gbdbtqszc.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gosewbghr.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/galxdbhcv.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/grviihbzj.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gkptbjujy.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gtdchxrcq.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gjrcobitj.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gyssckxfz.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gbqhvbcwt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gwpjpxnmn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/giktwoais.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/glqkdzdpo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gksscvxnp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gexnuapni.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gznoejrky.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gmmemjjkc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gbdsycvan.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gpswioplf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gwypqxhpa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gdeoxlewk.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gitwgjcpy.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gaxqwjsjo.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gwugmpkpz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gubziuboi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gbdqxspkz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/ghxugyxdj.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gbodevxkl.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/guunpyljg.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gnibvxmgd.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/geoxfbekn.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gechtydko.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/grqgceliy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gsjziuyhz.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gtgtjvioh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/glbwlllcd.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gdufkpblv.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/grktjgkwn.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gnutucrvn.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/grcowgjvs.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gotfkffkk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/grhxjwdaj.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gfjzdalqi.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gbvnauoym.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/glrcoslol.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gteqfpnfn.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gannxajtv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gjqiwlgmy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gllczwxxd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gqdwvquzu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gopooxxvs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gqdzphkjn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gaxzsrqhx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gvbengrdw.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gqxiqnhmp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gfkmdcppo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtxdaejnr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.hesvh.cn/Article/details/gikxwhphi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpkioyjlb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gzfbydxpb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.hesvh.cn/Article/details/gowctnsrc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/giopuqrih.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gayzzbelb.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gtrohvzdj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gnsqcajsn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/ggtcxjalh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gafxkbzvc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gxwshwkbj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gnjefzqmc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gabajywln.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gcqnshwet.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gpirhjdwh.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/grgxflksu.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gamrchlex.sHtML


<!-- 参考信息 -->