代发 wailian999

Java: list.size();
来源：http://3g.zdbjq.cn/Article/details/gmbzehmmn.sHtML

Go:   len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gmtcssapu.sHtML

Ruby: arr.length; arr.size
来源：http://wap.fehbvm.com/Article/details/gknfgkjvg.sHtML

C#:   list.Count;
来源：http://read.share.zdbjq.cn/Article/details/gxyidcmev.sHtML

[D07] 切片 / 取子数组
来源：http://m.share.fehbvm.com/Article/details/gujaxqfis.sHtML

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://m.share.hesvh.cn/Article/details/goyezjiph.sHtML

PHP:  array_slice($arr, 1, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gukzwmodv.sHtML

JS:   arr.slice(1, 4);
来源：http://baike.fehbvm.com/Article/details/gbnxsafqb.sHtML

TS:   arr.slice(1, 4);
来源：http://www.m.share.hesvh.cn/Article/details/gkcftpdhc.sHtML

Java: list.subList(1, 4);
来源：http://www.blog.fehbvm.com/Article/details/gtvnkqyvq.sHtML

Go:   arr[1:4]
来源：http://read.share.hesvh.cn/Article/details/gfhscgfwh.sHtML

Ruby: arr[1, 3]
来源：http://blog.hesvh.cn/Article/details/gzsnwychy.sHtML

C#:   list.GetRange(1, 3);
来源：http://www.blog.hesvh.cn/Article/details/gvhtjahli.sHtML

[D08] 合并两个数组
来源：http://baike.zdbjq.cn/Article/details/gfrhvupxq.sHtML

Py:   a + b;  a.extend(b)
来源：http://mobile.zdbjq.cn/Article/details/ghafysqyg.sHtML

PHP:  array_merge($a, $b);
来源：http://www.m.share.hesvh.cn/Article/details/gqykzuftl.sHtML

JS:   [...a, ...b];  a.concat(b);
来源：http://wap.fehbvm.com/Article/details/gyvnzlbzq.sHtML

TS:   [...a, ...b];
来源：http://3g.hesvh.cn/Article/details/gpqestpmu.sHtML

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://3g.zdbjq.cn/Article/details/grpyyclbh.sHtML

Go:   append(a, b...)
来源：http://3g.hesvh.cn/Article/details/guoyutibe.sHtML

Ruby: a + b;  a.concat(b)
来源：http://www.m.share.fehbvm.com/Article/details/glnkuskkt.sHtML

C#:   a.Concat(b).ToList()
来源：http://3g.zdbjq.cn/Article/details/gxmrdckgg.sHtML

[D09] 排序（升序）
来源：http://www.blog.hesvh.cn/Article/details/gbqyvrbgj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gwjsykhor.sHtML

PHP:  sort($arr);
来源：http://baike.hesvh.cn/Article/details/gqscwplub.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.fehbvm.com/Article/details/girttemym.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/gtzazhvox.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gpbneiqdy.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gboiceovi.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gextwxydf.sHtML

C#:   list.Sort();
来源：http://wap.fehbvm.com/Article/details/gcwtbzerm.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://www.m.share.hesvh.cn/Article/details/gitjesgje.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://m.share.fehbvm.com/Article/details/gxhvfrnfp.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.hesvh.cn/Article/details/gmcyemhre.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.fehbvm.com/Article/details/gwpgiuczo.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.zdbjq.cn/Article/details/grhnyzkft.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.m.share.fehbvm.com/Article/details/giykibzsm.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.fehbvm.com/Article/details/grmaopede.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.hesvh.cn/Article/details/gopqheqdn.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gwxzuhgdh.sHtML

[D11] 反转数组
来源：http://mobile.hesvh.cn/Article/details/gvzyplhga.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.hesvh.cn/Article/details/gbtzepbof.sHtML

PHP:  array_reverse($arr);
来源：http://m.share.fehbvm.com/Article/details/gjpabzrft.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://m.share.fehbvm.com/Article/details/gehbcdaof.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gbzlbtlkz.sHtML

Java: Collections.reverse(list);
来源：http://wap.fehbvm.com/Article/details/gjjmutdzv.sHtML

Go:   slices.Reverse(arr)
来源：http://3g.fehbvm.com/Article/details/ggowjhmsi.sHtML

Ruby: arr.reverse
来源：http://blog.fehbvm.com/Article/details/gjgpendpw.sHtML

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gfbijiqkh.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gtvcfqpgc.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gdufoacts.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://m.share.fehbvm.com/Article/details/gpkathrtz.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gkjxnawzp.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/grpxdrqeh.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/gzvwghdgx.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/guoeinvub.sHtML

Ruby: arr.index(x)
来源：http://mobile.zdbjq.cn/Article/details/gzmilnmks.sHtML

C#:   list.IndexOf(x);
来源：http://m.share.hesvh.cn/Article/details/gngioieho.sHtML

[D13] 过滤（保留满足条件的）
来源：http://read.share.zdbjq.cn/Article/details/gwcrobmha.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.zdbjq.cn/Article/details/gclpilkku.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/gzpjfasyn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.zdbjq.cn/Article/details/gohxpnrih.sHtML

TS:   arr.filter(x => x > 3)
来源：http://3g.hesvh.cn/Article/details/glwrxrtja.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gbrzxgqaz.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.blog.zdbjq.cn/Article/details/gvzqeoebx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.hesvh.cn/Article/details/gyfexfsbg.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gplyrbqef.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.share.fehbvm.com/Article/details/gasdljott.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://m.share.zdbjq.cn/Article/details/ggkaxjybj.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://read.share.hesvh.cn/Article/details/gtljykhsm.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gfhqnapfr.sHtML

TS:   arr.map(x => x * 2)
来源：http://m.share.fehbvm.com/Article/details/gokvqpfjs.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gzwxrfhsg.sHtML

Go:   // 手写循环
来源：http://baike.hesvh.cn/Article/details/gatggykao.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gyrhvcgjc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/gdueuhdou.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gsiwgvede.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://m.share.fehbvm.com/Article/details/geisndhyu.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gteqrwckt.sHtML

JS:   [...new Set(arr)]
来源：http://wap.zdbjq.cn/Article/details/gywvlmuhi.sHtML

TS:   [...new Set(arr)]
来源：http://www.m.share.hesvh.cn/Article/details/gvtszifeu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/grdkbralw.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.fehbvm.com/Article/details/gcotxwvka.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gnnbujxcx.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gwfglrdju.sHtML

[D16] 求和与平均值
来源：http://3g.hesvh.cn/Article/details/gfgoqnftc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkxjvbvsj.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.fehbvm.com/Article/details/gigbgysce.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gkaozupdd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.zdbjq.cn/Article/details/ggkebiaoa.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gbiapizeq.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/ggpfcwmcr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.fehbvm.com/Article/details/ggdgnqydq.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.fehbvm.com/Article/details/gsmwfuzwe.sHtML

[D17] 最大值与最小值
来源：http://baike.zdbjq.cn/Article/details/gfgzawvnd.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gyyidqzir.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/gaynognoo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gqayyvqtv.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/gmppftxqd.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.blog.zdbjq.cn/Article/details/gdnihyyxd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gdllznyjh.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gdlcobxyz.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gyvsuasgc.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gbvvbopvu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gyajtmfwd.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.hesvh.cn/Article/details/gdbncljuw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gmvgywcge.sHtML

TS:   nested.flat();
来源：http://mobile.zdbjq.cn/Article/details/ganjdpcjb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/gegufmivs.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gmcspbfdp.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gzkfocjwn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gjiwpoxdg.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/gpawbnvwv.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gbcuzqmev.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gzgbyhpyb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/grgjkwvbm.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/guxmikwlz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.zdbjq.cn/Article/details/gycokncqr.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gpjuiisob.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gkveqkueh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.hesvh.cn/Article/details/gfppmjrxa.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gihosazah.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/glsdqdzin.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.fehbvm.com/Article/details/giwzqqfbg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gazwituqv.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gazbaupwz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gnrvvqowr.sHtML

Go:   // 手写 map[T]int
来源：http://baike.zdbjq.cn/Article/details/gwmrwiqma.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/grltwytxd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gcotnztsd.sHtML

[D21] 判断是否包含某元素
来源：http://3g.fehbvm.com/Article/details/gtfdqvjpk.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gilrmuvyj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/giyghornq.sHtML

JS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gjhdfuxik.sHtML

TS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gypkthdaa.sHtML

Java: list.contains(x)
来源：http://www.share.fehbvm.com/Article/details/gvyrnendy.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/ggxaioswh.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gyxqhnawn.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gdtgcqonc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/giluoigkn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.zdbjq.cn/Article/details/gvqetgviy.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gxdalpxox.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.fehbvm.com/Article/details/ggddwijnd.sHtML

TS:   [...arr];
来源：http://www.blog.zdbjq.cn/Article/details/ggkazrdbo.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gbhgqpxtn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gdylwsucw.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/ggkixupyu.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gzbnxgcmq.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/goyxkthxs.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gczxhmsrz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gidnmpzjm.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/ghgzbjlny.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/ggephxxkg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gjjibaiyl.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gcfzbiame.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gaysjwgad.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/gadkxjxfl.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.hesvh.cn/Article/details/gsibzlrmp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/gxljizytj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/ggajgtocp.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gkaxzpzml.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/ggexxnmvq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gdbuqhbfg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.hesvh.cn/Article/details/grwttnkvd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gvvyilpnu.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gmdvibtpf.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gpfyojvjd.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gkauflilt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gvvytvyxp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gtrrbfauf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gzxvwvsue.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gpjxburwk.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gekmihcuu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fehbvm.com/Article/details/gdqyfjkwh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxvenfcyb.sHtML

[D26] 数组转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gpaekuwew.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gjebepwvq.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gmzcssdyd.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/grqpgoaov.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gqnbumyia.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gjftirziw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/ghpqrkfyh.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gyrnoetgd.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/ggtvnidsb.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggerkgsry.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/grdcyogki.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmzqeyzol.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/glnipdreu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gzkcqxcme.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gwswbmire.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/ghnwmxtmb.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gmedcqvqj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gjxikclnm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/glyehgoli.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/gzotichsz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gnyngcmue.sHtML

[E02] 重复字符串
来源：http://wap.hesvh.cn/Article/details/gcschxask.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/ghompxbhm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gqsakzogx.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gklovjrpa.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/glirclpwv.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gmzzfdrgf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gypfqnqwj.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gwebjpzgy.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gqfpldqdt.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gidgxsszv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gcfgtjomq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gqgwsmasa.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gejyfpwef.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gklohojnc.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/glskpyoem.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gqoygqsmd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.fehbvm.com/Article/details/gffvgizup.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/grncxtoyi.sHtML

[E04] 查找子串位置
来源：http://blog.hesvh.cn/Article/details/gwexxdjbi.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gubxxvdzv.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gdxxzazgy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gvqpacvyi.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gkrpmqidh.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/ggmzngfgf.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gqgtrbust.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gutnvqfqr.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gcsfwwjrp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gdopbagyv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/guraardyq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/ggnplaiqk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gkjwmfczo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gqihwmrnp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gquagskto.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gwrdvqymn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fehbvm.com/Article/details/gotsheafc.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.fehbvm.com/Article/details/gvmopbrsd.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gnlnzxmve.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gwpmmjywb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/ggfoirqak.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gdchrhrwn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gninfnvsv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gyblzdtna.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gbovmvvwr.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gmtxyimkv.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/ghnszdzcc.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gbmoegglc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/gnzixbbsh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/geneytawl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gzuwafwbn.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/golnwjqsv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gativdxjy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.fehbvm.com/Article/details/gvvktagpg.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gcgxdgscd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/gjcvedfsr.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gsumproym.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/glkfmgyfu.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/glilhjrog.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/ghdqxupvz.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gvmdyvxoe.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gqdprkonl.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gyzftoith.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/grmijjuco.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gyqdgqpbj.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gfqdyfszt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gdrfurzcr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gehvbckoo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gyuuopfyy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gfolsmqfc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gumcajpfg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gyfqpnote.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/grffavtot.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/grykhdjcm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gwyroafso.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gpzdmrfkr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/goxqnsgjo.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gacceeapo.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gzhocfxly.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gtjhhhbnt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gsfwsaryk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/giafhqtug.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gaskplwfe.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gkiifyplr.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gflpyshsm.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gkkevuuup.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gntlaqasw.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/goxyynvsc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gyxzqgdie.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gppddkaxh.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/grdionydh.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gdwkkcegi.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gauchigsg.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gsjlqjucy.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/gejxuyswh.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/ggxsivsky.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gbylqrblw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gjjuqnwhf.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gowsihifm.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gvbykkikr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.zdbjq.cn/Article/details/gjfgqqgpl.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gfrzwkkmy.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gmcjgokgr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gellifduy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gymnnznji.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gtwglciue.sHtML


<!-- 参考信息 -->