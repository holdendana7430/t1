代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://read.share.zdbjq.cn/Article/details/ggzzqfumj.sHtML

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://3g.hesvh.cn/Article/details/gtthhozlw.sHtML

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://www.m.share.hesvh.cn/Article/details/geppkommb.sHtML

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://3g.fehbvm.com/Article/details/gpjiyoxps.sHtML

Java: list.sort(Comparator.comparing(Person::age));
来源：http://mobile.fehbvm.com/Article/details/gshvcprnx.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://3g.zdbjq.cn/Article/details/ggzmibkbl.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://m.share.fehbvm.com/Article/details/gdawymvtp.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://blog.fehbvm.com/Article/details/goxwyykml.sHtML

[D11] 反转数组
来源：http://baike.zdbjq.cn/Article/details/gfxgvyvjq.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.hesvh.cn/Article/details/gyrrtjgqj.sHtML

PHP:  array_reverse($arr);
来源：http://mobile.zdbjq.cn/Article/details/gkollcqlc.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.zdbjq.cn/Article/details/gvmhaxrsg.sHtML

TS:   [...arr].reverse();
来源：http://baike.zdbjq.cn/Article/details/gtvwwdkha.sHtML

Java: Collections.reverse(list);
来源：http://www.share.zdbjq.cn/Article/details/gjaratnop.sHtML

Go:   slices.Reverse(arr)
来源：http://www.share.zdbjq.cn/Article/details/gihbihtio.sHtML

Ruby: arr.reverse
来源：http://www.share.hesvh.cn/Article/details/gwrvefyta.sHtML

C#:   list.Reverse();
来源：http://m.share.zdbjq.cn/Article/details/gmamhhlki.sHtML

[D12] 查找元素下标
来源：http://3g.fehbvm.com/Article/details/gtwmsukgs.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.blog.fehbvm.com/Article/details/gvappqcaz.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.zdbjq.cn/Article/details/gscznmrpq.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/ghszpidsl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.hesvh.cn/Article/details/gqzojrtbq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://read.share.hesvh.cn/Article/details/goviycqel.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gttjbqehw.sHtML

Ruby: arr.index(x)
来源：http://3g.fehbvm.com/Article/details/gztjbngil.sHtML

C#:   list.IndexOf(x);
来源：http://www.share.zdbjq.cn/Article/details/gpzijuaqm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.fehbvm.com/Article/details/gerwocgit.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.fehbvm.com/Article/details/givdgjpbl.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.fehbvm.com/Article/details/gkiwczyex.sHtML

JS:   arr.filter(x => x > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gpvfkwvae.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.hesvh.cn/Article/details/gmasbkyvt.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://mobile.zdbjq.cn/Article/details/golncjdjl.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gkmgpofjj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://3g.hesvh.cn/Article/details/gozihqkgj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.zdbjq.cn/Article/details/gxxyyinbh.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gguyuchnj.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://blog.fehbvm.com/Article/details/gexkdvlsg.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://baike.zdbjq.cn/Article/details/gopnkcjtn.sHtML

JS:   arr.map(x => x * 2)
来源：http://read.share.fehbvm.com/Article/details/gmwmgyqrr.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.fehbvm.com/Article/details/gwxeynlcu.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://wap.zdbjq.cn/Article/details/gdgzkijtr.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/grybfyghk.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gdbxfeknh.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gmlwbphjh.sHtML

[D15] 去重
来源：http://www.m.share.fehbvm.com/Article/details/gemkfjtae.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gylvcxzlr.sHtML

PHP:  array_unique($arr);
来源：http://blog.zdbjq.cn/Article/details/gjbdkvqnc.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gmybfppxz.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.fehbvm.com/Article/details/gruetdqdu.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.hesvh.cn/Article/details/gnqghmdes.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.m.share.fehbvm.com/Article/details/geucvvvad.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gdxvcmdzj.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.fehbvm.com/Article/details/gjaczggmi.sHtML

[D16] 求和与平均值
来源：http://wap.hesvh.cn/Article/details/gwkdftacj.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/gfwfevaea.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/godwwekmk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/ggfjmusiw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/gjpbwuzqy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.blog.zdbjq.cn/Article/details/gftkqdlbf.sHtML

Go:   // 手写循环累加
来源：http://read.share.fehbvm.com/Article/details/grjdomoiy.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.zdbjq.cn/Article/details/gbozudqzy.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/gzkvydkle.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gmatqyubv.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.hesvh.cn/Article/details/gtvwkparf.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.hesvh.cn/Article/details/gkzzlnnou.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://read.share.fehbvm.com/Article/details/gcvhfdsbj.sHtML

TS:   Math.max(...arr);
来源：http://wap.hesvh.cn/Article/details/gaalutwrw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.zdbjq.cn/Article/details/guqvplodq.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gwpxygvbj.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.zdbjq.cn/Article/details/gwlfvwuds.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/gellkpupo.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/goseeviom.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gywqejcep.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gvjjpjtjx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gfcyvpzcf.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gbkwmvbia.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/grdlaxbqf.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/glturzkgj.sHtML

Ruby: nested.flatten
来源：http://baike.hesvh.cn/Article/details/gjxeueytm.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.zdbjq.cn/Article/details/gzoabxlkh.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/gcolfqwxb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gfkaccock.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/gvkudczkz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gomgzldkp.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gwkyvkofb.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gsasnbjic.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gjmlxwdre.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gxphetmyq.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.zdbjq.cn/Article/details/gzqcrhcab.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gxvllymxs.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gmeaqwmzb.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gdwzgqxfc.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.fehbvm.com/Article/details/gihafsvii.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gnazcvict.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gezlqvcao.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gqswmukvr.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/guducsmxg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/giwbtujoj.sHtML

[D21] 判断是否包含某元素
来源：http://wap.fehbvm.com/Article/details/gasanfmtw.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/goxqfomqk.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.hesvh.cn/Article/details/gkrchvneq.sHtML

JS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/glzggwipl.sHtML

TS:   arr.includes(x)
来源：http://www.share.fehbvm.com/Article/details/guvktjknz.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/goawrujow.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gintxixwa.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gqnexscrz.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/grwbhqrqw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/gwnshfrgv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/ggwpxrjob.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gbphoktai.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gyfsbpfkp.sHtML

TS:   [...arr];
来源：http://m.share.hesvh.cn/Article/details/gliciuerb.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gwaamsmio.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.zdbjq.cn/Article/details/gbolvpqyj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gegfxghtg.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gzzxzfvmr.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/guywhekuu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gdtdxygib.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/gfplrkhos.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gkbcdlsdw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gvvwjisrl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gyshqpciz.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/guiwkvyju.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/guxzhvhvd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gqnaknscu.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.fehbvm.com/Article/details/ghlfiqvyt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/gkmhlvwfw.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gxbhkaxbj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.blog.fehbvm.com/Article/details/gufkzljwp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.hesvh.cn/Article/details/guvkiaxyg.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fehbvm.com/Article/details/gmadomtzw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://wap.fehbvm.com/Article/details/gxwtazwfk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gqoceslap.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gxvtnwshg.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gwoylwgsc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/geeeuljkw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gqpjwglbl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gveyemvap.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.zdbjq.cn/Article/details/gukgfsflc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gsxaauarw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gmckkjkpn.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gnbmrrywl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gziiorbny.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gaqlpsmqv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.zdbjq.cn/Article/details/gazrhhfja.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gezzfdmey.sHtML

JS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gvszwomuh.sHtML

TS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gtbkvdukf.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/ggkkykqcd.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gzrjexiax.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/guxrnrfcz.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/ggfismesb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnxrjsyah.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gmlhchsmm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gatqcbxig.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gomthizxq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gwefgcbyr.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/ghpnlrtcg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/golxclnck.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gueklekvx.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gttutzmqn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/grwtxhtyj.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.hesvh.cn/Article/details/gibtwvgdp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gcplzxgti.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gxbfqfney.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gdnqszani.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.zdbjq.cn/Article/details/geojxgymd.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gladddvmh.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gtoqljuoy.sHtML

Java: "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ghayiuzeu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.hesvh.cn/Article/details/gmikdjrim.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gssyxxbvq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.zdbjq.cn/Article/details/gnmhmvblh.sHtML

[E03] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/ggqpfafub.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.hesvh.cn/Article/details/geuyolepr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gvoghvdbm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/ghisgqubx.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gxsgugbhs.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gfibnyzku.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gzljosoev.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gifjbpprd.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gnaopblpr.sHtML

[E04] 查找子串位置
来源：http://baike.zdbjq.cn/Article/details/gmklcjnlg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gvusvpahx.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gzstykoyj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gputulgcm.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/ghrdvqtmm.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gpxevvkhe.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gikdwcwjo.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/gddjscdrj.sHtML

C#:   s.IndexOf("x")
来源：http://3g.fehbvm.com/Article/details/gsrokjuyv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gfthtxwvi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gigvlusxx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gpgfaycel.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gaqsxfabt.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/gmzelvvwk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gszmjdgit.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gfjewauem.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gjoozsnfo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gggbulrut.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/goadpwylj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gdmlpbmzw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gmmngwnsm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gtmomyrlp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gyybrxahp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gyskarlej.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gxvfcaexs.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ghkrlkkiv.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/getxzuwhf.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gxqdwvbeq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gdpefyzdc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.zdbjq.cn/Article/details/gmambrort.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gkwigrpvi.sHtML

TS:   s.split(",")
来源：http://www.blog.zdbjq.cn/Article/details/gsbfyhxay.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.hesvh.cn/Article/details/ghjfdggeh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.hesvh.cn/Article/details/ggssytevo.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gakvfpckp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gplfoqfsd.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gbquzxxfm.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/goyldjvwz.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/ggumskyia.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gagdsdwez.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gvcigtbfh.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gurbiqqhv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gshxbekzr.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/ggmdmftbc.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gbqxsermk.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gjwhqrklq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gqyzchjkg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gwveyzoyt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/ghabgfmlr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gnuhlbnjp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gtypojezr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/grtlwgoyh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/glqaywtwn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gzqrhwtoh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gxiwqgyxt.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gipkesdtp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gqwfczuex.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gjwrpckms.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gscqnilfz.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/ggidywefb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gpdcvrwbb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gwzcapqde.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/gddsemngh.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/grslobtaw.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/ggfjtwoka.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gkoxywhts.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gshpamftv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gvsquhbta.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/greistqho.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gvmozxbsd.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gynvzvwil.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gtwpmfwqs.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gipgqvuze.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/getuylyve.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gvxcmzzlo.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gncshqbnt.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gwxmjmgcd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gzuyoeafk.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gdrsabfcl.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/glhmggxcx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/ghcrjorql.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gzpcfmqvu.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gqbffwwzb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/ghcnntbff.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/geqholwkj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gduaisbiv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gckyoovif.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/gnyskjdsn.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gemzougea.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gudmsocss.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/geuvjsxpd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gfeandcxz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gnzxyyfzn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.zdbjq.cn/Article/details/gioalueup.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gqfhaamjh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gofrkigll.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gtrdzdxez.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gohxsjbye.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/grwkbvqsc.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/grwmycesh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gqffmghxk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gvvqymsvd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/grabazqdz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gpkkilrtc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gifvnjpwa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gcergysut.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gmapydllx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/garkdzvwn.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gqeljmkbf.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gedgmgsxv.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gqniuwjxr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gkxbqrpvd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gkshxlulw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gygguhsct.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/grzyrmatm.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gjkacyxep.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gvhvszrto.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gkbayxslg.sHtML


<!-- 参考信息 -->