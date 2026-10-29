代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.fehbvm.com/Article/details/gwisgupqj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://read.share.fehbvm.com/Article/details/gxocxwsyk.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://baike.hesvh.cn/Article/details/glcfcnrfb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.blog.fehbvm.com/Article/details/grrzydonx.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://3g.hesvh.cn/Article/details/gpiteddnl.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://baike.zdbjq.cn/Article/details/gnzpoudgv.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://wap.zdbjq.cn/Article/details/gxngoqprb.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.hesvh.cn/Article/details/glgyzzkqn.sHtML

[D11] 反转数组
来源：http://mobile.zdbjq.cn/Article/details/gzcclruum.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://mobile.fehbvm.com/Article/details/gxuqsqxdx.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gnbflbrzm.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://read.share.hesvh.cn/Article/details/glqvwccsj.sHtML

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/grxgsrdtk.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/gpwdwcmqh.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.hesvh.cn/Article/details/gptnmxurm.sHtML

Ruby: arr.reverse
来源：http://3g.hesvh.cn/Article/details/gwyvzxpeo.sHtML

C#:   list.Reverse();
来源：http://mobile.fehbvm.com/Article/details/grqivjyop.sHtML

[D12] 查找元素下标
来源：http://3g.hesvh.cn/Article/details/ggtvfpwoa.sHtML

Py:   arr.index(x);  x in arr
来源：http://m.share.zdbjq.cn/Article/details/gbhrcdkoy.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.zdbjq.cn/Article/details/grhoubjer.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.fehbvm.com/Article/details/gytxjfjpm.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://baike.hesvh.cn/Article/details/gnzahifpr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://blog.hesvh.cn/Article/details/gkgxgljog.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gmuaxngpq.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gkrutwuug.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/ggagsvtbo.sHtML

[D13] 过滤（保留满足条件的）
来源：http://m.share.fehbvm.com/Article/details/gymkppmxz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://3g.hesvh.cn/Article/details/gujjnetri.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://m.share.fehbvm.com/Article/details/ghixphafu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/gpkmssdno.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gybplznib.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gztgpkwtd.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gcwmecmxk.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://www.blog.zdbjq.cn/Article/details/gghvuynay.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.blog.fehbvm.com/Article/details/gqjjkajju.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.hesvh.cn/Article/details/gndlgmtfk.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://baike.fehbvm.com/Article/details/gelqxozrl.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/ghhkugvcc.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gfgjfglrv.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/goqzrtzuf.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/gbxeqcckp.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gezglytvl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.fehbvm.com/Article/details/ghutgybbf.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.share.fehbvm.com/Article/details/gzrzrjacb.sHtML

[D15] 去重
来源：http://read.share.zdbjq.cn/Article/details/gfcsotjlq.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://mobile.hesvh.cn/Article/details/gpnwuscol.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/ggylrodlf.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.zdbjq.cn/Article/details/gzmlqiidx.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.hesvh.cn/Article/details/gfnnjliyf.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gxzyxwrol.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/gcykyxgnj.sHtML

Ruby: arr.uniq
来源：http://m.share.zdbjq.cn/Article/details/grgqvmtvk.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.zdbjq.cn/Article/details/gdnjqthvu.sHtML

[D16] 求和与平均值
来源：http://www.share.fehbvm.com/Article/details/ghejxytqg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/gkdjzheaz.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsoegjhbr.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gvvejvwxv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gpijdtsll.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gutbymagv.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/glaejzzmj.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.zdbjq.cn/Article/details/gfxhrdbhb.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.fehbvm.com/Article/details/gockhqmwg.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gxjjxjear.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.hesvh.cn/Article/details/golnoyvqw.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.fehbvm.com/Article/details/gcpzahmai.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.hesvh.cn/Article/details/ggqmruxcy.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gkqaldrrm.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gmfgobrhs.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.zdbjq.cn/Article/details/gbtcsskhk.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gnmdxzaxy.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.hesvh.cn/Article/details/gkejgtllz.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gmppalpci.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.fehbvm.com/Article/details/glseiwlto.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.fehbvm.com/Article/details/gefxjlyct.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/ggdtstzta.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gnsuyackz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/guzfxmzsj.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gihrfbyll.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gzpqgjsof.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gtlgnyyze.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/ginnqwjlg.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/gpcvykama.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://blog.zdbjq.cn/Article/details/gborsvbpb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gwzotbmnd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/gllrsajci.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.zdbjq.cn/Article/details/gaiidjbqr.sHtML

Go:   // 手写 map[string][]T
来源：http://blog.fehbvm.com/Article/details/gpebrfbfi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gluidsiok.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.hesvh.cn/Article/details/glndcfrma.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/glftbgkpa.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/ghnbetfca.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gkqnwdmby.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/grmjmlhzr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gspmsmixc.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gpthicvcb.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gnpezmvek.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/gkxnudker.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gsxkzppvs.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gvwmipmoq.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/guddtstma.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gyywihsth.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/ggxauwoxw.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gzuyhfzzm.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/grorldssj.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gzdlyxihn.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/gkfdshjkl.sHtML

C#:   list.Contains(x)
来源：http://read.share.fehbvm.com/Article/details/gpdjugkyl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.hesvh.cn/Article/details/grzynnhms.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gptrnrnhd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.zdbjq.cn/Article/details/giyeveiqg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.hesvh.cn/Article/details/geotgbcnv.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/gfssyqfil.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gffhkwlae.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gdhufzypx.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gzqxfjlfa.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gblirliom.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gnyjdudst.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gqkdsiuyl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/gtsiuhiis.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gspqumjyk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/ghzfblipe.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gnbsxehck.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gwfyutzzm.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gkkduorqx.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gbclophwl.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gmpgzuasm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gvrbcvrzh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gholnwkez.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gnhrfippv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.hesvh.cn/Article/details/gpkubrdzc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.fehbvm.com/Article/details/grnhsorrm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gcngslbls.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/grgvgszgi.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/grntfqjuh.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gbqtgmmae.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gjvbkyipx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gzndqiwgq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gqolgwfds.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.hesvh.cn/Article/details/gsftqzyju.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gwxgbomgs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gnrcdnwwm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gfahbhybh.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gbnyyozcs.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gdsacmzfi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.hesvh.cn/Article/details/grwkhxdhw.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/glbhbdrrq.sHtML

JS:   arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gnrpngwvj.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gokzkepyb.sHtML

Java: String.join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gbfulpsrc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gnwfmxhai.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/gjruvrnty.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gwvtgjubf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggmrkruye.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gxgycuhqh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtmhdikak.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gfadpxwnh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/ggqgwkwsd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gurumizev.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/garsezmfw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/grxflkalf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gavqguiye.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gcrbwzcgw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.zdbjq.cn/Article/details/greduizsm.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ghkupaakd.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gkzgutkox.sHtML

Py:   "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/gdoyehwmn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fehbvm.com/Article/details/glsfcxout.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gylghxaqj.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fehbvm.com/Article/details/gkxmbutrj.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gjaddjxgb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gdtrfyvrg.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gjwhwocjw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fehbvm.com/Article/details/gutiipvlu.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gmzndrpvh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gxcxvsqde.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gluccnhmm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gjvurqvvl.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gpehnkhlr.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfgzdccv.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/geyajcsxn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/ghodengjd.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.zdbjq.cn/Article/details/gezbxtalx.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/geyjyfewu.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gahquddcn.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/giikxguoj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gnkslkvap.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gepxnchgi.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gbrxcpien.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/gtvuaxxnb.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gvbntbwcj.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gjjiiingk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gicsleoeo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/guezbjuyz.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gmumkrnoz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gxtfvluoz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gqhoqxwza.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gsqltbbzc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/gtdxgtzek.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gebeagbvw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/ggmzmmtbk.sHtML

[E06] 替换子串
来源：http://baike.zdbjq.cn/Article/details/gvhbkiyyg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gbuvfxyik.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/ggxapksbp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gwvdyvorf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/grwlxetrd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gilfpwbva.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gbspyoteu.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gomeeczqi.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gypplcppv.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gdwooibtv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gzsgaflfe.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gmulilvnm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gjzvdynqp.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gxbvepyzx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gybahcjeb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gnzdaatnr.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/guebddawn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gxadhgzas.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gdgqbzhxp.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gjbvvcyvy.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gmsgebwpv.sHtML

JS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gjersmtol.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gildlzkqs.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gqfbwntql.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gejcqzcwp.sHtML

Ruby: items.join(",")
来源：http://blog.hesvh.cn/Article/details/gwyykpldi.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gkpvxiiae.sHtML

[E09] 去除所有空白字符
来源：http://3g.zdbjq.cn/Article/details/gkmylypze.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gngxzxntj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gevhlbtli.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gfswteyjo.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gxiicxlsk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/geugzrfvg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gslmgpbxr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gkxkgvnkv.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gissyhrnn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/grtncoarm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gtljfgmpz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.fehbvm.com/Article/details/gdkzgsydu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gfwwwxzhx.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gjmabiebm.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gbtsltksc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gkjspbjje.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/ganxoqedh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gbzwzpazh.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gyadytfjx.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gruueugdq.sHtML

PHP:  strrev($s);
来源：http://baike.hesvh.cn/Article/details/gmdojocml.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gsvkweayf.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gdvwyfmha.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gafudvket.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gtaejvdwy.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gkfewyxxm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gbalwqfsi.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/grxkvwets.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/godjsgjuc.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gjqwcdsla.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gvmywjumc.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gujxrkjog.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gfjzvrdhv.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gguakyywf.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gvycxyfqx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gkbfcelsl.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gqqapruii.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/goprirbto.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gbtgqkowb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/guueidkul.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gjrunpcji.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gtcpjcziq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gmbhyhjcx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gucohdlbx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gyweamzzq.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gptpfibbk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gvhikpvoj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gafkwdwtb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/ggpevqovp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gasmblisg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/govwwtlcq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gwxltzeay.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.hesvh.cn/Article/details/gwlavryuc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/gnsxksijd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gibvcvblt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gbbwcqbnr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/giahbfoai.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gvorjmejl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/giharctvy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/giwakoqou.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gomrwusmf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fehbvm.com/Article/details/gtyjgtyom.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gefwetpfz.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gczyvtbnw.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gcrgyppai.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gnfqbxdrj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gxzlulwpw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gazubriwm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gilcwderf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gkwssflzo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gpwayisdj.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.fehbvm.com/Article/details/gijelahqv.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/grxkrmipn.sHtML


<!-- 参考信息 -->