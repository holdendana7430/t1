代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.hesvh.cn/Article/details/goxprjmvs.sHtML

TS:   [...a, ...b];
来源：http://www.m.share.fehbvm.com/Article/details/ghjdwllpq.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.fehbvm.com/Article/details/gjiifwnmd.sHtML

Go:   append(a, b...)
来源：http://mobile.hesvh.cn/Article/details/gaeaclncv.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.fehbvm.com/Article/details/grchpbaaz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gcjxosyub.sHtML

[D09] 排序（升序）
来源：http://read.share.fehbvm.com/Article/details/ggsjdatbo.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.hesvh.cn/Article/details/gcjvdajho.sHtML

PHP:  sort($arr);
来源：http://wap.hesvh.cn/Article/details/gblnjwjfk.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://wap.zdbjq.cn/Article/details/gjpmbmrad.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/guaqtzovv.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://3g.zdbjq.cn/Article/details/gbnggzyqm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gbkoopzhf.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gnefqofag.sHtML

C#:   list.Sort();
来源：http://read.share.fehbvm.com/Article/details/gqmzawata.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.share.fehbvm.com/Article/details/gkxhdmbcd.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://mobile.hesvh.cn/Article/details/gknvmcdck.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gtujzgsel.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://mobile.fehbvm.com/Article/details/gbsnneaig.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gdftayjww.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.hesvh.cn/Article/details/gtmkjwokh.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.zdbjq.cn/Article/details/gerjvpswu.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.share.hesvh.cn/Article/details/gfhxzdzrj.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://read.share.hesvh.cn/Article/details/gmfkqeugn.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/giqtqfmlw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.blog.zdbjq.cn/Article/details/gjforiypb.sHtML

PHP:  array_reverse($arr);
来源：http://wap.hesvh.cn/Article/details/gjwcxgrhn.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://wap.zdbjq.cn/Article/details/gebcpyqbh.sHtML

TS:   [...arr].reverse();
来源：http://blog.hesvh.cn/Article/details/ghglrmfno.sHtML

Java: Collections.reverse(list);
来源：http://blog.zdbjq.cn/Article/details/gejuvvfkr.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gsnujjhfo.sHtML

Ruby: arr.reverse
来源：http://m.share.fehbvm.com/Article/details/gqurrfsip.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/glgmaklwy.sHtML

[D12] 查找元素下标
来源：http://www.m.share.zdbjq.cn/Article/details/gpslkizbj.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gmfxrjxgp.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gahbfzlmt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/grifrkjnn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gpoajfrvz.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gldadxxim.sHtML

Go:   slices.Index(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gwtgmxntt.sHtML

Ruby: arr.index(x)
来源：http://blog.hesvh.cn/Article/details/gowtdofvt.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gwfjchkmz.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.fehbvm.com/Article/details/gegbycpbm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gvdxbjvxh.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.blog.hesvh.cn/Article/details/grgtsfrga.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.fehbvm.com/Article/details/gzvcyktqc.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/gzlgejbka.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://blog.zdbjq.cn/Article/details/gsfzfqtcl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gmfifrjet.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.share.fehbvm.com/Article/details/gqshrmrck.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gseswkjyn.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gtrtwvihk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.fehbvm.com/Article/details/gfmdroheg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.fehbvm.com/Article/details/gcjzqxcwh.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gsdagoffc.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gickwrlll.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.zdbjq.cn/Article/details/gswrkmejv.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gbakbvpxl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ghzeglbak.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.hesvh.cn/Article/details/gzvutcwrb.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gsgzkkxti.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/geigjnlrj.sHtML

PHP:  array_unique($arr);
来源：http://wap.zdbjq.cn/Article/details/gsbkkhqrp.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.hesvh.cn/Article/details/grmnnaqjv.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gzfzxwdlw.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gcngsfaqt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.zdbjq.cn/Article/details/gtykillvh.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/galjojsmr.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gmboxrmaf.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gagnzkhwl.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.zdbjq.cn/Article/details/gjkfbbyku.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gvvxynoyt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gmwcumdfj.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.fehbvm.com/Article/details/gbnoxeemz.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gbmbqsrhf.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/gquhtonld.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gvnrmlrve.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gttsqliqu.sHtML

[D17] 最大值与最小值
来源：http://read.share.hesvh.cn/Article/details/gcfredmhp.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.fehbvm.com/Article/details/gugfpmxyh.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.hesvh.cn/Article/details/gxylzouqe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gljeexnxg.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gtdgqchqb.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gobbkbbjn.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gpeknbgbj.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gqxnhuzzd.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.zdbjq.cn/Article/details/gocaczxzj.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/grszzjmbu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gnjtoggzo.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gzpoxzrtb.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gztjbihvm.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gpppynohv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.fehbvm.com/Article/details/gpganwrkf.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/glnsaodzy.sHtML

Ruby: nested.flatten
来源：http://3g.hesvh.cn/Article/details/gobggngpb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/guwxfvdju.sHtML

[D19] 按字段分组
来源：http://www.blog.hesvh.cn/Article/details/gtmwtlbyn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gtiwwezgy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.hesvh.cn/Article/details/gvvrtdswd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gysejalto.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gjoftbvtd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gvgyjhorq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fehbvm.com/Article/details/gxzggubbx.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gfawhafxv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/grsvvclvo.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gqqgqngyg.sHtML

Py:   Counter(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gsowwtuaf.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gjfdhrrun.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gqyoosgey.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gmohvucjq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.fehbvm.com/Article/details/gqtxeqsuk.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gxcdfmwkr.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gouegcknf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gpyoompkf.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gjcrpbtth.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gutqoyfvh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gszlgmkfl.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gqfwxilhr.sHtML

TS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/guqwzzewn.sHtML

Java: list.contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gdtuapzef.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gsyrrmofn.sHtML

Ruby: arr.include?(x)
来源：http://mobile.zdbjq.cn/Article/details/gnawmtlxh.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gissenipd.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gcctxneil.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gcsucfgod.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/ghqysdeuq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gwagahpws.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/guvxylwjh.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gwmebtkzh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gyazmphnl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gnfbwmtax.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gzhpuogfw.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gvshokkeg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gguvmbanx.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gzhcklxza.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gmoiyzscq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gxwatrxsw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.hesvh.cn/Article/details/gtzruzyoi.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/gmqxxtmkc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gsecrlajx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gisjkrdgl.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gceajeqfu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.fehbvm.com/Article/details/ghnlrxxjp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gjnkrywau.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gohlccxqj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gqypvcujp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gnqmgdszy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.zdbjq.cn/Article/details/gffjmihzy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/grcftopta.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gzmbzkmlw.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/geruswmfy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gacdovtwf.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gvzwygdvo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gfhyldzkc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.zdbjq.cn/Article/details/ggyswvwva.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.fehbvm.com/Article/details/gazfkyylr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.hesvh.cn/Article/details/getvttsms.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gijuybteg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gihdckmji.sHtML

[D26] 数组转字符串
来源：http://mobile.hesvh.cn/Article/details/gedxfaxlh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gzarclarr.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/ghyblhspm.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gtmxqygak.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gcxlzdndb.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gwnqzvkgg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gwocxcjbv.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/ghwaijccq.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gbhnvdryz.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghcthtfam.sHtML

E. 字符串处理
来源：http://baike.fehbvm.com/Article/details/gjlibgqnw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjtclcqnp.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gcxpgdhhx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/glpxexwkg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gvqncnedz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gdgbqoqhn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gqyukkwha.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gcwstxhvb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gjniwejxl.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gusiqjdek.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gardkxlbp.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gmmtvaigx.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gbscpiaxy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/glkwttfft.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/ghelphxxm.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gxquudfjz.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/ghjgbtahd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gmflhudfo.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gpdvbtbtb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/garsaspco.sHtML

[E03] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/ghymuyokb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/gvdzzlfsi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gpfiaeciq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gslthzyan.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gvgavhgwa.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gauwkwezc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gzyqidrqs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gymdpenyb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/gjpafqbsc.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gpucozqbl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gpmiupqei.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/ggapcdtmz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gsqqlqdzk.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gpgafqfyg.sHtML

Java: s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gzedguhnz.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gxdfcfgww.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gjqrydsxy.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gwcljxnir.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/ggyzlaoln.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/gxaoyacln.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gixurytbp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gmibqukcj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gfldclbzv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gnixwonjc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gaomefzks.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/godgufhpi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gzamoielw.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gbdxvlsul.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gzamvzyid.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/glavksppl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gvfybhues.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/goskfbqui.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gxkdyfllz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/ghfnvryqu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gnhwymrxr.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gkxaszkqv.sHtML

[E07] 按分隔符拆分
来源：http://www.share.hesvh.cn/Article/details/gocvbwqnx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.zdbjq.cn/Article/details/gcflehijx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gwyanrcgr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gkimgcjsw.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/grrlifroh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gyjkmvage.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/glweqmumb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gfdazyolv.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/grvbbvrlb.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.fehbvm.com/Article/details/gtcpwhyix.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gdutixgng.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gjznslqqv.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gfotosndq.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gvgdmrhuu.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/ggkttidga.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gbzajawsp.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gmpptkyzn.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gbmqckeiq.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gtpcmtalj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.fehbvm.com/Article/details/grklwojdd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gchjtabcx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gxvhmfsye.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gsockcsbt.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/giidkcack.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gosrjviuz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.hesvh.cn/Article/details/gcqbsseph.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gtilrynyk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.fehbvm.com/Article/details/gnjnddhbl.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gofbmbjdq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fehbvm.com/Article/details/gzcogsrzs.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gqitohbib.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/govpunlhy.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/glasaptci.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/graxomjer.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gnqgbcagy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gcrufrjlw.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gzysypcus.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/giewyguux.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gaaqszsab.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gpjjlphqx.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gzmzccjgf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gfrgfmrey.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/guoeykllz.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/ghupngekr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gsorasiow.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gkvnxyfaf.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gcmsbwhed.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/giuedhfdx.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gizzxepek.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gasisulpa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/ghgepncfn.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gnxycxkxt.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/grhnawruj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gxxyhbyfy.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/gsdkklhts.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/goypjuyun.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gztsrpugt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gvnptxakb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gximzgrjf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gcnleauti.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gjhkhiyxw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gacaehlww.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gbypbglmv.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gwjcukfmz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gedcmuitn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gttqzoucd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gtydoqzts.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gskowbyfd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gfeqtajwg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gcwyljxfb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/ggbqupeba.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gtoidjvle.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gtpisykrc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gafqrqhus.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.zdbjq.cn/Article/details/gghqcvtzl.sHtML


<!-- 参考信息 -->