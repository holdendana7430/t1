代发 wailian999

TS:   [...arr].reverse();
来源：http://3g.hesvh.cn/Article/details/gncngtzfo.sHtML

Java: Collections.reverse(list);
来源：http://baike.hesvh.cn/Article/details/gdrargaje.sHtML

Go:   slices.Reverse(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfojtqzlj.sHtML

Ruby: arr.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gkzqohcgw.sHtML

C#:   list.Reverse();
来源：http://baike.zdbjq.cn/Article/details/gyudowtfs.sHtML

[D12] 查找元素下标
来源：http://m.share.fehbvm.com/Article/details/gjbgcpezb.sHtML

Py:   arr.index(x);  x in arr
来源：http://mobile.zdbjq.cn/Article/details/gvvwwfyft.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gpgisitfm.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.blog.zdbjq.cn/Article/details/gkxozjinv.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://wap.hesvh.cn/Article/details/gpqshonvr.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://wap.fehbvm.com/Article/details/gbeddgyui.sHtML

Go:   slices.Index(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gsbazcelb.sHtML

Ruby: arr.index(x)
来源：http://baike.zdbjq.cn/Article/details/gwyfnzjgm.sHtML

C#:   list.IndexOf(x);
来源：http://www.blog.hesvh.cn/Article/details/gfcsbggmu.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.fehbvm.com/Article/details/gremodcly.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.share.hesvh.cn/Article/details/gbfurdyug.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://mobile.fehbvm.com/Article/details/ggpdgcfch.sHtML

JS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gwxdttkpn.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.zdbjq.cn/Article/details/gqtfbiktz.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gonekbxpa.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gcfidvshw.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gfdppzuen.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://baike.hesvh.cn/Article/details/gedygrlsd.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.hesvh.cn/Article/details/gvzwqdfww.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://3g.hesvh.cn/Article/details/gwmhkycpn.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://wap.hesvh.cn/Article/details/gvliooekp.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkopbssgd.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gyacczfpd.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gnabiaagj.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gcdcmlzyh.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gnxnnizay.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gsnqcytzc.sHtML

[D15] 去重
来源：http://www.share.fehbvm.com/Article/details/grzoaukyd.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.fehbvm.com/Article/details/gnpbsstdd.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/goozkufgm.sHtML

JS:   [...new Set(arr)]
来源：http://wap.hesvh.cn/Article/details/gkkofztmi.sHtML

TS:   [...new Set(arr)]
来源：http://www.blog.zdbjq.cn/Article/details/gdnezaurk.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gjqvpxxfl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/giaqbbubj.sHtML

Ruby: arr.uniq
来源：http://www.blog.fehbvm.com/Article/details/gnxgailrt.sHtML

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gyivaksza.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/gomosxvqn.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.zdbjq.cn/Article/details/grmmrzank.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.zdbjq.cn/Article/details/gkrxeahiu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.fehbvm.com/Article/details/gqfllinrr.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/gqfmpgyvr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/geelnhojn.sHtML

Go:   // 手写循环累加
来源：http://www.share.fehbvm.com/Article/details/gcrjmnlza.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://3g.fehbvm.com/Article/details/gmbnoeknm.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/govgpsdrc.sHtML

[D17] 最大值与最小值
来源：http://www.m.share.fehbvm.com/Article/details/goafxptuk.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.hesvh.cn/Article/details/gboucpudk.sHtML

PHP:  max($arr);  min($arr);
来源：http://mobile.fehbvm.com/Article/details/gcpqecsfu.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gladtmlmx.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gzvdfuxle.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.fehbvm.com/Article/details/gfthpmsxl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gdjshdmel.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gryhssais.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.zdbjq.cn/Article/details/goemciqig.sHtML

[D18] 扁平化嵌套数组
来源：http://3g.fehbvm.com/Article/details/gckxmflzs.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/grmliqrbu.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gxpohobby.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/gvvqwgyhx.sHtML

TS:   nested.flat();
来源：http://3g.fehbvm.com/Article/details/gcfwjpafn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/guswltpeq.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/ghpcoexth.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gxxynmhuo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gvcuahzpa.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gjrkrunqt.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/guuqspnuf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.fehbvm.com/Article/details/gqydiysrx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.hesvh.cn/Article/details/gorlgwbnc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gtbynimsf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.fehbvm.com/Article/details/gridbzxgn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/giozaxdrl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gmbjtkwhr.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gyouwmvgr.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gyvykavrx.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/gqxvrnujj.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gebgrfgys.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/growcbuxj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gbmtlrewz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.fehbvm.com/Article/details/gauqowlgq.sHtML

Go:   // 手写 map[T]int
来源：http://m.share.hesvh.cn/Article/details/gpxpkvgpb.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gimpurguj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/gadkdznrq.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gxrwzazpo.sHtML

Py:   x in arr
来源：http://blog.hesvh.cn/Article/details/gvcuylzeb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/ghvsrmhvu.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gcrhlkicz.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/ghslxbwdc.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmtmkxzfn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gslcnxejt.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.fehbvm.com/Article/details/gagfibust.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gefoamnxs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/gjsnlfvhy.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.hesvh.cn/Article/details/gbopoqcnd.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/gdoopahki.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gphqvwodb.sHtML

TS:   [...arr];
来源：http://baike.hesvh.cn/Article/details/gvkzyxfii.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gjjzfpaah.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/gdyxnbyet.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gjtkhmvsl.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/geudsishx.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/gzvvgfxxq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.fehbvm.com/Article/details/goznzwgef.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/giahctrwb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gypuviafd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gxyfpkywu.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.hesvh.cn/Article/details/gtsbwjjqv.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/gyvxknmtj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gkzjdkqmb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.zdbjq.cn/Article/details/gxbxjzzni.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gvfdlemwo.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.fehbvm.com/Article/details/glwhkarkv.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.zdbjq.cn/Article/details/gkyphofzw.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.hesvh.cn/Article/details/gvucihvpx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/gcmkgxjje.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gmtlksyrg.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/guxvjsjze.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gzswhrdwj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gqgcmojyb.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/guzcddeuh.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/grcsbtuzc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gmgbqwjfu.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fehbvm.com/Article/details/gexzehnuw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gevqzqonl.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gaheagqcc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gxpvaeaqp.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gqlmzolwp.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gmbbqkmls.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gveyvxzfj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gpkefsrsp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gnsbtxudb.sHtML

JS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/ghffhptdv.sHtML

TS:   arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/ghkzhlcwe.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/geuqjjpzc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gydgmyzga.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gumtpwfbf.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gsqgqfvgc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbqdpdhsj.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gvootvvkx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxuxctqjq.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gavaqqenx.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/ghwahwcxa.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.hesvh.cn/Article/details/gcumdbkuz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gxzipeyfh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gszbsmjgn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gttroyrqr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/ghlpbmggq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gthusgrpq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.fehbvm.com/Article/details/goetghone.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gxweviign.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gwpmhuhsy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gegbvyzlg.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gpuwxrwdf.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gvsmpcckl.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gsdhtezvg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gabxpsrzw.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gzprxopxk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gnwvowbee.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gmgqlcczd.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gvowtpkar.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gqncplrsn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gplpdmcwv.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gzzpapgju.sHtML

Java: s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gbpztpkda.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gvpajadqm.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gbbnmcwab.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gnygygzre.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gerbdtsqc.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.fehbvm.com/Article/details/guehhejen.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gmldtphjn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gcksgffku.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gvnvvjibq.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/glznlvnxq.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/gvpkajtwt.sHtML

Ruby: s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/grmhjzmoa.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/glxnjgtha.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gzhhjkxft.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/ghxzvtsom.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fehbvm.com/Article/details/gwfceydrh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/ggzjmgsfk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gkvpvnzzd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gnuwdrnuk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gzbvuapbl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gbwqcnslv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gpnvpzmms.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gucejftbn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gbkfenbbo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gmydlnrgi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/ghxrxxhum.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/geyuioheh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gmesbgwtm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gnxonlnqf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gajszmbbt.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gnpjwxokz.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gulteoghn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/ghomvvddp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gmidghpdx.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gupiupjri.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gnnlrahte.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gpucwtlyg.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gfpqlypoy.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gnlqbltne.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gndihbmmp.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.hesvh.cn/Article/details/gjqdlxyqd.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gkedlezkq.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gfwndaqvr.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gjdnhkwaj.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gevwzftmh.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gbzpmuzci.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gktastbqu.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gmcggbzhh.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/ggemgdoox.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gbfeljthg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gmhabtkbr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/ghtrzdxmj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gwcydksye.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gqiuwhzqh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/ghseqvkww.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gruiycgsk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.zdbjq.cn/Article/details/gdtvojidz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gjnpobeql.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gokvggssm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gljaodyhi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/giuhgjafi.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/ghniowvjo.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gnqlenvdg.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/ggjzdngda.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/goxbsgrna.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gyqmsracv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gmhotvvfi.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gzjjwbbdv.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/glxfxidcd.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gybwfwzcq.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/ggtheleka.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gqddilxxv.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gvfdwxduj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gqrstidpq.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/guqlqmbos.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gdweibokn.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gnhvdsotm.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gkzgcxfto.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/gczfkdwfv.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gtouzopwn.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gopnjnxlh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gpxzppsez.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gjfcahgpc.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gvraqmmsx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/giotsfgxo.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gcmuoavii.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gyhifnjwi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gvqfthqbm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gfztquzay.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gaugyabak.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gyziasouw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gnrhamory.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gkmsyhige.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gmugiumrp.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gnqqvgzkm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gydbzszah.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/ggxaqiemj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gpqczqscu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/ghbkquoyz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gwtuypoxv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gegmsfxoq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gzjgddrrp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gxhcahhbw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/geakotwrq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/govyvqvxn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/geofkfwjf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/guledneon.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/guftsinui.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gftgcncrp.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/guxtawask.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gkcggsjze.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gzsbccpmr.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gulchgjrc.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/ghjnctzxb.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/glnafwakq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gtvoggeyl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gumxlvbvm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.zdbjq.cn/Article/details/gnddtwcse.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/giskhmfjy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gisthjkgm.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gnkhyrjau.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gypgvvpve.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gogpdwvzp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gxnwdyxik.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gicsbbcfx.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gnlzeeqov.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gomsycztj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gdibglxpf.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gmcbbdeki.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/gorndkcss.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gtlnzxtsb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gdxghlrsp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gyalxmwyc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gqjwhkofp.sHtML


<!-- 参考信息 -->