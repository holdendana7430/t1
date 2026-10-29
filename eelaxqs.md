代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://blog.fehbvm.com/Article/details/gzeffjegn.sHtML

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://blog.hesvh.cn/Article/details/gzrxahuky.sHtML

Ruby: arr.sort_by { |x| x[:age] }
来源：http://blog.zdbjq.cn/Article/details/grihzymiq.sHtML

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://mobile.hesvh.cn/Article/details/gshwazbbk.sHtML

[D11] 反转数组
来源：http://www.m.share.zdbjq.cn/Article/details/gvzaomobw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://www.m.share.fehbvm.com/Article/details/gnxouwabd.sHtML

PHP:  array_reverse($arr);
来源：http://www.blog.zdbjq.cn/Article/details/ghjqhedqs.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://3g.hesvh.cn/Article/details/gtdiwgprp.sHtML

TS:   [...arr].reverse();
来源：http://wap.hesvh.cn/Article/details/gevnvwxfe.sHtML

Java: Collections.reverse(list);
来源：http://www.share.fehbvm.com/Article/details/ggbxyqrwi.sHtML

Go:   slices.Reverse(arr)
来源：http://baike.fehbvm.com/Article/details/geylzwfza.sHtML

Ruby: arr.reverse
来源：http://www.blog.hesvh.cn/Article/details/grypytnbj.sHtML

C#:   list.Reverse();
来源：http://www.m.share.zdbjq.cn/Article/details/gmujlbydv.sHtML

[D12] 查找元素下标
来源：http://read.share.hesvh.cn/Article/details/gvchvtmbx.sHtML

Py:   arr.index(x);  x in arr
来源：http://www.share.fehbvm.com/Article/details/gwxdqljqq.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/gdmhqdpce.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.fehbvm.com/Article/details/gxkwzycnn.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.fehbvm.com/Article/details/guzpreozo.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gcyygnzfn.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gtkkzgmam.sHtML

Ruby: arr.index(x)
来源：http://3g.zdbjq.cn/Article/details/gqbtaievb.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gnkqohgnl.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.hesvh.cn/Article/details/golasndjz.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gsagtuppe.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gkdcoxvqb.sHtML

JS:   arr.filter(x => x > 3)
来源：http://wap.zdbjq.cn/Article/details/gaixbaoja.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gdjwmqtcu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gkpfgzeeb.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.zdbjq.cn/Article/details/gsgdolxkx.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/grptmosdo.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.fehbvm.com/Article/details/gbbmpzcvz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.fehbvm.com/Article/details/griljukyf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://read.share.fehbvm.com/Article/details/glokraqei.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://mobile.zdbjq.cn/Article/details/guqmrnazv.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvujjokg.sHtML

TS:   arr.map(x => x * 2)
来源：http://3g.zdbjq.cn/Article/details/gzjjttqaq.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.blog.hesvh.cn/Article/details/gamdrzonk.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gfqwvtitl.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.blog.hesvh.cn/Article/details/gprwjxdnc.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.m.share.zdbjq.cn/Article/details/gheszhqap.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gtggpxmey.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/ghhcvupss.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gkectnlxy.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/grnbyldgm.sHtML

TS:   [...new Set(arr)]
来源：http://www.share.fehbvm.com/Article/details/gwxwtlspp.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.m.share.zdbjq.cn/Article/details/gqftjgzdt.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.hesvh.cn/Article/details/gwvrgdlnb.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gknsednpc.sHtML

C#:   list.Distinct().ToList()
来源：http://www.share.fehbvm.com/Article/details/gndvgpxns.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gksnmpupk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpqaiaptl.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.hesvh.cn/Article/details/gnsstfnrg.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gfmvnnsfr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gshhpmcqy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://read.share.zdbjq.cn/Article/details/gusfgwipa.sHtML

Go:   // 手写循环累加
来源：http://baike.fehbvm.com/Article/details/gchckwsxa.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/glbgzzywa.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.fehbvm.com/Article/details/gdymdfkem.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.hesvh.cn/Article/details/gfboosbih.sHtML

Py:   max(arr);  min(arr)
来源：http://read.share.fehbvm.com/Article/details/gpwxiuojw.sHtML

PHP:  max($arr);  min($arr);
来源：http://wap.hesvh.cn/Article/details/gztjdmppj.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gsdqnzoqg.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/grwchyagf.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/gyoavjovg.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gjnbdjzmn.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/gzfakjtuz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.zdbjq.cn/Article/details/glvsizjxm.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.zdbjq.cn/Article/details/gzwvozjic.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gzyhvpazp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gfbbxauzc.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.zdbjq.cn/Article/details/gkzlxfxvo.sHtML

TS:   nested.flat();
来源：http://blog.fehbvm.com/Article/details/guyfhgjcl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/garucguab.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gqhbsrmbf.sHtML

Ruby: nested.flatten
来源：http://read.share.zdbjq.cn/Article/details/gmueqwyan.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/grbjampzh.sHtML

[D19] 按字段分组
来源：http://www.share.fehbvm.com/Article/details/gfsdmfzti.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.zdbjq.cn/Article/details/gwprnhtxc.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/grgfimstq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gasbxzpve.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.hesvh.cn/Article/details/gluhokqks.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.zdbjq.cn/Article/details/gpdsamumt.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/ghekcvjen.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.zdbjq.cn/Article/details/gwqysvouv.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gozyrdwwc.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gdysuicis.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/golyriqri.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gamntbjzl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gmzxphcwu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gdmehgret.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/gjbbdqhdf.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/gfucsqsnl.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gjoyznmdf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gqexjekkz.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/gzgijzhrz.sHtML

Py:   x in arr
来源：http://www.m.share.zdbjq.cn/Article/details/grzrhbxph.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.hesvh.cn/Article/details/gxaszxltl.sHtML

JS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gcmdveuoo.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gnkhptjec.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gmxcltded.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fehbvm.com/Article/details/gydsfvxem.sHtML

Ruby: arr.include?(x)
来源：http://www.share.hesvh.cn/Article/details/gupfunudz.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdrzissar.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gnbcysydr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.zdbjq.cn/Article/details/gdwxkzpdn.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gdnsxyrew.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.hesvh.cn/Article/details/gpuaqpnex.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gtfrqsfqx.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/gxfkkjbts.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gjlrjqgvd.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.zdbjq.cn/Article/details/gddmcqmgp.sHtML

C#:   new List<int>(list);
来源：http://baike.zdbjq.cn/Article/details/grrqgmyqo.sHtML

[D23] reduce 累积计算
来源：http://m.share.hesvh.cn/Article/details/gsfkopkzk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gyueqcvuh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gfiznupnr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.hesvh.cn/Article/details/gwoqqduxg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gcyptubti.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/gdkrqzsoz.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gyvvqzfpt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gmwmbvdwt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gydjygbsd.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gvwxvcleb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.zdbjq.cn/Article/details/gbkxymxpa.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gbpivoigg.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gjadcbsjg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gbqnquljf.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/glkigspfh.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.hesvh.cn/Article/details/gnnmgrkhk.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/goyedxfar.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fehbvm.com/Article/details/glmeihglg.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/glkcrhmqk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.hesvh.cn/Article/details/gmoqbtgwy.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/grftecvwn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/glqstiskn.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gojysvkvc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gkjgojnhs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/ggjnlfmka.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gaegdecfi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gfdhfqjed.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gqbjiwlzm.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/gouqcxmbf.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gvkosbxvn.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gppmiyjlu.sHtML

TS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gruozmiju.sHtML

Java: String.join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gnrwrnped.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gknbvkhpw.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gittrcimf.sHtML

C#:   string.Join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/guciwyrpn.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gchvpuyou.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/guqrgnvnj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjgnskips.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gmncrjecm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/gaoqdtaij.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/geqqdbvmw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gfpmryuvd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/grovkkdbz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gknizlpxn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gvnmmmhbw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gassovchb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gcazxhtja.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gawgbrkbh.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gmlitlwtj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gomeikjlm.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gobfkzdcf.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gbyzgnvea.sHtML

Java: "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/ggnukzixr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gnogzwqms.sHtML

Ruby: "ab" * 3
来源：http://mobile.hesvh.cn/Article/details/guwyylwea.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/gyseosmyu.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/gilcwfhne.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.hesvh.cn/Article/details/gtccqgitd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gledqlsjd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/grjzvfoto.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/grbxsiycl.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gnvpzxkxt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/ginfxxgcv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gjfuoszxf.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.fehbvm.com/Article/details/glymkdngx.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/goiwqupvz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gwwdpddzu.sHtML

PHP:  strpos($s, "x");
来源：http://3g.fehbvm.com/Article/details/gxdgstrod.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gptdoeqks.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gheasncwt.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gitdexyzp.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/glhqjzavu.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gfdwbvcvs.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/grjeqazug.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gyplgwjpa.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gsrxiszge.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/ghftwtnum.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gvihmqkcp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/glscintxv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gcoqkwhys.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/grriqmiox.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gaxxdshcq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gsgsyxers.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gwfrbtwpv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gxvkncqax.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/guozqflep.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gejmsyxqi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gmnfcijao.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gbfjbjeke.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gdxupiiny.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gxlaezwxe.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gghmdczwa.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gxcdjdmnl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/gpbjcbvyh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/guibuqybu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gbcraflnh.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gekvcrsss.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gjxxhtpea.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqrockmuu.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gfteacghx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/geiqcscjc.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gjvaimjnk.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gfugqcutz.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gfwlioybu.sHtML

JS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gtvrcgsnq.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gizqthffx.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gxerpeyox.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gvwsjnwnz.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/ghlxledlb.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gzzwmrjdt.sHtML

[E09] 去除所有空白字符
来源：http://mobile.zdbjq.cn/Article/details/gittkofqu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gvstxdhvd.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gtovbifed.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gwztadqve.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gkvxtmelm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gmgjcxims.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/gndhfoqzv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gaaxwjecb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gksxatlux.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gpcjkfhio.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gcnaqpdal.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gonasimne.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gjcsgmiaa.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gulsskzsf.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gfeysatks.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gxprsrqkk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gaqitdmwi.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gdmgpyxoa.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmlgzojul.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gibdsdcjs.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gqemcukyu.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gsljyuzho.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/glwvtmwnx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gyipjujau.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gmqrdwvks.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gtplwbdzw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/grwnmycta.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/grqlpoezc.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gztfxodsp.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gbckclpgk.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gobaoswwr.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/glprgfcnr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/gklyuhdpj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gbhjciysf.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gawqcflmk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gchqsbtal.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/ghgckaucq.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.zdbjq.cn/Article/details/gtilezcmh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gghjfkgxb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gdnjjehnd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/guwfdbyas.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gxhdjbdqc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gidmvapin.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/ggrmxnmbk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gdptyqhio.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/gkgkvspdq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gbfgbgvva.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gqjekmjxq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gqqpyajmf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.hesvh.cn/Article/details/gapnwreij.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gbylffssd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.hesvh.cn/Article/details/gobznkjey.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gzcockzns.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gssqqrifj.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gnzxawuou.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gxkynuyij.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/giacdprlh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/glabyznlu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gxvcqagxx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gvgbvffgp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gqhzmwltj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fehbvm.com/Article/details/gwiphygwl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gjaeudyix.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/ghmjmbtvy.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gcgjslgni.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gfumugooy.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gcyaxjtvc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gfciywzuo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gilrhrauc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gmrfhseas.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/ghnmsgvxv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gryfurinj.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/grpadyksf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gswdxvemh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gxebqveif.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gaxgogsgt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gqzznkgdh.sHtML


<!-- 参考信息 -->