代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://blog.hesvh.cn/Article/details/gclekopiv.sHtML

TS:   [...a, ...b];
来源：http://blog.fehbvm.com/Article/details/grgjeppcm.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://mobile.fehbvm.com/Article/details/gzkrtnmyu.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/goxqrfjon.sHtML

Ruby: a + b;  a.concat(b)
来源：http://m.share.fehbvm.com/Article/details/gplhykyvz.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.hesvh.cn/Article/details/grifrzdkz.sHtML

[D09] 排序（升序）
来源：http://read.share.zdbjq.cn/Article/details/gcgnjpqzb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gtzthvmby.sHtML

PHP:  sort($arr);
来源：http://3g.hesvh.cn/Article/details/gvpcruwon.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gahruqoig.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/goksoewaf.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gubsuocfd.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/giviuedwv.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gqokecjok.sHtML

C#:   list.Sort();
来源：http://www.blog.zdbjq.cn/Article/details/gyxydbbim.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.blog.hesvh.cn/Article/details/gnyayltow.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.fehbvm.com/Article/details/gczhkvygt.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gescpjagb.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.zdbjq.cn/Article/details/gimgmvhjh.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.fehbvm.com/Article/details/grdvwfttd.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://m.share.fehbvm.com/Article/details/gxaqvjsod.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gqexdzort.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gsqltqapk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gtygmqsrh.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/ghfgqncti.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.zdbjq.cn/Article/details/gnhxoaufq.sHtML

PHP:  array_reverse($arr);
来源：http://baike.hesvh.cn/Article/details/geajofmvl.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gwlsvqwvx.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gequxfzvm.sHtML

Java: Collections.reverse(list);
来源：http://3g.fehbvm.com/Article/details/gjwfzrrda.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.fehbvm.com/Article/details/gglrkrpfz.sHtML

Ruby: arr.reverse
来源：http://www.share.fehbvm.com/Article/details/gejkawfom.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gyyukposz.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/girlprdim.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.hesvh.cn/Article/details/gjcbjejem.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/gbucnialy.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/guuofhocw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://mobile.fehbvm.com/Article/details/gcapafwta.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://baike.fehbvm.com/Article/details/gngnzblfz.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.fehbvm.com/Article/details/gecgzhtvg.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gqjkwuzyh.sHtML

C#:   list.IndexOf(x);
来源：http://baike.hesvh.cn/Article/details/gxsplhwgh.sHtML

[D13] 过滤（保留满足条件的）
来源：http://3g.fehbvm.com/Article/details/guobyuoic.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.fehbvm.com/Article/details/ggvmzdlvu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/gvqbcdpsu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gknybogxb.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.share.hesvh.cn/Article/details/gicjdapar.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gibwdcxsf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://mobile.hesvh.cn/Article/details/gbdrumwsw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://mobile.fehbvm.com/Article/details/glhgedals.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gcvkjjvkh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/gcyaixvvg.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gfesgflpx.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.zdbjq.cn/Article/details/gnhefcvoj.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.hesvh.cn/Article/details/gtjnrrgvo.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gqqxlmfwd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.fehbvm.com/Article/details/graohejri.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gmdhnnygf.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/grylvsnal.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/glwaegaap.sHtML

[D15] 去重
来源：http://3g.hesvh.cn/Article/details/gbveferog.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.fehbvm.com/Article/details/gsqvgxxlp.sHtML

PHP:  array_unique($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gvswegpde.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gcvxmawyx.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/ghtihyvtf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.zdbjq.cn/Article/details/gxcrkaigz.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.share.fehbvm.com/Article/details/giilmgxit.sHtML

Ruby: arr.uniq
来源：http://wap.hesvh.cn/Article/details/gtoarhhxz.sHtML

C#:   list.Distinct().ToList()
来源：http://baike.hesvh.cn/Article/details/geebdfate.sHtML

[D16] 求和与平均值
来源：http://read.share.hesvh.cn/Article/details/gajavfuzf.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://read.share.hesvh.cn/Article/details/gqjawtatf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.hesvh.cn/Article/details/gswoyujmb.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/gbrzcjupq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gzffhmmhx.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.fehbvm.com/Article/details/gfglmylbw.sHtML

Go:   // 手写循环累加
来源：http://mobile.zdbjq.cn/Article/details/geeajkjtk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/gggslovdj.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.blog.hesvh.cn/Article/details/gqyyvdone.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gzxafdlgz.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gjjovdtcy.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gbhwfwfzb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.fehbvm.com/Article/details/gdmplnoro.sHtML

TS:   Math.max(...arr);
来源：http://baike.zdbjq.cn/Article/details/gcmtvaktk.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/ggqzueyha.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.hesvh.cn/Article/details/gbtepfvlx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/guoswtsgl.sHtML

C#:   list.Max();  list.Min()
来源：http://mobile.fehbvm.com/Article/details/gshcvbscp.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gnyhuzsju.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/gorysfdag.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.hesvh.cn/Article/details/gmewjwmxg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.fehbvm.com/Article/details/gpammyjgj.sHtML

TS:   nested.flat();
来源：http://wap.hesvh.cn/Article/details/gbnsqpiab.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.hesvh.cn/Article/details/gbllvqins.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gocbmcnhc.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gpysnoljj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.zdbjq.cn/Article/details/guyjgvoiy.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gzxkiunih.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gcfgnlesy.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gudfpfzga.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.fehbvm.com/Article/details/gwfcktdpl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.hesvh.cn/Article/details/gwoyhqmei.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/ggoialkyy.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gumjfwwrr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.zdbjq.cn/Article/details/gnokfwxhe.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.hesvh.cn/Article/details/gsftngusc.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/grxhnzbyg.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gextooojf.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gfxqeizsp.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/guyjxmiuz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gmsywkaem.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gxlugdspz.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gdncrvhlu.sHtML

Ruby: arr.tally
来源：http://3g.zdbjq.cn/Article/details/gqbtwmpks.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gwdqtkopu.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gojyejsne.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/ghrdmkfxu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/ghdguglps.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gxrlljyua.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gkluwyhzv.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gbkdluocw.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gdedpswfv.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gzjntmxqy.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/gsxgluafy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gbnkfwrld.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/grgclmyis.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/gptclazec.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/ggzmnhvlt.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gmqozwbxi.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/guxgfvupe.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gwzmlbvrw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gsmkdxjkj.sHtML

C#:   new List<int>(list);
来源：http://m.share.hesvh.cn/Article/details/gvwkfsxfk.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gqbwvmrlq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gaxukizaq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/grzsuzvdt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.hesvh.cn/Article/details/gayxnnzss.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/geieovazn.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gehpgjosk.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gwbittguc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gsbqjcqlx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gkihvksfe.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fehbvm.com/Article/details/gpfuibhnq.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/gobrniutx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gcrcmsnoj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gppzvyhcm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gyrydpzgd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gldgzqbgo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fehbvm.com/Article/details/gvellrpom.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/gezzgsqmq.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/ggodhnsxa.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gximwjwad.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.hesvh.cn/Article/details/gtnvvwfpc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/gtmyezzgn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gqmlhwyuy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gftvofvpx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gryhvlcjq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gqhwsesab.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gpgygbjxn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gbjtejtcn.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gxqnfautr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gjcecclad.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gipbldbre.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gpxeuvsmm.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/givniektr.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gfarsutmn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gtmzcmosg.sHtML

Ruby: arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gyjdpanwo.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/ghdqdhnau.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbgoeypku.sHtML

E. 字符串处理
来源：http://blog.zdbjq.cn/Article/details/gbykacfvt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvfkzuehs.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/guanypqpv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.hesvh.cn/Article/details/gdwwfzwjy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gptsfpjep.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gayetcrvy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gsjbaovci.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gjglgkhia.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fehbvm.com/Article/details/gawqqqvff.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gfzwevksk.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.fehbvm.com/Article/details/grkplfcaq.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gjansvilq.sHtML

Py:   "ab" * 3
来源：http://m.share.hesvh.cn/Article/details/gyrfvojxc.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gfmuifkoh.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/guyqbgwvu.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/ggzakeadw.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gforzxbjn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/gchxrbuij.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gjdivazfv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.fehbvm.com/Article/details/ginczxypj.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/ghicudyoi.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gaetocjcd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gtbpwewsi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gyjznxplq.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gddlcitab.sHtML

Java: s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gkmcslmuu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gjhlmwody.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/giwaglykw.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gcciqimwt.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gxljcmmnt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/grlquwisf.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gtluuilkn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/glltbetgh.sHtML

TS:   s.indexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gyjicltdd.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gioabwuqz.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/ghglaliqg.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/glilfnkra.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gxpcglzhg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gqemvmlni.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gmqmkffqw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gjbwujxhn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gnnaqewmk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gvyynnqvl.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/glcwulrpa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.hesvh.cn/Article/details/gijvuytrd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gjsmypxyw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gewahvbri.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gabsgjtpq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gwymkrnvn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/gtwuuajot.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gaufppnrp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gikndwnho.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gpotisyzm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gwxllsmxy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gbmxlcwqh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/ghrupunme.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gjuwgzygd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gmljlakah.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/guhbrfnic.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gjerrkrja.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gdqbrkzuj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gwmmlcxxk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gfmqwyzxd.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gezujzbkd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.hesvh.cn/Article/details/guglclewx.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gszmxrcmd.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gqiuuglqz.sHtML

PHP:  implode(",", $items);
来源：http://blog.hesvh.cn/Article/details/ghmtjrhui.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gcsbelflu.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gbquyzyts.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/goulgqfij.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gqvklnarb.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/goyhjpell.sHtML

C#:   string.Join(",", items)
来源：http://baike.hesvh.cn/Article/details/gvrujzabd.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.zdbjq.cn/Article/details/grphtwsjz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gajibnovq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gfeborjde.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/galtuaffm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gkjkrhvxe.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.hesvh.cn/Article/details/gxykntwyb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/grimludpv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gilcvivze.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gnfemhntb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gvctvntgb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gjdpyeuqa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/grdpmahpl.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gwdgowlxe.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/goyahrzao.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gqotzfeog.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gbsdrswqm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gvtztyqxl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gwablsmtg.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gowxzmtpt.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gftqybhyj.sHtML

PHP:  strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gfiybxaxn.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gykumdikl.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gcamilmyy.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gbbdbzkxm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gkndzmacg.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gbwlejoik.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gvxioflrj.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gonzfslsh.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gnbrioyaa.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/ggtyuvjti.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/greqecyht.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gostqrqyz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gibmooord.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/grouvukbr.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gytaxmktr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gpalxwygr.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/ghyybcmgc.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gepstorwk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/goxtgpazo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/geyfsxfxe.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwnuboyyw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gihqufunx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gfirdisql.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gjwzkwblt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gkjwwvbez.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/guguiyqzc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gedibddgm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtcprjhmn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gakggfdsn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gpmlxigwt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gzjbdawel.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gphhxaczr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gympucumf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/ghwkgpnwg.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/gpddwqrgd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gnvivgweh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gobgqodix.sHtML


<!-- 参考信息 -->