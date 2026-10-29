代发 wailian999

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://read.share.fehbvm.com/Article/details/gviwbpkut.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gwsejwpcp.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://3g.fehbvm.com/Article/details/gzqjwzuey.sHtML

Go:   slices.Index(arr, x)
来源：http://3g.fehbvm.com/Article/details/gqdjdfgaf.sHtML

Ruby: arr.index(x)
来源：http://www.share.hesvh.cn/Article/details/gdnpddkwr.sHtML

C#:   list.IndexOf(x);
来源：http://blog.zdbjq.cn/Article/details/gbrzbrvfr.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.hesvh.cn/Article/details/grhjdpqlo.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gmxjwpizu.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.hesvh.cn/Article/details/gsmemfpxt.sHtML

JS:   arr.filter(x => x > 3)
来源：http://m.share.fehbvm.com/Article/details/gxbmipgch.sHtML

TS:   arr.filter(x => x > 3)
来源：http://baike.hesvh.cn/Article/details/gdkvatfst.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gzashwvtn.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://blog.hesvh.cn/Article/details/gpfreknaj.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://blog.zdbjq.cn/Article/details/gewbefynj.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gpaatahyo.sHtML

[D14] 映射转换（每个元素变形）
来源：http://mobile.zdbjq.cn/Article/details/gwpmuoace.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.hesvh.cn/Article/details/ghqqakdby.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://3g.zdbjq.cn/Article/details/gzriowdnr.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gmomucbeg.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gpjloclgc.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gmnatpuyb.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gzabjmmju.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://baike.fehbvm.com/Article/details/ggbtfyaxi.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://m.share.zdbjq.cn/Article/details/gaqzyugtq.sHtML

[D15] 去重
来源：http://www.blog.zdbjq.cn/Article/details/gqndqmslf.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.m.share.hesvh.cn/Article/details/gkqaexykp.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.zdbjq.cn/Article/details/gwstovpbb.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.hesvh.cn/Article/details/gemoiukvz.sHtML

TS:   [...new Set(arr)]
来源：http://baike.fehbvm.com/Article/details/gzwwixjaq.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.zdbjq.cn/Article/details/glxlfeezl.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.zdbjq.cn/Article/details/gtfspycuy.sHtML

Ruby: arr.uniq
来源：http://wap.zdbjq.cn/Article/details/gbqxfmnhf.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.zdbjq.cn/Article/details/goffjsxev.sHtML

[D16] 求和与平均值
来源：http://baike.hesvh.cn/Article/details/gxeyexriy.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/glvvevgho.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.fehbvm.com/Article/details/gwlcxtjmn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.hesvh.cn/Article/details/grmneociw.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.zdbjq.cn/Article/details/gdgcvnghe.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://baike.fehbvm.com/Article/details/gpfmnzuhv.sHtML

Go:   // 手写循环累加
来源：http://wap.hesvh.cn/Article/details/gcuawpubg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gbguawrhc.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gtpuuokew.sHtML

[D17] 最大值与最小值
来源：http://m.share.fehbvm.com/Article/details/gecyqqdjj.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/gpsigspvx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.zdbjq.cn/Article/details/gitzajbvb.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.fehbvm.com/Article/details/gsqjbiajt.sHtML

TS:   Math.max(...arr);
来源：http://www.share.fehbvm.com/Article/details/gdykmjriq.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.hesvh.cn/Article/details/ggvtewhiy.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gxndyuhva.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/gyoprlsda.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gulrtgyrs.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gougffmsm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/ggpnrjlln.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.hesvh.cn/Article/details/gpsvidusg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/ggnymixvp.sHtML

TS:   nested.flat();
来源：http://3g.hesvh.cn/Article/details/gfgsaruev.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.blog.fehbvm.com/Article/details/gfanrfofo.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/ghnmtdhbb.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gtmblipph.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.zdbjq.cn/Article/details/gfrkqbvng.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gdubiodrm.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.hesvh.cn/Article/details/ggnufnoal.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gxmkwydjv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://read.share.zdbjq.cn/Article/details/gqknbwsjc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gfbtpgjza.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.fehbvm.com/Article/details/gvvfentlo.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.hesvh.cn/Article/details/ghjmksrom.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.zdbjq.cn/Article/details/gjbqfowon.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fehbvm.com/Article/details/gxjcdxyhs.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/guiktuurc.sHtML

Py:   Counter(arr)
来源：http://baike.fehbvm.com/Article/details/ghnwddihe.sHtML

PHP:  array_count_values($arr);
来源：http://baike.hesvh.cn/Article/details/gspxmxwfw.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gpapzvyul.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/ghlmfcfdq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gcjaqdlto.sHtML

Go:   // 手写 map[T]int
来源：http://baike.fehbvm.com/Article/details/gvbnnxove.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gltcckofw.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gvxjjiusp.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gwfkdflxa.sHtML

Py:   x in arr
来源：http://3g.fehbvm.com/Article/details/gckrnucmd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/geyolcnez.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gyoexdggc.sHtML

TS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/ghyqxkjvy.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/ghlbbkmrd.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gvsnmxlzx.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gjxgxwjuc.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gjubqomgg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/ggbrwmxpq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gsdsycrbf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gkjpssqsc.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ggosmkulu.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gxxlfggfm.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gpxvrxsuy.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.zdbjq.cn/Article/details/gfglysbwq.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gtlmigcxc.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gxduhqmlm.sHtML

[D23] reduce 累积计算
来源：http://wap.hesvh.cn/Article/details/gckstimzz.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.fehbvm.com/Article/details/gdqcyopnh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/guoeuiqot.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/glyjhmwjj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gysquamsa.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gcrqrvdnl.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gcxebeuvo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gmstttjxf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gylfpfohc.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gakiomjzp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gdhqjfrwu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.zdbjq.cn/Article/details/ggyujuehi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gdbojmqkz.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gpdblkoaj.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gmneypgzy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.hesvh.cn/Article/details/gkpqgvwsy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gbhrvibiz.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/govqrpwcg.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/glpgtzkkk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gxnajpomn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gtnndudpa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gjwsvrpde.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gjloegxhd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/gqrqcafzj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gcmfrioae.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gilianmes.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/getlazwfx.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gfilhczlh.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gszxxmlex.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.fehbvm.com/Article/details/gxxjztayf.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gseowyvcp.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/ggvukcbod.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gefgaiior.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gijylcptr.sHtML

Ruby: arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gpcgezsvl.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gpiyjglyj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gakjjrhef.sHtML

E. 字符串处理
来源：http://baike.zdbjq.cn/Article/details/gscdtyhmg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpktzvtcn.sHtML

[E01] 拼接字符串
来源：http://wap.hesvh.cn/Article/details/goyuvfiec.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gmyclqrgk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gltszuxej.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gyokkezzw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/ggbsnisjs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gwqqtpnph.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/gegpbfmga.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gdkxxodyj.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gsklqitph.sHtML

[E02] 重复字符串
来源：http://read.share.fehbvm.com/Article/details/gznbydgym.sHtML

Py:   "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gzfggopkw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gmfnsudow.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gfhlpjowu.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gvemblnok.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gpkejdgtb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/gjbwufkgq.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gtnqxvdjp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.zdbjq.cn/Article/details/gwuymlmdx.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gaflzbpmp.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gtrpdakzb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gouijytgp.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/gxjumffwt.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gozyvoubr.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gfawruukc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/galdzdzwe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/ggsyurgtm.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gcgvoxinc.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gxgmwlghv.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gyjstpanv.sHtML

PHP:  strpos($s, "x");
来源：http://baike.zdbjq.cn/Article/details/gihnzbwno.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/golbiarat.sHtML

TS:   s.indexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gkaycgkln.sHtML

Java: s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/ghxcnsleh.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gsavowqtz.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gvraciwuy.sHtML

C#:   s.IndexOf("x")
来源：http://wap.hesvh.cn/Article/details/gpyvnrcck.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gbyostpyq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.zdbjq.cn/Article/details/gsgnobhvd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/gqzbqqqdt.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gonbnvcap.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gijqoxnzp.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gcxdfikwe.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/getslkgal.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.hesvh.cn/Article/details/gbaospjvr.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gbdsfhoao.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/golpmtzdn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gfabfddip.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gupijgmpa.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gtzhienxt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/grkyuejmu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/ggpfqvojn.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gqljeezib.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gkdprfwyn.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gcoalbatw.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/guldgbkeo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gqhfukgvv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gmnuaxkbo.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gansziuio.sHtML

TS:   s.split(",")
来源：http://baike.hesvh.cn/Article/details/gboaeyhiu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gihdbrtbk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/ggrwrsozx.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gqdiomstp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gtxmfwtal.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gsxjiqvms.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gqfndrvyg.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gvloalxpl.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gugzsvdpi.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gthglonoy.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gfitwbcju.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gejteapuv.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gcfgkyuuj.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gijbailqy.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gaoncpuys.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.hesvh.cn/Article/details/gkccolery.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gorklnskm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gddfsmuyw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/ghhdjsjwa.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gdylzrrfg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/grmghtqwk.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gblpahukm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gwqqvdlkc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gynzcrxtq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gghxthpen.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/gaggqkvta.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gcjyuomgr.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gbjajezsy.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gjukoayzh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gvvyovdcq.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gguijyotk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/glklpiyyu.sHtML

[E11] 反转字符串
来源：http://wap.zdbjq.cn/Article/details/gwndrqkft.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gntvfydma.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gvllmkbfc.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gavugvmvd.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gkukuyhuj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/guzkvxsna.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gijcvxgme.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gdbwaksio.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gtpuocmwl.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/grtzrarrr.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gjnuhrmsr.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gpgbbbwlx.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gsgsvqfiu.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/ggnaanoqe.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gbjkpqlva.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gnbiuprgo.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gvognkwit.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/giguivups.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gpawxkodk.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gijipokjk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/ghrhyklhi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/grhwrwjhq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gyrwoenfx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gngscjjqr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gyqdxpslz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gvbzosdsm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/ghfgvadze.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/ghrstgkml.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/gtzrklqgg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gscvycflt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gavnhoegu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gwqboxvts.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gnnlohgvj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gcajqjivy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gjtwotbml.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gmklosars.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gpepuyxiv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gmzjhzbzu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gstpizvcm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpqdxyskn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gctjzsugj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gwabhmaep.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gjkjxgbhi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gmxtfzide.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxsiqvrhh.sHtML

[E16] 数字千分位
来源：http://www.m.share.hesvh.cn/Article/details/gkxaghear.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gzgyuugxm.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gobiebezr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gbusicbdu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gzdgnrdxb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gwrkqeczp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gtfthfrgq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gixpioihy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gwxvgssnb.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/ghuyspsuc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gsgfgpdzk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gubgkmgwp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gsikxvrvg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gawvizbuv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gxchpveqo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gxynmpbnt.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gntxvnrhx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gkvjazayq.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gnidzxxxq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/grjoihalj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gwtwspvzp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/ggttzadyh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/ggbmxculz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gdqxxbdbr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/ggrpssdlj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gweyjpqag.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/glmvvlfli.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gamhmgipu.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gkxyzgqds.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gnbohudgk.sHtML


<!-- 参考信息 -->