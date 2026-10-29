代发 wailian999

Java: list.size();
来源：http://blog.zdbjq.cn/Article/details/gteutjyws.sHtML

Go:   len(arr)
来源：http://wap.hesvh.cn/Article/details/gkqoqfpcm.sHtML

Ruby: arr.length; arr.size
来源：http://blog.zdbjq.cn/Article/details/gsudfpqod.sHtML

C#:   list.Count;
来源：http://blog.hesvh.cn/Article/details/gostjgwka.sHtML

[D07] 切片 / 取子数组
来源：http://mobile.zdbjq.cn/Article/details/gpiuxphup.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://baike.zdbjq.cn/Article/details/ghkcgfumj.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://3g.zdbjq.cn/Article/details/gopaaihhp.sHtML

JS:   arr.slice(1, 4);
来源：http://mobile.zdbjq.cn/Article/details/gyunebrwq.sHtML

TS:   arr.slice(1, 4);
来源：http://3g.fehbvm.com/Article/details/gjmrdoyie.sHtML

Java: list.subList(1, 4);
来源：http://3g.zdbjq.cn/Article/details/glwxaoeam.sHtML

Go:   arr[1:4]
来源：http://baike.hesvh.cn/Article/details/gslojosgg.sHtML

Ruby: arr[1, 3]
来源：http://baike.hesvh.cn/Article/details/gbvbxgdvt.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.share.zdbjq.cn/Article/details/gauzkehem.sHtML

[D08] 合并两个数组
来源：http://www.share.hesvh.cn/Article/details/gzxbcxubx.sHtML

Py:   a + b;  a.extend(b)
来源：http://read.share.zdbjq.cn/Article/details/gqsjtxkhv.sHtML

PHP:  array_merge($a, $b);
来源：http://www.blog.fehbvm.com/Article/details/gomxbjuyr.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://mobile.zdbjq.cn/Article/details/gunfnqzcz.sHtML

TS:   [...a, ...b];
来源：http://www.blog.hesvh.cn/Article/details/glhzwenet.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://m.share.fehbvm.com/Article/details/govazbruu.sHtML

Go:   append(a, b...)
来源：http://wap.hesvh.cn/Article/details/gpiajyimi.sHtML

Ruby: a + b;  a.concat(b)
来源：http://mobile.hesvh.cn/Article/details/gtprxokky.sHtML

C#:   a.Concat(b).ToList()
来源：http://baike.zdbjq.cn/Article/details/gtvevzaxj.sHtML

[D09] 排序（升序）
来源：http://wap.fehbvm.com/Article/details/gonflslmk.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.hesvh.cn/Article/details/gkquywnjf.sHtML

PHP:  sort($arr);
来源：http://www.blog.hesvh.cn/Article/details/gztqxznii.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.zdbjq.cn/Article/details/gsratixym.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gyuorqumj.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.zdbjq.cn/Article/details/gzlqmincv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gdglfkbqw.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gmnxwulro.sHtML

C#:   list.Sort();
来源：http://baike.hesvh.cn/Article/details/gewurrtgb.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.hesvh.cn/Article/details/gtinwbsws.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.zdbjq.cn/Article/details/ghicuunyi.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://www.blog.hesvh.cn/Article/details/gwunkhkhs.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.zdbjq.cn/Article/details/gyaxfpnwg.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gusurycrc.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.zdbjq.cn/Article/details/glyazskdp.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.m.share.fehbvm.com/Article/details/gdytwddpg.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://www.m.share.fehbvm.com/Article/details/giuknxihk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://www.share.hesvh.cn/Article/details/gzrawynot.sHtML

[D11] 反转数组
来源：http://3g.fehbvm.com/Article/details/gvrwvejup.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.zdbjq.cn/Article/details/gozoymzzu.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.hesvh.cn/Article/details/gfkwvijcp.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.share.zdbjq.cn/Article/details/gsuqsqatu.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/ghboghbut.sHtML

Java: Collections.reverse(list);
来源：http://blog.fehbvm.com/Article/details/gdramvvpw.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.hesvh.cn/Article/details/gcqhpphkc.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gbtaudism.sHtML

C#:   list.Reverse();
来源：http://www.blog.zdbjq.cn/Article/details/gehslhugy.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/ghrzanign.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gxyisqaxq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.zdbjq.cn/Article/details/ghwdhakye.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.hesvh.cn/Article/details/gzseojfqe.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gkxzkegmq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.zdbjq.cn/Article/details/gzqelxmct.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.fehbvm.com/Article/details/gffwmnwbp.sHtML

Ruby: arr.index(x)
来源：http://3g.hesvh.cn/Article/details/gchivuhwm.sHtML

C#:   list.IndexOf(x);
来源：http://read.share.fehbvm.com/Article/details/ggeobvwud.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gatabobky.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/goeoibhtq.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gbucagcbs.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.share.zdbjq.cn/Article/details/gutrazpbh.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gzyrbqpqp.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://wap.fehbvm.com/Article/details/gdgjkilrf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.hesvh.cn/Article/details/gjlcmrvpq.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gywzojxqe.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://m.share.fehbvm.com/Article/details/ggjlwsnos.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gzgwbigpx.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gpljiaves.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/glgkflpsk.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/ghvnftcag.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/guxvvqndo.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://3g.fehbvm.com/Article/details/gzbdgffmg.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gftkxhicl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.zdbjq.cn/Article/details/gbxoapiqj.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gwrjwkdix.sHtML

[D15] 去重
来源：http://blog.fehbvm.com/Article/details/gcuencuiw.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.zdbjq.cn/Article/details/grlkjkyex.sHtML

PHP:  array_unique($arr);
来源：http://m.share.hesvh.cn/Article/details/gcgsvrigf.sHtML

JS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/glishytms.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/ghprtouse.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gimslrknp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.fehbvm.com/Article/details/gcsxeqjrq.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gbnlcyemy.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.zdbjq.cn/Article/details/gsgjpsrpx.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gnbtlkbrm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://mobile.fehbvm.com/Article/details/gatjukjls.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.zdbjq.cn/Article/details/gensaqhyk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gzcxswunc.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gqvonkfur.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gwdoswpja.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gpmmhmnhm.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/guklibaly.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.hesvh.cn/Article/details/gyatmmpsf.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gkzfbqbzk.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gdipvvtyc.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gigxufarv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.fehbvm.com/Article/details/ggcvvhjcm.sHtML

TS:   Math.max(...arr);
来源：http://mobile.fehbvm.com/Article/details/gkgglmfqy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gsfxeatnf.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/ghtkqqmkd.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.hesvh.cn/Article/details/guzmxeogn.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/gynfcsyfn.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/goyovnrdd.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/giemnomuu.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gowkthivx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.fehbvm.com/Article/details/gpjqrfiag.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gjbimibdz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gcwcrwqsk.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gzochmoql.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gxdrgbdde.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gzwkrmsel.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gjxahieye.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.hesvh.cn/Article/details/gmenzfrob.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gltwadbvu.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.fehbvm.com/Article/details/gahkmztoy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.zdbjq.cn/Article/details/gpwtwigtg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.zdbjq.cn/Article/details/gbouesmma.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.zdbjq.cn/Article/details/goqmphehf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gajzdidha.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gijtulehd.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gflfdmhel.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gjourpufe.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/gnvtiojjx.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/grgqwcxtp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gnmwagoen.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gdthnzsnd.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gogczxvps.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gcfoimvxf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/glcxmqcre.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gowmheckw.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gpudhcvir.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.zdbjq.cn/Article/details/gcshtjokd.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/goiyodkmm.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gvlhjmzyr.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gtzjwsysk.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gozjyoabc.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gigvjmfrt.sHtML

C#:   list.Contains(x)
来源：http://3g.fehbvm.com/Article/details/gsnfzxsmu.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gzgjzbxpf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gxhbojfaz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.zdbjq.cn/Article/details/gvytraghv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnfvdawmt.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gezlqmdkd.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/ggysktgjn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gkmmlmxwe.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gputblwnx.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gjxzaxttj.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.fehbvm.com/Article/details/gtmkjznzm.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.fehbvm.com/Article/details/gbbexgfez.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.zdbjq.cn/Article/details/govbopkfs.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/genlqnqdm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gegshhqal.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gkepwcsbb.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gdabmiacb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gwiuqvsok.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gzcbmsvya.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gcrbukpap.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.fehbvm.com/Article/details/gbhxggtbk.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gzlgspdcl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gfixnmgnd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gaafvbidw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gtfxazkpw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gbiassryo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gxigxacbd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/gspbsgrkq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/gpfvvtrkp.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gpskamzsn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gtapabcgg.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gkpikljae.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.zdbjq.cn/Article/details/gcbrxfnvx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gjyivpcow.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gezmlkvhn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gkyjifsju.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gqnmyjhsk.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gjbfkuznq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gbuuoaaom.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gzszkzssg.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/guavtcucz.sHtML

TS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gakndlzac.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/gglpppctn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/grhvweeuz.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gaetomwse.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gqbbexeil.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtpzoscmx.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gqoonkvbi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gonohkotw.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gdahewlgp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gkjcyhrqe.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gsefjrfwt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gkzqpksmu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gnbksyzrc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gyqumisfa.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gfxgdfldz.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gdngepzag.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/glxiboibp.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gijakhhch.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gmjumdpwv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/gnwyttbum.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/ghwtwbntk.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gaxsuzikb.sHtML

Java: "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gdnujmoyb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gmjhsiilc.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/grjhoiijy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/gazlmfmkl.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/ghsjhilnn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.fehbvm.com/Article/details/gzoneyqll.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gnhqapubm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/giadpjfez.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/geyllcdgn.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gtjahafxa.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gyrpkpvgw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gkzhyzslz.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gxdfmkomc.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gvyikzwun.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gzjzecbcc.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gjvzqrwqs.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gllqhsafl.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gjierbpop.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gonjrqxwp.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gwswfytcb.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/glplhlsme.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/gxbucbcjm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gxvrcfsrd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gnguwsydn.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gmjzgrnvh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gzubstwtm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gjeviwsvn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/guwvxywmt.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gdandkbea.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gunuyyxol.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gwevqcgrz.sHtML

[E06] 替换子串
来源：http://www.blog.hesvh.cn/Article/details/gqwlpqhou.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/ggpcnbajf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gzzpefwoy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/genygjwma.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/ghtwgglfo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gyttvxjhr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gaaludkof.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbvpddjtd.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gryupikfs.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gvavvdxzd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gvpcatzug.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gtshdanpa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gwjszxajl.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gmdfdudbh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gwyuvanig.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/ggxhkaqco.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.hesvh.cn/Article/details/gjgsatpvk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/grnltiuhf.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/gfmjvhtuk.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/gjyjxevwd.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/guarctlhd.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gbxdtpeoq.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/ggdrkzels.sHtML

Java: String.join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gxjiupgbw.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gohadpvoj.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gyjneqymq.sHtML

C#:   string.Join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gdrnlxwxm.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gadbaoytu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gbhfofyvm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gvfmahfct.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gmyoegfvh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gfqprjjiu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gmgsqmcjo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gxydyevby.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gqxrhbpxn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gshpgspwh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gdpmwxggv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/ggvhrzqzl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gqvuciorq.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/glgfvhxlx.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gietwidej.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gkpdqyzlo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gjfruqbga.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/ghbinjlou.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/giyvrszwz.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gqzkbbmjq.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gfquntcqr.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/ghvdkqehm.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/geknrgckm.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/grwoedagz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gzodvjwbx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gjgxyvbxe.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gesspvizt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gevjoeuql.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gnoaczxnv.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/guzjwiiwo.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gytdurtjt.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gpyjjgfmu.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gnjnwfjqg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gsbbxtihr.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gkbnyottf.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gooupqtxd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gxlvjuhrb.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/girkwudrq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gwajmpmsw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gatbvagmy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gxdtyidlm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gfysvpyro.sHtML


<!-- 参考信息 -->