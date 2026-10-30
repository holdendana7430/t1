代发 wailian999

PHP:  sort($arr);
来源：http://www.share.hesvh.cn/Article/details/gkncpeuwc.sHtML

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://m.share.fehbvm.com/Article/details/goczqfadc.sHtML

TS:   [...arr].sort((x, y) => x - y);
来源：http://3g.fehbvm.com/Article/details/gtgngeehi.sHtML

Java: Collections.sort(list);  list.sort(null);
来源：http://www.blog.hesvh.cn/Article/details/gigycrhbx.sHtML

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gcvzubdok.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/ggwefchmo.sHtML

C#:   list.Sort();
来源：http://blog.hesvh.cn/Article/details/grmxqvktn.sHtML

[D10] 自定义排序（按字段 / 多条件）
来源：http://3g.fehbvm.com/Article/details/gscsruxpn.sHtML

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://wap.hesvh.cn/Article/details/ghrijxuoy.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://mobile.fehbvm.com/Article/details/gtkrsunmr.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://wap.fehbvm.com/Article/details/gnjlgzhxv.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.share.hesvh.cn/Article/details/gurjqsbwb.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://baike.hesvh.cn/Article/details/gaajpvikk.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://m.share.hesvh.cn/Article/details/gcldutslc.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://read.share.zdbjq.cn/Article/details/geylvigvk.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://wap.zdbjq.cn/Article/details/gfslcyddt.sHtML

[D11] 反转数组
来源：http://www.share.fehbvm.com/Article/details/garmkqewd.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://read.share.fehbvm.com/Article/details/gvdglywcx.sHtML

PHP:  array_reverse($arr);
来源：http://www.share.hesvh.cn/Article/details/gomxosuzy.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://mobile.zdbjq.cn/Article/details/gjtehnlzw.sHtML

TS:   [...arr].reverse();
来源：http://read.share.fehbvm.com/Article/details/gaqaidurr.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gxkkmlfaw.sHtML

Go:   slices.Reverse(arr)
来源：http://blog.fehbvm.com/Article/details/gyvnlutol.sHtML

Ruby: arr.reverse
来源：http://www.share.zdbjq.cn/Article/details/gipaggfdm.sHtML

C#:   list.Reverse();
来源：http://wap.zdbjq.cn/Article/details/gzdcxvoqd.sHtML

[D12] 查找元素下标
来源：http://www.share.hesvh.cn/Article/details/gihceebod.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gzxwdinci.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gxynvoypp.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnvnnqdvo.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gmphypsfu.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.zdbjq.cn/Article/details/gadjwlsum.sHtML

Go:   slices.Index(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gztvsgxvo.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/gpppzwgjl.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gzlpagzzk.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/gvhbizbxe.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.fehbvm.com/Article/details/gbbkrsakc.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.hesvh.cn/Article/details/gltizsdav.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gxahluapl.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gmctlfauc.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://m.share.zdbjq.cn/Article/details/gdidkstbj.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://baike.zdbjq.cn/Article/details/gixzoclrp.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.fehbvm.com/Article/details/grriyqznz.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gkblywxjt.sHtML

[D14] 映射转换（每个元素变形）
来源：http://m.share.hesvh.cn/Article/details/gaiknqryr.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.blog.fehbvm.com/Article/details/gqsdqucoe.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://blog.zdbjq.cn/Article/details/ggrlrapfw.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.zdbjq.cn/Article/details/ghqkavwkr.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.hesvh.cn/Article/details/gbzxjqlno.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://mobile.hesvh.cn/Article/details/gfeihvwac.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gcyeyjkqu.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://m.share.hesvh.cn/Article/details/gvjqxtudi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/ggzcdazjh.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/gtppozohn.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gowjjurms.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/glceoyvnv.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gjiklnhwg.sHtML

TS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gmlubahqd.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gwqpbijbp.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/gdvaehzor.sHtML

Ruby: arr.uniq
来源：http://m.share.hesvh.cn/Article/details/gqlzakqhf.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/geukgtpdi.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/guvfcfljw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/ghjwfwkgf.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/guyzypqtc.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.zdbjq.cn/Article/details/ghiusnaes.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gjthsqtby.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.zdbjq.cn/Article/details/gvcfkfvoy.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gmkbxfqoz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://m.share.zdbjq.cn/Article/details/gqwbeekyc.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gchgridat.sHtML

[D17] 最大值与最小值
来源：http://www.share.hesvh.cn/Article/details/glrcopcce.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/gfxakuxjh.sHtML

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/ghlxyovhc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/guxzejcse.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gfkdauuay.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/gfuddmnmt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.zdbjq.cn/Article/details/ghabeutrb.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gbigqgmtb.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gdxibdozc.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.fehbvm.com/Article/details/giggokqaa.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.zdbjq.cn/Article/details/gonrsscjg.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gnfngclqn.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/ghgngvvop.sHtML

TS:   nested.flat();
来源：http://www.blog.hesvh.cn/Article/details/golosptcs.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.fehbvm.com/Article/details/gzustqfyj.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/goaqlsivj.sHtML

Ruby: nested.flatten
来源：http://mobile.fehbvm.com/Article/details/gxhlpzwpi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/gslszfdzb.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gvdxuzsts.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.fehbvm.com/Article/details/gccmtssjj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/gsfptvejp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gtkxtkvuh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/gbjlfdxdt.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.fehbvm.com/Article/details/gaszyxoqq.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/gohnyqmcr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gjthilize.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/geqmfrilr.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/geepzpikh.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gpwrogmjk.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gpshiiaxi.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gfxmluopr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gwgslhqfe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/giguzlofw.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gzfpbuxus.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gymbyscwr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/giwyjlrcc.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.hesvh.cn/Article/details/gpyywvsxk.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gpkjfwepx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gnhgyaich.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gfsvzyxbx.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gptwidvzc.sHtML

Java: list.contains(x)
来源：http://wap.fehbvm.com/Article/details/gtdhxkqzb.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gsxqwuibi.sHtML

Ruby: arr.include?(x)
来源：http://m.share.zdbjq.cn/Article/details/goildudpt.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gnkryojkb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gkyvsnywt.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.fehbvm.com/Article/details/grlfokfxz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.hesvh.cn/Article/details/ggmobcywk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/guybufgdr.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/guvvbermk.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gpmmixwsr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gtpiquugl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gnufsyfdv.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gkeusvbnd.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gysiatign.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gmvxwzqwt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/grljlsqvi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/glmkvocbp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/ggewmfzaa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gyqqgdkvm.sHtML

Go:   // 手写循环
来源：http://mobile.hesvh.cn/Article/details/glsdphhjz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.hesvh.cn/Article/details/gbzkpgqos.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gwjetbyms.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gxpkcmqdi.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gayrpodhp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/grmtiixou.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gyckagxzx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gwqnglyzf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gdbyllebz.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/ggrncwoul.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/glnmyolyz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/ggqrcfvju.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gumkjgxvl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gxoargead.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.zdbjq.cn/Article/details/gsraygfoc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.fehbvm.com/Article/details/gkrifynfy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gizqqlivx.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gykopwdvn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gvqupauee.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gyxsqwaxk.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gasxjtkby.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/govmsdouj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gnwzzirhe.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gnibebzas.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gjywztiix.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gyfmhwobk.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gppyrrdlg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gdozbnazh.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/ggndqwwfk.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gbkcqugum.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvqhcongt.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/goljmzgdl.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjxweunwq.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gvozknrfm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.hesvh.cn/Article/details/gwlwrjepj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/gsmhpomtw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/gciatbtkm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gvajctdzz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gsskhdoeo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gxcbhozck.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/ghqdlzwgz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.hesvh.cn/Article/details/gcmppgrnk.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gjukiixby.sHtML

Py:   "ab" * 3
来源：http://3g.hesvh.cn/Article/details/gmfizavgj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gopnnavvy.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gjoxjuawm.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gkkqzvchc.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/grbbgtnjh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/glryspqny.sHtML

Ruby: "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gaulhigyl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gemmmvydz.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/glwiyrgdh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/grxqsyxhh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gzsxnqyxx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gqanxamyn.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvjnrnej.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gioomfkam.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gpraqhbpa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gciqqwean.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/glflfprcn.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/giygpdbjt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gswqdwvsg.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gclawwpos.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gryyyoote.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gvaekeaoz.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gffohufoh.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gfcifyqgd.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gmrdssgsh.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gyxtlikwx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gbodyfadl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/grmbnjkal.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gbfbnugje.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gmnxfhhpx.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.fehbvm.com/Article/details/gylhjwnzz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gqdupvkcu.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.zdbjq.cn/Article/details/glzzzluak.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.zdbjq.cn/Article/details/gmvrklojn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gtyshzglm.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gqqhthfga.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/giuiiaicg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gfvtsfxwf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gmhdgchtd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfswjfrge.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gfozvfgql.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gjxobgzjz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gojuxescg.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gcjvpixcc.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gpilbucly.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gbtlxkobs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gyfjmyicy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gkciebbbx.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gssyqxssw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gxjoyazfk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gtypzweuu.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gqswggczj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/grsbzbwlm.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/gjqvygmto.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/glxooiwno.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gysnjqtmk.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gsfvmazlr.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gnxkmxjvw.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/goghhboom.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/ghgwbkoqx.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gevpqlpsa.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gvpfvrcjh.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/giieutwqn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gdwdyzwnl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjnclyrpj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gbgjbfvcm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gwsaicwpv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gcptwiecv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gqcvlvugg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gahreiwzl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/guragefzy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gvwxfmytz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gchgzvxup.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gvzjufjhl.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gqxzliczz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gvhidusqw.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gcuujltus.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gazwbxnzf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gaaknadzo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/groaixwru.sHtML

[E11] 反转字符串
来源：http://baike.zdbjq.cn/Article/details/gpgitowwk.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gryalqoyl.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gjeptyxti.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/ggjfrnoyo.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gernyqtip.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gesgcmmnu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/giedebvvy.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gaiewskve.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gqeddfjjw.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/ghwuvmoun.sHtML

Py:   s.count("a")
来源：http://baike.fehbvm.com/Article/details/ghqsdakfv.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.zdbjq.cn/Article/details/ggomzkxjg.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gagdogabn.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gblcgulaw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gdmpbnsja.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gglnovrcn.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gtemdvilq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gdftfmbfb.sHtML

[E13] 逐字符遍历
来源：http://baike.zdbjq.cn/Article/details/gskfjibtq.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gccedzpkb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gdblmdpwz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gbnxdqmph.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gpyebdram.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gslfpwjlg.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gaycifugq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.zdbjq.cn/Article/details/gnexckobj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/griebaxyx.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/giacvhejs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/guxzbhpgq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.zdbjq.cn/Article/details/gntbriwrt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gzetowrsw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gkxfjfupv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/ghadelzrr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gdqtgnquu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/glyklqsev.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gidfdrslu.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/gheurabli.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfawqwdzx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/geeikpvjd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gpetclbjp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gcapslwea.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gnwqyjlat.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gkdjmilmn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/gqayxejjr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gkpilprwz.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/grwdcetxp.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/ghsctucjt.sHtML


<!-- 参考信息 -->