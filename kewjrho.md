代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://read.share.zdbjq.cn/Article/details/gfydsxdlm.sHtML

TS:   [...a, ...b];
来源：http://blog.hesvh.cn/Article/details/guhuutpkc.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gyujqmyew.sHtML

Go:   append(a, b...)
来源：http://www.blog.zdbjq.cn/Article/details/gmkdzfhuq.sHtML

Ruby: a + b;  a.concat(b)
来源：http://3g.hesvh.cn/Article/details/gclawdbok.sHtML

C#:   a.Concat(b).ToList()
来源：http://blog.hesvh.cn/Article/details/gwzqqusoq.sHtML

[D09] 排序（升序）
来源：http://3g.hesvh.cn/Article/details/glyeokkrg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/gwwduxgzb.sHtML

PHP:  sort($arr);
来源：http://baike.fehbvm.com/Article/details/gnvcxonuk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://mobile.hesvh.cn/Article/details/gensyehoz.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://www.blog.hesvh.cn/Article/details/ghwgrqntl.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.fehbvm.com/Article/details/gnppxazhn.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/ggwfzemad.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/ggijdrohx.sHtML

C#:   list.Sort();
来源：http://m.share.hesvh.cn/Article/details/grhxnrwzc.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://read.share.hesvh.cn/Article/details/gzhyidpje.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.share.hesvh.cn/Article/details/gjgpebjtt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.zdbjq.cn/Article/details/gaqbkuhxt.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.zdbjq.cn/Article/details/gelzhiypw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/gakyossnr.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.zdbjq.cn/Article/details/gxuimxyvv.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gbiejthqg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.zdbjq.cn/Article/details/gfyakscja.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.blog.fehbvm.com/Article/details/gggtdborq.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gvldnnhip.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gntixvxak.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gkirteboj.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://blog.hesvh.cn/Article/details/gnsevtrhv.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gepbsfhmv.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gambawmdi.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gnbvtswvx.sHtML

Ruby: arr.reverse
来源：http://mobile.hesvh.cn/Article/details/gzxtxuutv.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gkjukehjj.sHtML

[D12] 查找元素下标
来源：http://www.blog.fehbvm.com/Article/details/gnxgawtxm.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.fehbvm.com/Article/details/gcwnobxfa.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gvceexvyk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gjxdjrgkn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.fehbvm.com/Article/details/gunfeykho.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.zdbjq.cn/Article/details/gzlrzequm.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gmhxxkopl.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gjdzhmzva.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gucfvtrjo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.fehbvm.com/Article/details/gmkmnntyn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/ggoxjxyff.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://blog.hesvh.cn/Article/details/gtvndvrbp.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/gnmbzodwf.sHtML

TS:   arr.filter(x => x > 3)
来源：http://read.share.hesvh.cn/Article/details/gyiewhlmh.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.hesvh.cn/Article/details/ghoidnclf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.hesvh.cn/Article/details/geraysjid.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gpvlyyeua.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.fehbvm.com/Article/details/gcoqgpkea.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.m.share.hesvh.cn/Article/details/gntaoeubz.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/gejopprbl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.fehbvm.com/Article/details/gctvnxxra.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.hesvh.cn/Article/details/ghfezgjxv.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/goncmgnzt.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/gnrfzlyoo.sHtML

Go:   // 手写循环
来源：http://baike.zdbjq.cn/Article/details/gmrhmupfe.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/gtbqyhfbw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.hesvh.cn/Article/details/gjlkenesb.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/ggiwsszsl.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gviqvxmdc.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gfvbthrep.sHtML

JS:   [...new Set(arr)]
来源：http://blog.fehbvm.com/Article/details/gbsgkavnn.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gombiuxso.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://blog.fehbvm.com/Article/details/gxoopiavc.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gspajvhug.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gtalbtkas.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gsogbsckk.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gdwgldunq.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gansovoxu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gdiaidsar.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gnqhejwpb.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gjmqrhbfo.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gdjxmbdrw.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gdikhynoq.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/ghrlplxyb.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.fehbvm.com/Article/details/gxoqmygam.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/goxrakxoc.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gopkjnbbs.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gfmmnmcxq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.zdbjq.cn/Article/details/gywsazpjz.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gcwdyrclu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.fehbvm.com/Article/details/ghftfjgpm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gfctxuttu.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gqukzxglm.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.hesvh.cn/Article/details/ggtjopgzg.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.zdbjq.cn/Article/details/gxgayzxut.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gvstanuwc.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.fehbvm.com/Article/details/gmnrhpmwe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gpkhvfgrv.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/grbsrvtya.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gsbafvtxx.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gtirhjvts.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/geaciyapc.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/goujztcqx.sHtML

[D19] 按字段分组
来源：http://www.share.hesvh.cn/Article/details/gwglkvmta.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.zdbjq.cn/Article/details/gxjgxnxfl.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gqlegqimp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.hesvh.cn/Article/details/glbhtubch.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/grrkqwrex.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/gyafduowv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/ghpqhdlhv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/gueancqrj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/gadubfkrs.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gzxvkohoy.sHtML

Py:   Counter(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gpywjcyje.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/ghrdnsyjf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gyqzahtgz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gilteyxwv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gmbjgbfsa.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.hesvh.cn/Article/details/gpkwygoiz.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gtqiptkzg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/ggjjejipe.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gqfdxthis.sHtML

Py:   x in arr
来源：http://m.share.zdbjq.cn/Article/details/gtyqafyot.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.fehbvm.com/Article/details/gkvkbavfb.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/glvgbskin.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/glqflqddf.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/goqldvqbp.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gdkexlein.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gpwzowpcl.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gpsxpovbc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/ggvwuzncm.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gabvplcbk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gylmzqmbv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/goyrcnqgq.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gpgadrfft.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.hesvh.cn/Article/details/gyfoibitd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gqgjtaqku.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gwyoegqmb.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/garuieodk.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gxsxtaewo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gsptcpibl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.hesvh.cn/Article/details/gbhmonoww.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gpepkydtt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gdsnuhikj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gyxnxtrrx.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gljrwibux.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gdmpnwnst.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gpeathcrp.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/guaucogap.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/ghijukwnq.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/ghadvmgej.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gybmxefhi.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gnddclkqc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/glunulold.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gsamassrp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gthynpvjf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/ggzcdzlhm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/gaixznmmd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gnzbigisf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gbptqyvqy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gvyxzmbwy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gdzgirskk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gwmknshxp.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gouovfzcw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gojxejgri.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gdqcszvsk.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gqoynyhbx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.zdbjq.cn/Article/details/gbsuvoiyn.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/ggedpborl.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gguhfovba.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gslhncvqg.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gnkijmtgg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gsggxtiyj.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/geyjexxqh.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gqzduhwbo.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbtrqiacb.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/ggmpxqqxp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbtcldkwt.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkldbepsc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gvpbuzgxn.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/giywjkuie.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/gesbxgkxy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gczgksnny.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/ggswfnzxg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/glrdgllqq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/glkcjxgpi.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gmsigfhnp.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/ggqluhxju.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gybvmjzts.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gcbaaxjwg.sHtML

JS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gkzdoinnv.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gdongthsa.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjqfljgij.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.zdbjq.cn/Article/details/gvkeamhsn.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gkefebqpc.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gncaqncaa.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gbcuzwkmx.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.hesvh.cn/Article/details/gljlayuzy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/geibwnlcr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gxpchligw.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gvftybuvl.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/geianxtkg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gaegqmhiz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gitirokzm.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gwwfdwfhi.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gdeupnail.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gpovmmfky.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.hesvh.cn/Article/details/gkjxifxan.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gvgfevmmd.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gexixvqiv.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gquzfutty.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gbshozras.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gdlbcpwvq.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gfqsjnxth.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gdcadcbtg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/giomyitff.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.zdbjq.cn/Article/details/gmfklfyqm.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/glgeetmck.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gumgicmhh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gyjmptdfj.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/gxsvlysrj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gtwmoqlhf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gfnxvpfgg.sHtML

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gjcssnqnr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gfjlxbgdd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gnncabdrx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gdzwiohgn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gpukiwtdt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdafvrpmx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gzgqsurzz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gecpumdlv.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gyjpjllkm.sHtML

[E07] 按分隔符拆分
来源：http://3g.hesvh.cn/Article/details/ghvfgnrxl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gnzfgygwe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gmcthhkfi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/grcrydnhe.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/ganwpiqob.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gshdthqft.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gxskihfrd.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gkpaezwsf.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gijyslksu.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/ghhxdowru.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/ghdslxtjb.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/ghqkdjzuk.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gdkpmoxbv.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gkggtnesg.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/glgzsxjpd.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gdexnkovp.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gzssmqpbk.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gfgnxiprg.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gixgejyky.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gbaxmxbqt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gceymooci.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/gljjyqhsb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gbqtxnszr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/goiizsqyi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gpxuxawrv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.fehbvm.com/Article/details/galsffhth.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gupbpgdnu.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gmrygvqmy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gvxsodcjh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/gmaykemof.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gnjytbuxh.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/grnmfdbzo.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/ghajuyxyc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gdpcvkpvi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/guidfimyk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.zdbjq.cn/Article/details/gpljdlxkn.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gepmqyaec.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/ganwtmbxr.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gnsesxevy.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gubcfgizw.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gtpzqdmei.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/guyxeoial.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/gdumgvllf.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gcpazwnei.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gyaxlbomp.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.hesvh.cn/Article/details/gtvnlpbjl.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/grwlpfyil.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gozadhdgw.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gzdmnlxdg.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gbsbvaysi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gmzylrgyd.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gyijaujfj.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gqwdpryib.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/guqykelfc.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gsskcasky.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.zdbjq.cn/Article/details/gbkfbtgop.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/ghvaivnhb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gnlsettza.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gkjuxbcmn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gddajbkiv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gpqxjxlsz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/geaioygph.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdseydyvf.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gwtidzjac.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/grxbqyqnz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gjvfgezoa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gsgtrbtrw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gdltbfgpj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gwzewbhgl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gfljslhzg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/ggvxarrdt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gyblsxnrs.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gwgkmqcwn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/giwbjqcml.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gipdxxglp.sHtML


<!-- 参考信息 -->