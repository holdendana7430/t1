代发 wailian999

[D11] 反转数组
来源：http://mobile.fehbvm.com/Article/details/gianojriw.sHtML

Py:   arr[::-1];  arr.reverse()
来源：http://wap.fehbvm.com/Article/details/gbdmsxbgs.sHtML

PHP:  array_reverse($arr);
来源：http://baike.zdbjq.cn/Article/details/gvlqtnsks.sHtML

JS:   [...arr].reverse();  arr.toReversed()
来源：http://www.blog.hesvh.cn/Article/details/goowaeoyp.sHtML

TS:   [...arr].reverse();
来源：http://read.share.zdbjq.cn/Article/details/gwuthvtns.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gjayydryc.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gzxaydzjt.sHtML

Ruby: arr.reverse
来源：http://baike.fehbvm.com/Article/details/gkhmezqsi.sHtML

C#:   list.Reverse();
来源：http://read.share.zdbjq.cn/Article/details/gezfjqzla.sHtML

[D12] 查找元素下标
来源：http://www.share.zdbjq.cn/Article/details/gjithlrpw.sHtML

Py:   arr.index(x);  x in arr
来源：http://read.share.zdbjq.cn/Article/details/gvgqakfps.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://3g.fehbvm.com/Article/details/gyikpxdab.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gqlvqoqkc.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://3g.fehbvm.com/Article/details/gikedqbcy.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.hesvh.cn/Article/details/ghbgnmzar.sHtML

Go:   slices.Index(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gahttspka.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gyntjivpm.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.zdbjq.cn/Article/details/gxycxrgfm.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.share.hesvh.cn/Article/details/gzjoubbvd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.fehbvm.com/Article/details/gshfrozzo.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://wap.fehbvm.com/Article/details/gdqbwcxfk.sHtML

JS:   arr.filter(x => x > 3)
来源：http://mobile.hesvh.cn/Article/details/grxmvzypa.sHtML

TS:   arr.filter(x => x > 3)
来源：http://www.m.share.fehbvm.com/Article/details/ggnadahxg.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.zdbjq.cn/Article/details/gjgggyuhk.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gwpjrihks.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.fehbvm.com/Article/details/gbffhmlph.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://3g.hesvh.cn/Article/details/gwnsnawqq.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.hesvh.cn/Article/details/ggyydgaez.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://mobile.fehbvm.com/Article/details/gqzijlhcr.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.zdbjq.cn/Article/details/gjhapabij.sHtML

JS:   arr.map(x => x * 2)
来源：http://wap.fehbvm.com/Article/details/gzumarykl.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.m.share.hesvh.cn/Article/details/gtcxhhmig.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gelfpuyks.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/ghpwfnoso.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gpmqvslbv.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.hesvh.cn/Article/details/ghxktysep.sHtML

[D15] 去重
来源：http://www.blog.fehbvm.com/Article/details/gyaglffxc.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://baike.fehbvm.com/Article/details/gkgbjsafn.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/grwdihiyp.sHtML

JS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gnwdlvfrs.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gwgmpcbfo.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gbhqdwszk.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://wap.hesvh.cn/Article/details/gmjukdswn.sHtML

Ruby: arr.uniq
来源：http://baike.fehbvm.com/Article/details/gfgabydmd.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.zdbjq.cn/Article/details/geibomqef.sHtML

[D16] 求和与平均值
来源：http://m.share.fehbvm.com/Article/details/gbvoubynt.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://baike.fehbvm.com/Article/details/gbwvlgtmq.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gwvthqozk.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.fehbvm.com/Article/details/gzsgngkiq.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.hesvh.cn/Article/details/gaupojlzy.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gryjgaduv.sHtML

Go:   // 手写循环累加
来源：http://m.share.fehbvm.com/Article/details/gicyieebt.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://read.share.hesvh.cn/Article/details/gebwhxheg.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/gyfgqckza.sHtML

[D17] 最大值与最小值
来源：http://mobile.fehbvm.com/Article/details/gwjhnahmc.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.hesvh.cn/Article/details/gxyyglypn.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.zdbjq.cn/Article/details/gphzbnvar.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gmnnnckph.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gdcgojoqu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.zdbjq.cn/Article/details/gbeqlfxdi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.zdbjq.cn/Article/details/gqsgcqysu.sHtML

Ruby: arr.max;  arr.min
来源：http://baike.fehbvm.com/Article/details/gifswrqkz.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gpllmsoox.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.hesvh.cn/Article/details/gcvykrufg.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.fehbvm.com/Article/details/gawwabmyn.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gfbephdhs.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.zdbjq.cn/Article/details/gpxaznsxr.sHtML

TS:   nested.flat();
来源：http://read.share.fehbvm.com/Article/details/gokidboyy.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gmcrqlffl.sHtML

Go:   // 手写双层循环
来源：http://mobile.hesvh.cn/Article/details/gokxxehwg.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gptqafhkr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fehbvm.com/Article/details/guvmvhrll.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/glerrnjfs.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gzfmtaeug.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.hesvh.cn/Article/details/gifpafrir.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gpiwdjizv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/gwbzhjmje.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/guxdlncsu.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.zdbjq.cn/Article/details/gkisdedoi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.zdbjq.cn/Article/details/gyhuscjkd.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.hesvh.cn/Article/details/gtkrsawjo.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.fehbvm.com/Article/details/gnnnhttxr.sHtML

Py:   Counter(arr)
来源：http://baike.zdbjq.cn/Article/details/gmtaotibg.sHtML

PHP:  array_count_values($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/guqdrwgst.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/goqtvfydn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gkxsgxctw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/ggolxfkja.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.zdbjq.cn/Article/details/gnadjnkxe.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/ghvkxaegq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/ghgvdxjcq.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fehbvm.com/Article/details/gvbiovcqq.sHtML

Py:   x in arr
来源：http://read.share.fehbvm.com/Article/details/gagmkyogt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.hesvh.cn/Article/details/gworbrieg.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gqrqczkkd.sHtML

TS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gjfdfujsp.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/geekqsvzg.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.fehbvm.com/Article/details/gickmlyyx.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/glpldjcbb.sHtML

C#:   list.Contains(x)
来源：http://read.share.hesvh.cn/Article/details/gmwnuqmax.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.zdbjq.cn/Article/details/gglyydfyh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gytcucwdj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gitpzzssm.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.hesvh.cn/Article/details/gmaswejqq.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gjvphfimt.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gpszusyza.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.zdbjq.cn/Article/details/gdzeoaozt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.zdbjq.cn/Article/details/gjpbhxgpu.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gowcmxign.sHtML

[D23] reduce 累积计算
来源：http://www.share.hesvh.cn/Article/details/gqdgmzlka.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/gicmjleht.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gosidmclk.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/geafgmmve.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gepfmrwgo.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gyctggzmj.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/ghedgiqrc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.fehbvm.com/Article/details/gcshwfmpq.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gbtubhfac.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gepnibljz.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://blog.zdbjq.cn/Article/details/gperooglh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fehbvm.com/Article/details/guzpcazrm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gyraxfazp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gshplxjmk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/ghexpvfbw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.zdbjq.cn/Article/details/gjnzeofjg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gcbsvrlxl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.fehbvm.com/Article/details/gvmeiakmv.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/gtibmpdnu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/gcafwhday.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/genscqmhy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/gyjevrzhq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gvqmcmcfi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gytmntgsn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.zdbjq.cn/Article/details/gqlieyzve.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.zdbjq.cn/Article/details/gicikckzc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gsxbwbmwk.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/gekdupert.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.zdbjq.cn/Article/details/gfwgkxshd.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqabofogs.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gjwowavma.sHtML

TS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gdprgptqg.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gphxrgygz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.zdbjq.cn/Article/details/gnqoefiwa.sHtML

Ruby: arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gzakpvvcz.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/ggsgfyiyj.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcrlrtydl.sHtML

E. 字符串处理
来源：http://www.blog.zdbjq.cn/Article/details/gjydjukbd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ggonsehyy.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/goqektegb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.zdbjq.cn/Article/details/gdybelxin.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gzpvourbt.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.zdbjq.cn/Article/details/geydbsmoq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gqodjjdub.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gaxvergnn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gfqcxtlyt.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gzlpwjsiy.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gjgkdvuei.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gsychvajv.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gapfudaog.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gpfmutlgo.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gnhgnlhhr.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gpmobmaeb.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gbtmrbhra.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gzgnwdftq.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gdizjvzra.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/ghvtnvaqd.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/gasjdpitg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gzgnkcywd.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gsgbyzrph.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gyxwpgear.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fehbvm.com/Article/details/ghsbamstv.sHtML

Java: s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gpuaoosnc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.fehbvm.com/Article/details/gurfavaei.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fehbvm.com/Article/details/gszptcacm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gmkdviakd.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/githhmlmc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.hesvh.cn/Article/details/gfldajzrt.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/garawstxz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/gbkzbohcj.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gmtcoqwyh.sHtML

Java: s.indexOf("x")
来源：http://baike.zdbjq.cn/Article/details/gqxrkhemn.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.zdbjq.cn/Article/details/gaztbrsvv.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/ggdaaozpc.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/ginghblek.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gubekcfvh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gbznrdsjg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/grpsqlhiv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gyaqweywr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/grbjthlkx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gzxrrqxaz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.zdbjq.cn/Article/details/grteturiw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/gwdweofid.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gxohvkqkt.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gyfpiunzx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gocvhttpg.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gmsunexbt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqnbenfgs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gzbrbdbzn.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gvygpdtrv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/ggjgbwqut.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gjlxfkauf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gtrwlulwm.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gihdmeihk.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gandouzez.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gplakdcwq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gwtlmbfbk.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gqdnomeww.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gmtcnclwt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gehajuwol.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gmmsncizl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gjsxbceyx.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/grwprqodb.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gtkjixcxf.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gfreqqlle.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gswjivpnl.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/ghtntvmzk.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gglgcjswo.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gfyldeiex.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gkwiauhns.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkxojtcv.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gqdgptgya.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gmauanzai.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/guvvosawd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gxivdfkkd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gblityevs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/garubrvjg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gzmqkwygy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gishlshfo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gqyzryjmm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fehbvm.com/Article/details/gmmhoejyp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gvxguwdiy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.zdbjq.cn/Article/details/ggopijntf.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gevfiiipt.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gnzveurxv.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gzkztkytn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gakbjyatb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/grxruzcvc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/guyqwppch.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gzvuingft.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gtztwtxnw.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gjntvkfqy.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gpwvqugrh.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gtfevxbiz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gikbzgujs.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gcifqlykz.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gtfbnlkqc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/ghxfxkvwj.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gorlaqfos.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gjbuulxpw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gvkgnpzus.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gubjxurqn.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gasvvjgap.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gmpxavilq.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/glvfigupz.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gflfwkeac.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/glapwkyew.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/gwqowyupo.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/ggmcengtq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/gqgnjqfni.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gspvsxava.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gcyuswvqc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gpwttuowl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/gfebjifhp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gukbfhisg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gmukxotef.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gdpkqvxak.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gvexubjog.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/gvqokajmj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gdpzodvnz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gfwxivsud.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gwecmdwhc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gndmbkmgk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gdiqifmrs.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gkxntiuih.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/gnhsfzdgw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gvmhkjyay.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gylxvzdzs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grcalviyn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gjrzpwlpf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.fehbvm.com/Article/details/gprovoanl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gljoeisfy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gbfulgxil.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gagumzoas.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gcafulape.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gvsvjjnvo.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/ggmqrkgpm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gpimxxsku.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/ggtxqseau.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/ggzlcxisu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gwgouaqkl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gajwixawd.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gwgqlggep.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gaeovokij.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/giypupvbf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gyhfamnbp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/geeavhaef.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gqvorjlil.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gjiuevqcf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gslfsmruq.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gcqamencb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/geccdyxpd.sHtML


<!-- 参考信息 -->