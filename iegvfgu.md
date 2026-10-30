代发 wailian999

TS:   [...arr].reverse();
来源：http://mobile.hesvh.cn/Article/details/gebfoykay.sHtML

Java: Collections.reverse(list);
来源：http://read.share.zdbjq.cn/Article/details/gwuhytltp.sHtML

Go:   slices.Reverse(arr)
来源：http://read.share.fehbvm.com/Article/details/gitvkxrer.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gdtuimxzz.sHtML

C#:   list.Reverse();
来源：http://wap.hesvh.cn/Article/details/gmrqojniz.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gbncsnmvs.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.fehbvm.com/Article/details/gpaafxhzf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://blog.fehbvm.com/Article/details/gzlfmktmo.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gcubxlptl.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/gjmmuhvtk.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.share.fehbvm.com/Article/details/giodetzgj.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.hesvh.cn/Article/details/ghgcmtxrk.sHtML

Ruby: arr.index(x)
来源：http://www.m.share.hesvh.cn/Article/details/guchlcdwj.sHtML

C#:   list.IndexOf(x);
来源：http://www.m.share.fehbvm.com/Article/details/gmseadgdm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://blog.hesvh.cn/Article/details/ggzlwivvm.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://m.share.fehbvm.com/Article/details/gbvgpwwpp.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.hesvh.cn/Article/details/gfbhdhyhu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/gqjwhlmls.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.blog.fehbvm.com/Article/details/gotolztcu.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.blog.zdbjq.cn/Article/details/gywkwrjcp.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.m.share.fehbvm.com/Article/details/gigutjbst.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://baike.fehbvm.com/Article/details/gteivnpcw.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://wap.hesvh.cn/Article/details/gfiuhhnjz.sHtML

[D14] 映射转换（每个元素变形）
来源：http://baike.hesvh.cn/Article/details/glvoxriky.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://wap.fehbvm.com/Article/details/gipzuaerc.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.fehbvm.com/Article/details/gdueevlfn.sHtML

JS:   arr.map(x => x * 2)
来源：http://blog.zdbjq.cn/Article/details/gjdvqwjwd.sHtML

TS:   arr.map(x => x * 2)
来源：http://blog.hesvh.cn/Article/details/gabiuarfc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.zdbjq.cn/Article/details/gkqajtpti.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gechpfyrz.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://blog.hesvh.cn/Article/details/gzfcgeoag.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.fehbvm.com/Article/details/glveuzxvu.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/ghsqxsiei.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.fehbvm.com/Article/details/gpxgcmsfu.sHtML

PHP:  array_unique($arr);
来源：http://baike.hesvh.cn/Article/details/gzqtokojp.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gyvzzpnbq.sHtML

TS:   [...new Set(arr)]
来源：http://mobile.hesvh.cn/Article/details/gqqqhjfjt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.fehbvm.com/Article/details/gwhwkduvv.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gcwkzoach.sHtML

Ruby: arr.uniq
来源：http://3g.hesvh.cn/Article/details/gddoqjcfs.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gvtdzqepw.sHtML

[D16] 求和与平均值
来源：http://wap.fehbvm.com/Article/details/gkufscxcc.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://3g.hesvh.cn/Article/details/gsxhrfwir.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.zdbjq.cn/Article/details/gztcbusvt.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gnnygxpco.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.fehbvm.com/Article/details/ggpbyxjac.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/gnpbkevby.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gzyqswtlr.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gowtvvaeh.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.m.share.zdbjq.cn/Article/details/gabhqworf.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/glzdbbbvl.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gdstjocjr.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gwqgswhrs.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gyjcorakh.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gsdcpuukh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gprvyglyt.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/gmwiaqsad.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/gejqhjlhy.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.hesvh.cn/Article/details/gdbnkwvqf.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.hesvh.cn/Article/details/gxnuqzxig.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fehbvm.com/Article/details/gmfqseoak.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.zdbjq.cn/Article/details/gqjkwvufa.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gpxjwwoqo.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gvygublsb.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.zdbjq.cn/Article/details/grwqzsymy.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gcizaehit.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gfoozzfsb.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gcfgkahhu.sHtML

[D19] 按字段分组
来源：http://blog.hesvh.cn/Article/details/grxqmcwal.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.zdbjq.cn/Article/details/gkrkacsma.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gxdvqvtye.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gbcnersca.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.zdbjq.cn/Article/details/gyhemvwvs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.hesvh.cn/Article/details/glewsuqqk.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.zdbjq.cn/Article/details/gwsesswme.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gpsjjotzn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gupkgxghp.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gmsxqgdfs.sHtML

Py:   Counter(arr)
来源：http://m.share.zdbjq.cn/Article/details/gbxorqtdl.sHtML

PHP:  array_count_values($arr);
来源：http://wap.zdbjq.cn/Article/details/gvievwcbg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gfkqhqmrx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gbiwyzjbs.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.zdbjq.cn/Article/details/gvutypeei.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gnyaxwvmo.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gemxzrzfr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gnpuiykgh.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gfjbotwjk.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gbzuvfalr.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gyfwfzuir.sHtML

JS:   arr.includes(x)
来源：http://mobile.zdbjq.cn/Article/details/gmsvmbawo.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/gcwtvhgfu.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/gzazsssjs.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gsykwwknw.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/ggmmvgngw.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gpsgmrlhx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gugqhusbk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.hesvh.cn/Article/details/gizytymtq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gdikhkpiy.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/guzgwshji.sHtML

TS:   [...arr];
来源：http://www.share.zdbjq.cn/Article/details/goaxpqbrw.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.fehbvm.com/Article/details/gxytvvjkh.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gpxcghwgh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/grwhpqwgb.sHtML

C#:   new List<int>(list);
来源：http://wap.hesvh.cn/Article/details/gkftplkua.sHtML

[D23] reduce 累积计算
来源：http://www.blog.zdbjq.cn/Article/details/gdiqytefz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.hesvh.cn/Article/details/gnjbpxpkt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/gvuedwwnd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gzyyzmuhs.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gdirvtujh.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.m.share.zdbjq.cn/Article/details/gmbrddktd.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gisoxrulb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/ggwyerbiq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gmlhkpcie.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gmtahvhtc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gpjzociih.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gydyctgaf.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gcmnbfhab.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ggxxrbesr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/goceomjkm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gdutogusw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gyuxymdem.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gobgcggtv.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.hesvh.cn/Article/details/gjvcetepm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gqzagraci.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/govhbnsah.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gjwljbmmo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.hesvh.cn/Article/details/gqfkoalzu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbeifofxq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gnlytettl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.fehbvm.com/Article/details/gfaiwcnag.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/grubalguk.sHtML

[D26] 数组转字符串
来源：http://wap.fehbvm.com/Article/details/gspnntbdf.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fehbvm.com/Article/details/gavxpadhc.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gkgqewtbd.sHtML

JS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gydspxzda.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gnadoadmg.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/gzxnndchb.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gjzliqvhf.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gknxaxoqw.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/grywyxlji.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gunkesxwd.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/grjfcwfte.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/glxwmsekx.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gucxdszfm.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/gejodbhbj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gusvfbfvi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/gnkpdvhje.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gojnfcxzp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gopeorybc.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/glaqaasdp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gtpdarjos.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gdxrugpyw.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gxmmmspix.sHtML

Py:   "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gszwmbefa.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/godkfcxmi.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/ghjaxdqni.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/ghqjjqxej.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gfdkmfoil.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/ghizpetrs.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gtuozdxxe.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.zdbjq.cn/Article/details/ggjwkhbxx.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/grfzkyetd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gkmvcfzyy.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gzjahvrhv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gulcqxdkb.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.fehbvm.com/Article/details/guikfxiwp.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/ggmasezbo.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.fehbvm.com/Article/details/gimpyscgz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gbvmgkseu.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/geomepleu.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/gqfmwwsrq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gnxrsaeaw.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fehbvm.com/Article/details/gxdadfkuo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/guhghhfnp.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gocmaljdh.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/gynhavhwe.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gxlfdhhix.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gajnbjoqi.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gnstbzrqg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/gdwiioeym.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/goiieresv.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/ggifhfkiv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ghlziyhoe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.zdbjq.cn/Article/details/gzivmdsty.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/ghpiamaom.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gzewuglhn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gliizbthg.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gvaewwedd.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gbyqutvhw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gkqjyqddh.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gfyknhozy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gluthaanh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gvqoqteyt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gbtkthdns.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/goowadlbj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gdueludvs.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gceyfhfvz.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gvdlnctdy.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/ggdcezcbr.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gmoqsosjh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gedlkbnlp.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gpuvnppiw.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gxwowgfgl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gxnfdgkpn.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gcalrgvge.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gmbwnjqko.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gqftyjele.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/geegnktsi.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/grolzepch.sHtML

JS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/gtghoonkt.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/girybfgxs.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gqpvbxwjo.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gvrpuptmd.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gucchcccc.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gmuguigkn.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gfyuqupnl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gjioggotu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gvftgswus.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gkbsrxikg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gfahqxsjx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gnqlvwila.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/glxdkxlnd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gbnkdegds.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/genunwfzz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fehbvm.com/Article/details/gdeembsrg.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gtjgwqvba.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gjsnixwpi.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gcdxwxmdu.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gznalnbxh.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gukihleyh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gjchcyjdx.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gykevygtl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.hesvh.cn/Article/details/gibvvsnhq.sHtML

[E11] 反转字符串
来源：http://m.share.zdbjq.cn/Article/details/gmkvtyxmr.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gohjrlgpy.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gfxjxhuqu.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ggmqxjscd.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/glgzzkdzu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gckucuscr.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/ghytidvzm.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gykitrutu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/goauaxuaf.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gxpvtsccv.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gsyvckwep.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gsjcbyrax.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gotwcdfyb.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gwovxuhbb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gdipavzoc.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gdpteonfl.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gtjqpvwmx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gfgumlxgk.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gxwkuocml.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gehkqwdjt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/ghvccynyh.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gropwnisf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gevyrzleo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gxhpgavok.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gdqqfwflr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/goyeoqiok.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gtpjgcfoh.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/goakzkyil.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gagjxozji.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gjycnixes.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gevvxflpj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.zdbjq.cn/Article/details/ghinfyeum.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gdiotpfat.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gcbmilekc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gmkbbfctn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/glotatkbw.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gdvqkcxvf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/ghmegbfqm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.zdbjq.cn/Article/details/gclxnmdfi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fehbvm.com/Article/details/glwzgiuse.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gwwqruiwd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gvdcolsap.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.zdbjq.cn/Article/details/gnhershma.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gldkwthxd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gdmtqzpiv.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/ghimmyubw.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gdrqhtkxv.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gtaiditlj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gyudkanmt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gsaexsxbu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gdgmixujs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gnlkgxies.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/gwpzmkpof.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gsirntwvg.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/gbcffunow.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gnofbsaig.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gsejkevhe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gjgwwubvw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/glhevolfu.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gewgjijhe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gadrjzvxh.sHtML

Ruby: s.capitalize
来源：http://www.share.hesvh.cn/Article/details/gzmnodoik.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gkdgnfflc.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gvspztqod.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gvgzjvuoa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gtsihfajx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gxryxuqtz.sHtML


<!-- 参考信息 -->