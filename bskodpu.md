代发 wailian999

[D07] 切片 / 取子数组
来源：http://wap.hesvh.cn/Article/details/gdbofvcuf.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://www.blog.fehbvm.com/Article/details/glmokbzsl.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://mobile.zdbjq.cn/Article/details/ghoasiwyn.sHtML

JS:   arr.slice(1, 4);
来源：http://read.share.hesvh.cn/Article/details/gokmucyto.sHtML

TS:   arr.slice(1, 4);
来源：http://baike.hesvh.cn/Article/details/gsnsrgohq.sHtML

Java: list.subList(1, 4);
来源：http://wap.zdbjq.cn/Article/details/glbnvwcdr.sHtML

Go:   arr[1:4]
来源：http://www.m.share.zdbjq.cn/Article/details/guhafcjbr.sHtML

Ruby: arr[1, 3]
来源：http://m.share.zdbjq.cn/Article/details/gyqkzqdlx.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gkyywgssh.sHtML

[D08] 合并两个数组
来源：http://www.m.share.hesvh.cn/Article/details/gbchmvcrt.sHtML

Py:   a + b;  a.extend(b)
来源：http://www.share.fehbvm.com/Article/details/gzxoixvth.sHtML

PHP:  array_merge($a, $b);
来源：http://blog.zdbjq.cn/Article/details/gxptqtern.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://3g.hesvh.cn/Article/details/gmoxqpsnv.sHtML

TS:   [...a, ...b];
来源：http://m.share.fehbvm.com/Article/details/gbmrockuv.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://wap.zdbjq.cn/Article/details/gdelvvweg.sHtML

Go:   append(a, b...)
来源：http://read.share.zdbjq.cn/Article/details/gdmlrjopr.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.blog.hesvh.cn/Article/details/gzacbbsyq.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.fehbvm.com/Article/details/gqteoeldf.sHtML

[D09] 排序（升序）
来源：http://mobile.zdbjq.cn/Article/details/gjhumtbka.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/ghgbsozpo.sHtML

PHP:  sort($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gttutauhc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/gvqriwahi.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://blog.zdbjq.cn/Article/details/gjdvmjcio.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.zdbjq.cn/Article/details/gcwuifdxm.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gvdvgzmyx.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gikvekhsc.sHtML

C#:   list.Sort();
来源：http://wap.hesvh.cn/Article/details/gpvpitbem.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.fehbvm.com/Article/details/gncalxfxf.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.hesvh.cn/Article/details/gqehnhbuw.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://wap.zdbjq.cn/Article/details/gdecpczgg.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gtusiildw.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/gcqbjcxbp.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://read.share.fehbvm.com/Article/details/gbtxsfzki.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.hesvh.cn/Article/details/gktmfcwaj.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.hesvh.cn/Article/details/glcpgrhmx.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.fehbvm.com/Article/details/gudikrqfe.sHtML

[D11] 反转数组
来源：http://www.blog.zdbjq.cn/Article/details/grooljdeu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://m.share.hesvh.cn/Article/details/gmigndsnw.sHtML

PHP:  array_reverse($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gxmkvimhk.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/golxnlcoe.sHtML

TS:   [...arr].reverse();
来源：http://wap.fehbvm.com/Article/details/gkbrlhopp.sHtML

Java: Collections.reverse(list);
来源：http://read.share.fehbvm.com/Article/details/gjqqtrqml.sHtML

Go:   slices.Reverse(arr)
来源：http://mobile.zdbjq.cn/Article/details/gcbwustbm.sHtML

Ruby: arr.reverse
来源：http://3g.zdbjq.cn/Article/details/ghlpvhtuk.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/guedsvvaa.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/goqydokum.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.zdbjq.cn/Article/details/gtxxlkyai.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gtuxizvfg.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gbhwevjjh.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/gmcodqmvi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.hesvh.cn/Article/details/gystzkurp.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gulvxcznv.sHtML

Ruby: arr.index(x)
来源：http://www.blog.hesvh.cn/Article/details/gylgshdxi.sHtML

C#:   list.IndexOf(x);
来源：http://baike.zdbjq.cn/Article/details/gxjjlwnyt.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gsnumcqdu.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.zdbjq.cn/Article/details/grafqeqsc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://baike.hesvh.cn/Article/details/gslvfqkim.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gdblsckrt.sHtML

TS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gnothktob.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://baike.hesvh.cn/Article/details/gwpuxwski.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/grbfmarxl.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.fehbvm.com/Article/details/gatcnxqnw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.fehbvm.com/Article/details/gtoainpfo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://wap.zdbjq.cn/Article/details/gywzrsuhb.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gfietvzan.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gudwvjpsg.sHtML

JS:   arr.map(x => x * 2)
来源：http://mobile.hesvh.cn/Article/details/gubbjxkhm.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.hesvh.cn/Article/details/gahvddesm.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gihjwhuxe.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gdtjxyrmt.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gqikqodcg.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/gurqdlbdp.sHtML

[D15] 去重
来源：http://baike.hesvh.cn/Article/details/gchfwzcty.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.zdbjq.cn/Article/details/gzpipcksc.sHtML

PHP:  array_unique($arr);
来源：http://3g.hesvh.cn/Article/details/ggftvdnqq.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gzhmplofg.sHtML

TS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gzrblplji.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.hesvh.cn/Article/details/gbybojlgx.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/gvuzeisrh.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/gtxlbzprt.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.fehbvm.com/Article/details/ggxagpeto.sHtML

[D16] 求和与平均值
来源：http://baike.fehbvm.com/Article/details/gixophdzt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.zdbjq.cn/Article/details/gvtehjbaq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.fehbvm.com/Article/details/gbkftcjeu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gkexfbsqt.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.fehbvm.com/Article/details/grukjvvji.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gpmeewyko.sHtML

Go:   // 手写循环累加
来源：http://3g.hesvh.cn/Article/details/gkeihsufl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gxtghukcl.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.zdbjq.cn/Article/details/gmyerlcek.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gotfzrdvt.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gteflankx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gjhhofqkd.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gxuycuygd.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gfuuwnvoj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/gqttttkeh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gkraxxbjf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gejowbwej.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gbmboiggn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.fehbvm.com/Article/details/gakuiwkng.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gfubvbxdf.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gpbstgvri.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gndeuionx.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gwaypdmdr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gpybgctgi.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gfcxqlgwp.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gslmphuyl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gaodoyqqu.sHtML

[D19] 按字段分组
来源：http://www.share.zdbjq.cn/Article/details/gdvhxrxtu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gfnvpaqaw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gqdyrhyvb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gnvmrgwmq.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/grhbgwehv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/gmylcukdl.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/glhntsrvq.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gctvrfnmz.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.hesvh.cn/Article/details/gmsxlktyk.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gcgpxrfjx.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gfghagide.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gecmplajb.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gyunviien.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/goqclmama.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gepeyaiyy.sHtML

Go:   // 手写 map[T]int
来源：http://wap.zdbjq.cn/Article/details/gevfdelxv.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gbokpjurl.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/giwrtkclt.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gtctkpnyp.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/gojunuooe.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/geonvfpnx.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gemliuvqw.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gipcsmgnt.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gvyskbwcw.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gkjxflbme.sHtML

Ruby: arr.include?(x)
来源：http://wap.fehbvm.com/Article/details/gaffeujjc.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gevurkmeh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/grgnvpbbt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.fehbvm.com/Article/details/gettzdcvy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/guwgboqog.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gwxoyrnsw.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/ghdtbnlol.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gkrxnmxii.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.hesvh.cn/Article/details/gilvuynyq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gemofeazu.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/getylmwjk.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gybaaajcn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gedsbzppd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fehbvm.com/Article/details/gdwduczfh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gpvrdbxqe.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gpoquhaay.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.fehbvm.com/Article/details/gujysnjbi.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gcirjlxsj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.zdbjq.cn/Article/details/gwtpqyxhc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gwtqmcpmt.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/gjnpisvow.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/glzizklrv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gjktoigqn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gvmpnyuof.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gjqgkxfcl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gssoiivzd.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/ggkdxuorp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/guwwohapp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/gdzonqyzn.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gmfrqyyly.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gmsihotoj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gbjlrwuol.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.fehbvm.com/Article/details/gwizrurfu.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gahynziwi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/guslzlyhz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/grkfaxgae.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.hesvh.cn/Article/details/giqkqvcxm.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gwzcnxwlz.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghwibtrnu.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gxperylpm.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gwdyqhlmy.sHtML

JS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/ggeliyigd.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/grjzprrjp.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gdakcniyv.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/gqeuxxkdp.sHtML

Ruby: arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gpcrifdzl.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gksjgccmm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gslxpoezf.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gwevqtwzb.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxlepxegf.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gllrzsvzo.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gwmcjvebo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gczmjrrad.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/glgjvolji.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gefueztnj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gtnqomqqq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/gqingqygg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gelmiskji.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/gigtrlkyv.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/guwahlmed.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gitovxvpu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gjtujimak.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gbhcbkhta.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gzimzwiir.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gzsbzwmsk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fehbvm.com/Article/details/gtpebuohf.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gfdeeybsk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/ghkxoionk.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/gnyyauwyq.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gzemlwrpx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gtcfaqpok.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/ghqkymwtp.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gxycflwhp.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gpomqezcv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/gboyfitvr.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/grdocwudj.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/gqbxkgbdc.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gilimboou.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gafcfrgig.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gvyymdlle.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.fehbvm.com/Article/details/gmnfnkizr.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gagwqflfi.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gcszuoukw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/glpptffaf.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/grzgnyysp.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gssmwyvqg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gutlzcneu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/glixjspdu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/ggqcquqzk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gmqoiojen.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gkrjbbbqz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gjazjqaga.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/ghythcyzi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gvbqjecrl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gyemnscdk.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gccknrlqq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gvfwohmvb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gvhfpyubb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/giotuwsaj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/goalxsgem.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gnrxxlqnq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/ghhpyzhca.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gmowprahe.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gadctxaqb.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gpzafqckg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.fehbvm.com/Article/details/gzatwjfdv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gfguklbfu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gzvhfncfp.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gpopcrtnf.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gxukbjskj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gxarhpvcw.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gjptiqvcs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/glztwakeg.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gcormrupp.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gmsigaiql.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/glthapgpe.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/glxwlmkcf.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gvzujvbso.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/glrhsurvz.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/glsvfygqh.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/guwpcxwfm.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gqvlcvpdd.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gopxmxvel.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/ganbzzgbp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/giuvogaby.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gnccddjaf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/geegfmfqw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.hesvh.cn/Article/details/gpfgsfggh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.hesvh.cn/Article/details/gwrkfnsya.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gntccmxgs.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.hesvh.cn/Article/details/gomzrstgi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gwvurjvey.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.hesvh.cn/Article/details/grzrfzsbh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gcvqsuuyr.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gdyljrpvs.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gvfefkuhi.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gzowhzshc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/goltmmdjh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/ghsnmrktq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gbbqodfob.sHtML

[E11] 反转字符串
来源：http://www.share.zdbjq.cn/Article/details/gjlxhnrfy.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gsbfkzzvd.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gdkdnuewx.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gccsyfeoj.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gslwzpoyd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/giqkzsxgy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gvruiaaek.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gnemdtcod.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gxkhivzrz.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/galfkymvb.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gzfhnwmnp.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gsxasuxid.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gpwrwamwk.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gnzzcgxmx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/glhvdtjwl.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gngykucxt.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gwcqmpbff.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/ghgwackzu.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gmgpryxzd.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gjbzohnld.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gbdvlayie.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gwysyfjop.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gfuslyjse.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gmokegaoh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/glzepbxkp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gorwdsxkt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gqknkyqxz.sHtML


<!-- 参考信息 -->