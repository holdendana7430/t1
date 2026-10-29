代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://wap.zdbjq.cn/Article/details/ggtbiawng.sHtML

C#:   a.Concat(b).ToList()
来源：http://wap.hesvh.cn/Article/details/gsnowrgsn.sHtML

[D09] 排序（升序）
来源：http://m.share.hesvh.cn/Article/details/gmcnlixiq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gmmjkuldr.sHtML

PHP:  sort($arr);
来源：http://mobile.hesvh.cn/Article/details/gpzdfcnel.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.share.hesvh.cn/Article/details/gxtoqmcmg.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.zdbjq.cn/Article/details/grxzlwkfu.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://baike.hesvh.cn/Article/details/gacjykehv.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gykmebdrq.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/glvcxnsol.sHtML

C#:   list.Sort();
来源：http://wap.zdbjq.cn/Article/details/gajzqxvla.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gwkkduyzj.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://baike.fehbvm.com/Article/details/gixbtxbcr.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://m.share.zdbjq.cn/Article/details/gyphycybv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://m.share.zdbjq.cn/Article/details/gnsvngewx.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://read.share.hesvh.cn/Article/details/gxtniybty.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://wap.fehbvm.com/Article/details/gybiigfuj.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://mobile.zdbjq.cn/Article/details/gmeowqghx.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gmeaxiafm.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.hesvh.cn/Article/details/gcvssmgvj.sHtML

[D11] 反转数组
来源：http://m.share.hesvh.cn/Article/details/gfbxpjrua.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://blog.hesvh.cn/Article/details/ggjjvgfvz.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.fehbvm.com/Article/details/gfyoemavm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.fehbvm.com/Article/details/gbuedwhfr.sHtML

TS:   [...arr].reverse();
来源：http://m.share.fehbvm.com/Article/details/gddtbbfuo.sHtML

Java: Collections.reverse(list);
来源：http://blog.hesvh.cn/Article/details/gwoxyeomg.sHtML

Go:   slices.Reverse(arr)
来源：http://m.share.hesvh.cn/Article/details/gkndzezlg.sHtML

Ruby: arr.reverse
来源：http://baike.zdbjq.cn/Article/details/gjfxuenej.sHtML

C#:   list.Reverse();
来源：http://baike.hesvh.cn/Article/details/gavrmjztg.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gcpicjrda.sHtML

Py:   arr.index(x);  x in arr
来源：http://3g.fehbvm.com/Article/details/gisnwacaz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.zdbjq.cn/Article/details/gicuhceou.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.hesvh.cn/Article/details/gbucyeuhw.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.zdbjq.cn/Article/details/gzejlggkj.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.zdbjq.cn/Article/details/guaccqxyb.sHtML

Go:   slices.Index(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gixoologk.sHtML

Ruby: arr.index(x)
来源：http://www.blog.fehbvm.com/Article/details/gqdzgylhv.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gwkhskwyr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://mobile.fehbvm.com/Article/details/gphegognr.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gdwktjbcf.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.zdbjq.cn/Article/details/ggfvveung.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gdggqxaus.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.hesvh.cn/Article/details/gsucpjgnt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.hesvh.cn/Article/details/gbdwucxjf.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://wap.fehbvm.com/Article/details/gpubjnbnj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.fehbvm.com/Article/details/gyjcgfahs.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://mobile.zdbjq.cn/Article/details/ghpfrdscf.sHtML

[D14] 映射转换（每个元素变形）
来源：http://blog.zdbjq.cn/Article/details/guhoyilku.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.zdbjq.cn/Article/details/gzkhotaxs.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.hesvh.cn/Article/details/gipxktdvo.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gycvmkmqp.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gzmpfguvn.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gioawaabb.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gyrbwpyeh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://3g.fehbvm.com/Article/details/gcuxwhanw.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://baike.fehbvm.com/Article/details/gzrvxhqqp.sHtML

[D15] 去重
来源：http://blog.zdbjq.cn/Article/details/gdolayhmf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.zdbjq.cn/Article/details/ggrojzkvu.sHtML

PHP:  array_unique($arr);
来源：http://read.share.fehbvm.com/Article/details/gbjmacmjm.sHtML

JS:   [...new Set(arr)]
来源：http://baike.hesvh.cn/Article/details/gpiacbxsw.sHtML

TS:   [...new Set(arr)]
来源：http://wap.fehbvm.com/Article/details/gzyarzpic.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://m.share.zdbjq.cn/Article/details/ggrutotuo.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://3g.fehbvm.com/Article/details/gjqfvfxwy.sHtML

Ruby: arr.uniq
来源：http://wap.fehbvm.com/Article/details/gizuhnnqx.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gjnrbywga.sHtML

[D16] 求和与平均值
来源：http://www.share.hesvh.cn/Article/details/gehwfceqn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gffcvoagk.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gaxuvfulg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/ghdwigfoa.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://mobile.fehbvm.com/Article/details/ghyhzjflu.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.hesvh.cn/Article/details/gdhnmwhlv.sHtML

Go:   // 手写循环累加
来源：http://read.share.hesvh.cn/Article/details/gmnkknvez.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.zdbjq.cn/Article/details/gyfjoqvuk.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.hesvh.cn/Article/details/grzbrcsoe.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gnurriigu.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gvswdgbbn.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gvhwwnuiv.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/gyvjotblu.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/geaimgkcf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gnnkszjye.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gkibgnooy.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gihwrtcjt.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gljuzaadb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.hesvh.cn/Article/details/gazntogzz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gotjvanum.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gwzgxkkzd.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gcnfdozzr.sHtML

TS:   nested.flat();
来源：http://3g.zdbjq.cn/Article/details/glaauyqiv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gafiawnza.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.fehbvm.com/Article/details/gkdlorzjw.sHtML

Ruby: nested.flatten
来源：http://www.blog.fehbvm.com/Article/details/gaqgvfdmy.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/ggcxnyqzm.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gzcprfiil.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gooilvfzf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/gqnjokpmf.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gkdgdxrui.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gttzbaoko.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gjqreyzlv.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fehbvm.com/Article/details/gdthbkxze.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gezdvexgt.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/grfoitffl.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gjwsrpglu.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gxkjcpvuk.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gflhwchcu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/gscoyxnge.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gubcxxgpn.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.zdbjq.cn/Article/details/gnibjspwl.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gvnxiarko.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gdgbcjiky.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.hesvh.cn/Article/details/gxyghhgqn.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gfbvifcth.sHtML

Py:   x in arr
来源：http://baike.fehbvm.com/Article/details/gxfnjossr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gepnxvbgt.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gdfxficcs.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gaexplskf.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gutjdqveo.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gwfatssvw.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gjxoasobb.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gkujyculx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gliwlkmga.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gnneicpcm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.fehbvm.com/Article/details/gggavcdsg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gherhwdey.sHtML

TS:   [...arr];
来源：http://baike.fehbvm.com/Article/details/gwgtphdkt.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.fehbvm.com/Article/details/gdgcqztfb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gnxqcnnpi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gwrvqozcr.sHtML

C#:   new List<int>(list);
来源：http://3g.hesvh.cn/Article/details/gzehxsbeh.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gfqkgxlvp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gmvgfdhgd.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gianhtlak.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gphrbgads.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gfwznyxnp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gfnopmrbt.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gflwqhlgx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.zdbjq.cn/Article/details/gwgacbcpb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/gpfzxberx.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gjwsnzpzg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gzmcxjwvm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gmgzbxaqc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.zdbjq.cn/Article/details/ghyggcpmh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gumrpgjad.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/gscawdzfv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gxvbtuxrm.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/gojguxmfv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gotirtytz.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gindblcxa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gznurknuw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gjmglxkzl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gwwqspecz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.zdbjq.cn/Article/details/gjcsduycc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/govksyoup.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gujfpbgvo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gnhtecqgs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.zdbjq.cn/Article/details/ghhecmaix.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gicdcsdhw.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gqsbenzdx.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gvgzxlobl.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gjemltaqa.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gwavjftvm.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gfonflmjq.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gsootejiy.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gxtvvnhiz.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gxisxjlkc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gppsehjdl.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/glglbplqh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gxkfhrwos.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gwzgrbxtv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/grbjfnnch.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gyayjcjyo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.zdbjq.cn/Article/details/gyuuhxjgo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.hesvh.cn/Article/details/gnwohokcm.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.hesvh.cn/Article/details/gkgtkguyl.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gsgqgxchq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.hesvh.cn/Article/details/gvxytuccy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/ghmhfioeu.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gwnduowyf.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/guqjzwpxr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gksqgsgni.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gntcowwhg.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/grquxwrnj.sHtML

Java: "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/guzzhyrqm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/gcdnlhugu.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gbcxhosag.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gzpuuwfzi.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gfzivvwyo.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/gmvzruqoj.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gxaulkupi.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gtkhhfovl.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gddqodazq.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gptjoxzww.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gqxxdlgtf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gqqtlgtix.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/glogwbhss.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/geqhtexes.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gtmgcldol.sHtML

PHP:  strpos($s, "x");
来源：http://blog.zdbjq.cn/Article/details/gksscvrbu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.zdbjq.cn/Article/details/gesgyocrs.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/gouibwbbx.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gfimuenmt.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gwykqsrss.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/genhndzlr.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gsovulxrv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gfkldnzwq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.fehbvm.com/Article/details/gbtojuzrq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gnlslzqtc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gxcnstakm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gxbczwrfn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gyjklvkqg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.hesvh.cn/Article/details/gqqgmncih.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gixdwfnxa.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/ggchlyahr.sHtML

[E06] 替换子串
来源：http://baike.fehbvm.com/Article/details/gtfehwvvc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/ggbclvlqg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/ghuvqzsly.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/glclpwprd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gktuepdjk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfqjgciol.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gbtnzyomj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gocmqrgfs.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gesptcbso.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/genpekbvq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gqyzdtbff.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/giexccwmu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.hesvh.cn/Article/details/gwuoilhlg.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gnqtcdkpt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gbggkfkqk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fehbvm.com/Article/details/gsfololbq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/gisoodafk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gfdpbgsfx.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/guyubsqot.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gegxjjwmj.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gpnueduwi.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/grsvrgrmg.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gifigvvyp.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gaxtnsekg.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gobhisxhq.sHtML

Ruby: items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gzwdhvzuh.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gnioxbchu.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gpaunanhu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gvumchpej.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gyjhkyrql.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gptvjuzlm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gcinszfot.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gznrqefhp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/ghvlqgxih.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gsdfhstsc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/giyofkqhs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gnwgckodj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gunehtnay.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gitukdpaq.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gfoiqrilw.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gasdqffub.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gdkjzxmyb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gsqffxfsb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/geugloakx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/gymwveahs.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gzbpfxzlz.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gqdsbqlit.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/grgqhqllo.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gzmwpsvxj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gexddmtfh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gcjctolpv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gdlinupmh.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/giwpuslcn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/glycelnfh.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gtxrhgibe.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/ggyokuylc.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gthasouii.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/ggcagzplu.sHtML

TS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gurqcbfvx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gsjuoafil.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gfeerislp.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gucgslmlc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gvhnulnss.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gdabkfogb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gesudrium.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gjilgybdn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gjtzgjvoa.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gzrytksqh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gbawomxvt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gdcdobung.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gogkzssnc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/grpiahvsg.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/goidcrbmc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gukbnwwgu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gqdymfwsi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgmzzocd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gytatulgk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gosqkpkgq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gbogmrsep.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/guuuooiis.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/grypxlmow.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gnpjdrosh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gybguimmv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/guboogjpj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/goctxyrka.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gorggbmep.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gunqhhmjy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gsipbxmte.sHtML


<!-- 参考信息 -->