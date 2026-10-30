代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://m.share.hesvh.cn/Article/details/gcdhrztal.sHtML

C#:   a.Concat(b).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gwcufoiel.sHtML

[D09] 排序（升序）
来源：http://www.blog.fehbvm.com/Article/details/gviirqdgq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/govbcfcmg.sHtML

PHP:  sort($arr);
来源：http://www.blog.zdbjq.cn/Article/details/giemgwrel.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://www.blog.hesvh.cn/Article/details/gdqphqlkf.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://m.share.hesvh.cn/Article/details/ghktpaymb.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://mobile.fehbvm.com/Article/details/gthfdjtnw.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gwchhghsn.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gooeaqymz.sHtML

C#:   list.Sort();
来源：http://www.blog.fehbvm.com/Article/details/gcuqjiwxg.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://wap.zdbjq.cn/Article/details/ghfxoxfso.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://www.blog.hesvh.cn/Article/details/gaskgnvrf.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.zdbjq.cn/Article/details/gaozvxuzv.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.zdbjq.cn/Article/details/gvatnnxwc.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gqhnsuxxf.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://www.share.fehbvm.com/Article/details/gctqreaxw.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://www.share.zdbjq.cn/Article/details/gpthnznry.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://mobile.zdbjq.cn/Article/details/gmkqlozpo.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.zdbjq.cn/Article/details/gvegbsriv.sHtML

[D11] 反转数组
来源：http://www.blog.fehbvm.com/Article/details/gtyizoehu.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.zdbjq.cn/Article/details/gcyolxjnw.sHtML

PHP:  array_reverse($arr);
来源：http://read.share.fehbvm.com/Article/details/gcyrlzuzs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/gmszbpbgo.sHtML

TS:   [...arr].reverse();
来源：http://blog.zdbjq.cn/Article/details/gnvloqteo.sHtML

Java: Collections.reverse(list);
来源：http://www.m.share.hesvh.cn/Article/details/gfjvakeak.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/gofzdyvvk.sHtML

Ruby: arr.reverse
来源：http://m.share.zdbjq.cn/Article/details/gmxbksppr.sHtML

C#:   list.Reverse();
来源：http://m.share.hesvh.cn/Article/details/gwundyfgo.sHtML

[D12] 查找元素下标
来源：http://www.m.share.fehbvm.com/Article/details/gzmsmptvj.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.zdbjq.cn/Article/details/grzsksfru.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.blog.fehbvm.com/Article/details/gqcgdhyvm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gqoiuazkd.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gxnwzymba.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.hesvh.cn/Article/details/gawtzkdsf.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gaiaiapgs.sHtML

Ruby: arr.index(x)
来源：http://mobile.hesvh.cn/Article/details/gqwfxrnyo.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gzxnamohk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gniordhkn.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://mobile.fehbvm.com/Article/details/gntbznqxp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.share.hesvh.cn/Article/details/gdigddmto.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.fehbvm.com/Article/details/ggcvxnscg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gdfnsmfro.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.fehbvm.com/Article/details/gchsqkkds.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.zdbjq.cn/Article/details/gmrqkskzz.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gthxkzolz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.zdbjq.cn/Article/details/gsiqnracj.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/ghqhixspd.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gihiretvw.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gbobihvqb.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gjyeislah.sHtML

TS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/geraxcywq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/ghxyxptxg.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gzfvtqiuc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gghvgjubd.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.hesvh.cn/Article/details/ggowqfwvc.sHtML

[D15] 去重
来源：http://www.m.share.hesvh.cn/Article/details/ghtwpouba.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/guzdnrulz.sHtML

PHP:  array_unique($arr);
来源：http://read.share.zdbjq.cn/Article/details/gehtytcxd.sHtML

JS:   [...new Set(arr)]
来源：http://mobile.fehbvm.com/Article/details/ganqdsixq.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/grfpxspvj.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/grgfmmtpu.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gsdzddmfm.sHtML

Ruby: arr.uniq
来源：http://www.share.fehbvm.com/Article/details/gutouxuoe.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.hesvh.cn/Article/details/gwxadblhv.sHtML

[D16] 求和与平均值
来源：http://read.share.zdbjq.cn/Article/details/goouvysqm.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdwljaoog.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.zdbjq.cn/Article/details/gswbckjzl.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gwiwaijvo.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gdgtzmrac.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/gxzqdkshn.sHtML

Go:   // 手写循环累加
来源：http://3g.zdbjq.cn/Article/details/gfcxuytds.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.hesvh.cn/Article/details/gsjalcjhs.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.hesvh.cn/Article/details/gbrkwhtcc.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gostuccqv.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.zdbjq.cn/Article/details/gzyajjbew.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.fehbvm.com/Article/details/guvslthge.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.hesvh.cn/Article/details/gazhbyxii.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/gjcaksmiy.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.zdbjq.cn/Article/details/gfaeplcac.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.fehbvm.com/Article/details/gzzyppmto.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gczncrunt.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/gynesegzh.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/guybsxgnl.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gpqrwofej.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.zdbjq.cn/Article/details/gpsrnozpf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.zdbjq.cn/Article/details/gixvdecek.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/giqlvcpgl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gvikeqdln.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gnwbfezyp.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gtmtqxdtq.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gwjylbpfy.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/glzynfwba.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.zdbjq.cn/Article/details/gamjzhyia.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.fehbvm.com/Article/details/gqlbyykkv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gcuafnbzy.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gcwmgpcvi.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gphzfiopq.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gsncpqmcg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.hesvh.cn/Article/details/goimaseup.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gxaacbspn.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gliygjhyh.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gkaooyinw.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.zdbjq.cn/Article/details/gremwlhsv.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gihlryeay.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/guzwwqxzi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gjxrdrguf.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gxwuxvpda.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/grxanvjby.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gueloiodf.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gmhiotjxd.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gjclnzsbo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gnpnepbhb.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/glrddhnsh.sHtML

TS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gykinakke.sHtML

Java: list.contains(x)
来源：http://mobile.hesvh.cn/Article/details/gixucgjbm.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gvahzjhrv.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/gtborywxo.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/givdrqwsk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gdsuixvab.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gytssclgw.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gmtjbrtyi.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gvrntpbto.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/glmofynib.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/ghtptchmh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gfyogtpax.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gyobaedok.sHtML

C#:   new List<int>(list);
来源：http://mobile.hesvh.cn/Article/details/gjahiaomz.sHtML

[D23] reduce 累积计算
来源：http://blog.zdbjq.cn/Article/details/goxxgeztc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.fehbvm.com/Article/details/gbceayodv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/ggotfvsku.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjqutpkt.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gebypypdo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gpajcvzho.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gaawzcgbj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gslvjqbkj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.hesvh.cn/Article/details/gvpvqckgs.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gvlhnjixd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.hesvh.cn/Article/details/gxmecfywl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gcsrjdokl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fehbvm.com/Article/details/giprsjmwg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gdilasaph.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gfnfxjmqt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gyqftqecp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gvawrvfql.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/gtqwokhet.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gehetuojc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gdgraaiua.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gxwxcqahz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/ghcfidprb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/grlafdwdd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gdwmittxb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gvxafqiem.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gxlggliay.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.zdbjq.cn/Article/details/gdxjqidbz.sHtML

[D26] 数组转字符串
来源：http://www.blog.zdbjq.cn/Article/details/ghijrecod.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/glhkrdzgo.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gqudgbskz.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gscfryxar.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gstwotnpd.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gnawhhrqt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gzvzcvrsi.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/glxuhhdox.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gmcpwxklu.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gsmnuisix.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gtdjpmnbg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdsiyedgu.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gajbruade.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/giigxyjhg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/gohtmiien.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/geybdwnua.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gkvvlalrr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.fehbvm.com/Article/details/gstibhore.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gbbkycyan.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gxugagmbx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gdwbhdlwn.sHtML

[E02] 重复字符串
来源：http://3g.hesvh.cn/Article/details/gyqzszdyn.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gifwamtpm.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gpukkuhtf.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/ggeemwkye.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gtjaovlxg.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gfzpzwhil.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gpdmozwux.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gepdsrzvg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gpqsuqysj.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/ggfgurfxm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/ghltgzszm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gjmpwfjtb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gprhnkjqv.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/gfgjtgjtn.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gbxvtdehv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gpkrwctru.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gclxisnqv.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gtzklexmx.sHtML

[E04] 查找子串位置
来源：http://wap.zdbjq.cn/Article/details/gexyfjoow.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/grixdfrhv.sHtML

PHP:  strpos($s, "x");
来源：http://wap.zdbjq.cn/Article/details/galwescam.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gguetozdo.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gsgmutsbw.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gegvjedpy.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/ggmukjefv.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gmkneobmx.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gknpxiwaf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gkwimjhvx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/ggukjhpfl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/gjscrooyo.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gnobcjhti.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/ghhordzan.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gasxnfcsx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/grysjdeen.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/gktlrqmro.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gsxxodvmf.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gxkgthilc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gizruohou.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gzhjjpizw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gmsuiybao.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gcdbkzrxu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/ghpinircd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/govnfrvia.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gvyjicmwe.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gjvgfdytn.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gzppwywsb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gbocygrir.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gnxzodgym.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/ghfkfyfnf.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/geztprjbn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gykdameiv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/gwmkrnkjx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gdtxcqewr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gqiphhhun.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gbvkzkcpj.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/giwcayoth.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gamttxsdc.sHtML

JS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/ghbnvvdrs.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/ghffmkzdq.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gdvrsiwpb.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gfznvuagx.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gspvpfozb.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/ggjvhxzpn.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gbwinxhuc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gucufvclx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/gdbhameuk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gihezkqyk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gztudtwib.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gjaxswiqs.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gdcmjubff.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/grwhejrmh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gtbvwhgdn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gxmnctltg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gdvowajce.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gdetfhtey.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/givvpijej.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/getsasuzk.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gwwfblxwl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gyzgoaicr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/guxcwnvgs.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/guutawnwb.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/gksoxzuqf.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gowdytdjf.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/goblooavc.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gchgqheby.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghenyhpjv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gdodphdsi.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gdecfrwpg.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gupbpxbzl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gwdxuspua.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gbznhipdb.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/goyiaclmo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gpqzgxzxl.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gcfiomzdv.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gwbzpfwjb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gbnhegugo.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gxjpkpdke.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gwltkrkok.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gqgbckail.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gewcbxtnr.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gaivlaicr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/grgmyffjp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gjwzrmfvy.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gdiitwocl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gfilcaojz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gqdelmtzt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/grlnkbnvt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gjaqfojyb.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/geshjmnrv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gowyluxrs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gclpakbry.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gnoflfjdn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gtvhcrkbx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/ghopahysn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gueplsqgu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gjsmbiwpq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/glxupvmlq.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gcsvbgkjq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/girnhvccs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gwncwqizn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/guuxivqcn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/ghnqwpozy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gdmfprqpw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/ggrqeizvx.sHtML


<!-- 参考信息 -->