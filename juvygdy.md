代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://3g.fehbvm.com/Article/details/gdsgrhkxb.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gninxzdex.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.fehbvm.com/Article/details/gthxpkuua.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gmmqoyryc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/giccwryya.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gtvqdhucm.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://baike.hesvh.cn/Article/details/gbqjrvrwq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://m.share.zdbjq.cn/Article/details/gibvwazac.sHtML

[D11] 反转数组
来源：http://baike.hesvh.cn/Article/details/gbqullore.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/gkrnyiads.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gtrdlrrwd.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gmrplqqfh.sHtML

TS:   [...arr].reverse();
来源：http://m.share.hesvh.cn/Article/details/gwlwqxwnh.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gsnjxbesj.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/gfndmrkmt.sHtML

Ruby: arr.reverse
来源：http://read.share.zdbjq.cn/Article/details/gnyxyntof.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/ggldcqyvm.sHtML

[D12] 查找元素下标
来源：http://baike.fehbvm.com/Article/details/gikczgjih.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.hesvh.cn/Article/details/gtbbaavps.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/grghejsuw.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/giwrzronm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gsbwnnwoy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/gobogospf.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gyakvdoxa.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gvtqyvhgf.sHtML

C#:   list.IndexOf(x);
来源：http://mobile.fehbvm.com/Article/details/gemfjekgs.sHtML

[D13] 过滤（保留满足条件的）
来源：http://wap.hesvh.cn/Article/details/gfulvyqps.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://read.share.fehbvm.com/Article/details/gpbrtcaib.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.fehbvm.com/Article/details/gzivoqbwc.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmlmaktl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/grasjmupp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.fehbvm.com/Article/details/guoeuxban.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.share.zdbjq.cn/Article/details/gytxwjprc.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/ggqsanauf.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gdgiczbia.sHtML

[D14] 映射转换（每个元素变形）
来源：http://3g.fehbvm.com/Article/details/gyhsbseib.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gorzjyiuf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.hesvh.cn/Article/details/gsptkbsia.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gseidmjhd.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gzolctjwq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gavkscapc.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gtxsvkgre.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gugzrdthh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.hesvh.cn/Article/details/ginoneluy.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gmcircmhv.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.blog.hesvh.cn/Article/details/gkfesgice.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gwgcynmlw.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gwbovqsem.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gklxzpmvm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/ghiwvusax.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/grzdrltll.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/ghmibzkrx.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gsubsvlvb.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/giswundgk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.fehbvm.com/Article/details/gbaviogkl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://mobile.fehbvm.com/Article/details/gxjptepkl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gpgbrvqtz.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gyqgykhxo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gqfsjghfi.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/ghxalnuhx.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/grozfxvva.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gfsarivik.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gtsqccfgu.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gutghivjf.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gopcitphb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.hesvh.cn/Article/details/goeyjpwwe.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gmfldenzw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gtivodhgz.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.zdbjq.cn/Article/details/ghdbjhqfx.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gajpdavjo.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gnyoscfkj.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gcsejmgmq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.zdbjq.cn/Article/details/gpzgnaoix.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gnayafdhc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gdxfqttmb.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gxnrgpswd.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gvupewjsn.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gvkwexhwe.sHtML

Ruby: nested.flatten
来源：http://www.m.share.fehbvm.com/Article/details/grpxcvdng.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gtgjmpoad.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/goedjhqck.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/gjzhbwnst.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gbjdtrvxd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gduymvese.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gzkzkugdz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/ghhkprjjp.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/goatzsqpa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gtgfgrqcn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gqxxlsjxz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gnoqwrgzm.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnyngjaql.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gvyifasej.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gdvapvnid.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gdzctzhkf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/goxgmkvia.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.fehbvm.com/Article/details/glhtalxgp.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/ghojpzina.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gkfvemsdd.sHtML

[D21] 判断是否包含某元素
来源：http://www.blog.fehbvm.com/Article/details/gafjdtvma.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gizyjfiun.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gpzrqgwll.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/guwwuztwj.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmxocloau.sHtML

Java: list.contains(x)
来源：http://3g.hesvh.cn/Article/details/gwufemsea.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gvxarotpk.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/glyyznwrz.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gmxjavrug.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.zdbjq.cn/Article/details/gzenxypaj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/gkvkrgzxi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.hesvh.cn/Article/details/gycymojvf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gcofismtw.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/gjdszkoox.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gemzogzdo.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gdqsrltfc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/gnujedemv.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/gzmvmphau.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gnsaataev.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gvbtpvyei.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gixbjtywg.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gsicsqdrp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gvrnaeqyw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gavfkbngr.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/ggcfxokae.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gnhbqbhht.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.hesvh.cn/Article/details/gbgtelfqs.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gnxamzpfg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/gyxbvtfes.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gnrusdhvj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gjgbokjof.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gtjqkiilu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gtxavebni.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gtquwdtwh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gqnocgdcp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gyxvamfqf.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.hesvh.cn/Article/details/glamkicqc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gyxpjqxaw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/gebczfyit.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.fehbvm.com/Article/details/gojvrifgn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.hesvh.cn/Article/details/ghabjcjjw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.hesvh.cn/Article/details/grbosbefa.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gpmvgkehq.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggfkwfazp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gdedxskud.sHtML

[D26] 数组转字符串
来源：http://baike.zdbjq.cn/Article/details/gdftjuqva.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/gmdeirgqq.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gruyuitid.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/ggefvymea.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gmumlnjvb.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gmsosbejm.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/guxssjear.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gmmwcffyr.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/grqapzkii.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzbjhmefc.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/ggzndupif.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grlelenwl.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gvebzrwix.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.zdbjq.cn/Article/details/gdvntkbio.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gompnhfat.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gcfutznfs.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gjbyietra.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fehbvm.com/Article/details/glrtdlmoi.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gqaxefifd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/ghlxpdsrj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gidfaywbs.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gdstsnkom.sHtML

Py:   "ab" * 3
来源：http://baike.fehbvm.com/Article/details/ghugbvswu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/gkixdxlti.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gtufnjeht.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gzletvmfq.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gjvzzgcvq.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gwwfabnhv.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gmkokcvcw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gseqnwkit.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gpxbtdweu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gsoiufmui.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gttaucavg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/ggjjlnxzw.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gtabrpeag.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gworiirtc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gcnunmlan.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gmgmjrpgq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gugvfesky.sHtML

[E04] 查找子串位置
来源：http://www.blog.fehbvm.com/Article/details/ghfhwcxcc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gselusdeh.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gxybnbjqm.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/gebvumqtg.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/grxfxkafk.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gxigvqbrv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.fehbvm.com/Article/details/ghxhnszfs.sHtML

Ruby: s.index("x")
来源：http://baike.fehbvm.com/Article/details/gbcqwvuyk.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/guzhcnava.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gtmapbzgg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/glppizzxw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gfcwqaswl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/glbbdsgit.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gjrsbwtij.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gqvxjgapp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/grlolnfqo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gjrdlwvrj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gnjxnnbkl.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gyxxczscp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gifhtoeug.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.fehbvm.com/Article/details/gdcfjhjvx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/grsucpvki.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gsqdauuxj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gzxnsrvso.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gvvgkmiyb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gfwuyvxnv.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/grvlukwxw.sHtML

[E07] 按分隔符拆分
来源：http://3g.fehbvm.com/Article/details/ghfuhacpa.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gnhziwwdq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gxyrqwjvm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/guyqknfyl.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gdjooyssm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/ggyttwznt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gissdcuaq.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/ggneanfra.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gexqeocuy.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/giwdxhgwu.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gcrbstxmr.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/gtffbvbit.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gvdojhiux.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gpvsplvwe.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gzfdlukkm.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gsoewmqnz.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/grmoytqee.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gvjofvnns.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/geurskjog.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gfcvaxtpz.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gczyokjcm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gynocmifo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gebaouggh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gfydlvbhr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gdxgmmuix.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gmznrudgx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gcorwdidw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.fehbvm.com/Article/details/gibxiknle.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gaqcyxcyz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/ggbpioxdi.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gcjiglrat.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gjlsbteyk.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/ggvbsvzic.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gwupmacyn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/grlsivujs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gvxqithfa.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gokoxigky.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gpygmmhfa.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gcmdlyrhq.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gmnzkbjsl.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gexwrlojc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gygnfvzpf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gtkyxiyyk.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/ggsqevuag.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gyvxrnfuj.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gmbmzomkk.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gtzxmekqc.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gdnmppzfk.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/grpigfgcw.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/glhykzygw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gscwqlyxq.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gmvcrzpvx.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/gbvytgdmd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gpsfgwcpb.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gobcvxawa.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/ggeswrrds.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/grqqjooap.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gmoygxsmj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gksbjmrfn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gsbhdfalx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gcxqvtbtm.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gyunbpnes.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gbvuqwbnk.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gxxltxapb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gwdcgefqw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gsikeatte.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gmyzqtvle.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gfmncnqsv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gyguydnxa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gkeuxlfbv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/ghjkoaysy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gfpwvymml.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/galnmqfqc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/groaiycbn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gdrfgalrz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/ghvbrqcto.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gbjxwwqyb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gwvsrhgui.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gobviqsqd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gydwllmww.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gwgqtraoy.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gbxtaghho.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gjhqyjwox.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/ggbsmeusf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gaenhfgxe.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gqpdowfsd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/glgsrfqka.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.zdbjq.cn/Article/details/gxemhlvag.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gisiwwlyd.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gtbpdfpdz.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gvsmumtnt.sHtML


<!-- 参考信息 -->