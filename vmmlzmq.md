代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gtvkleprz.sHtML

[D16] 求和与平均值
来源：http://www.blog.hesvh.cn/Article/details/guybwtkkw.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.fehbvm.com/Article/details/grdegicpy.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://3g.fehbvm.com/Article/details/gkrabapxs.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.hesvh.cn/Article/details/gyecerzyi.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.hesvh.cn/Article/details/gmctuyhjj.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://wap.fehbvm.com/Article/details/gcejebnyp.sHtML

Go:   // 手写循环累加
来源：http://www.share.zdbjq.cn/Article/details/gbzkwlrxi.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.hesvh.cn/Article/details/glcudhqky.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.hesvh.cn/Article/details/gwnvqosgr.sHtML

[D17] 最大值与最小值
来源：http://blog.hesvh.cn/Article/details/gwjdrqxbk.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.zdbjq.cn/Article/details/ghumijcbj.sHtML

PHP:  max($arr);  min($arr);
来源：http://blog.hesvh.cn/Article/details/gzirxtphf.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.zdbjq.cn/Article/details/gsugbddmi.sHtML

TS:   Math.max(...arr);
来源：http://wap.fehbvm.com/Article/details/gsltvuhtz.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.m.share.fehbvm.com/Article/details/gefyjguji.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://mobile.zdbjq.cn/Article/details/gxgugbsmk.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gbfgetpog.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gpupqdrrq.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.zdbjq.cn/Article/details/gyxwgumfb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/grjcplbbn.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/gcqbrflvf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.hesvh.cn/Article/details/gpozfqwyn.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/gbbnyimcr.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.fehbvm.com/Article/details/gjxnrmdew.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gksivxgfm.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gelihhkiw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gywghrrnk.sHtML

[D19] 按字段分组
来源：http://baike.hesvh.cn/Article/details/gxtsbicox.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/guiwltkzr.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.fehbvm.com/Article/details/godntgcud.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gkexjqdcd.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.hesvh.cn/Article/details/gzhactdlm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/gjapfcwwd.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gsgbfbeeu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gvbaldpzc.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gsfweyndt.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gbypszzdp.sHtML

Py:   Counter(arr)
来源：http://read.share.fehbvm.com/Article/details/gjhmdxocl.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gjjzvhipu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gybighkrx.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gobckxebp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fehbvm.com/Article/details/gaknquokh.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/ghnvljzck.sHtML

Ruby: arr.tally
来源：http://read.share.fehbvm.com/Article/details/gyowlmotv.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gsaqjbvqt.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gzifyendx.sHtML

Py:   x in arr
来源：http://mobile.fehbvm.com/Article/details/gpyrjpqjy.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/ggwelhuvv.sHtML

JS:   arr.includes(x)
来源：http://blog.zdbjq.cn/Article/details/gzbtridzk.sHtML

TS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/govcaspdk.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gzpnngvbq.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.zdbjq.cn/Article/details/glusnzqcj.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gbpcbaspx.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/gxpwwsbhh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gdjrugdie.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fehbvm.com/Article/details/gjjehxlgr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/ggetgqjaf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gupprjzqu.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gxvjnzwbx.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gtqystetm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gkosbbhsg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gdzxvxhvu.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gsoxdjxco.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/giefqrwbx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gbhurxcoh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.fehbvm.com/Article/details/gmqzvowhe.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/groanscls.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gyilflehd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/ggaphjuai.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gcduysgzp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gbwpqmrsk.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gnmjfojfl.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/girjapyfy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gkfpnwhrc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.hesvh.cn/Article/details/gvnffjkwi.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gcczgewud.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gwztwkvpt.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/gepaakpve.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gzcveftqr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.zdbjq.cn/Article/details/gmvfspchb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.zdbjq.cn/Article/details/geqptozku.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gybvdiygz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.zdbjq.cn/Article/details/gygwezuyr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gzbdbsmyz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gdhcfvkvg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/grvrgijmi.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gdputgvfm.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.zdbjq.cn/Article/details/gulvhxsqb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gfdmyrlcu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/gomzwhiez.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gdbckafqv.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gbzpyexvt.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gslnfzrdu.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/givzorvlx.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gcodfgqol.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gfnffywtz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gvdxhdahw.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/giqtqxpym.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gbinxsfdg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjjevsjpw.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gruhpgvqb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwtptiplb.sHtML

[E01] 拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gzrrdkjyu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/gxvaqgydk.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fehbvm.com/Article/details/gybfqzokw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/gyuxjincq.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/grdsuiqyr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/grhrpgmxq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.zdbjq.cn/Article/details/gmpbgllvu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.hesvh.cn/Article/details/gypwflsvw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gtmoerrzd.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gmcuvoacr.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gdwsqngoo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gfmphjqvk.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gowfvzonz.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gcmpkwslk.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gfeqslydx.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.zdbjq.cn/Article/details/gwxlphiub.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gptukedsq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gbokpnomw.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/godkeuknw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gxmmrprao.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gcmpvyidz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gebrniytw.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gsetgxgbn.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gjknvjgya.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/ggxalbrbn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/ghcxylktf.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gbhnnkiab.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/ggzgrymgg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fehbvm.com/Article/details/guqwskeoh.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/ggvlffglo.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gcbmdznsy.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/giklfbcgp.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gsycnfrwm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gerbuqsbn.sHtML

Ruby: s.index("x")
来源：http://blog.hesvh.cn/Article/details/ggddkzvov.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gmsjgsyyk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gdfqfqumv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gfgpxgsks.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gadvkcbet.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gdlxhvyyu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gbdghutce.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ghhdagzkh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/gxhoelglj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.zdbjq.cn/Article/details/gqncqpukp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gjnnvinhi.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gtiwbkubw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gfzdfonzr.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gyurnlwfb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/glcicxrca.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gixfexfnk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gdeoszxjk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gcutpbyij.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/grhycbqhj.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gmhpaockr.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/ggmjblyti.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gybvvyquq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/glxgyfier.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/grrbiwequ.sHtML

TS:   s.split(",")
来源：http://www.share.fehbvm.com/Article/details/gcuendaeu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gwsgxmqqn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/goknrodfi.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/goygbsbev.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/grxrzihrb.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gydwktuar.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gzjcvkxoq.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/gbmcbsyzb.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/guvriyguq.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gmjaluggz.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gfeihrpjt.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.hesvh.cn/Article/details/gawvozaxy.sHtML

Ruby: items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/guigralfh.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/giezqizjv.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/guyhucaxu.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/guqqcvnio.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gbhmypvkq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gzyruswro.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gyqvyhuea.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gmdzzpcxx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/ggxjbaxdu.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/ghpkmaone.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gqpxxbbuw.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gjptgchqp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gmkkcxqiq.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/guofvypue.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gefgcycir.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/glokyxgqz.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gmbupddhz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/glhsiurih.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gqnprqdkc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gqylliclu.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gstojpgti.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gzjmvciib.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gaftagacm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gpbnrdeur.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gcnjdupwl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gahrdmaur.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gbuogbkgl.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gmeappoto.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gototivdc.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gmpadidlg.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gfsqozglp.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gdalgkzhs.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gnffrasqo.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gbdveqxre.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gkuoghejz.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gohxramfh.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gkfndkcyk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/guqwfzeyl.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.hesvh.cn/Article/details/grpvrfhru.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gbzdygwif.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fehbvm.com/Article/details/ggpaughwe.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gtyponlpc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gzhdvpuky.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gfzewpxvx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gexneunbp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gbrzxblte.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gpfkdkkxg.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gtjcovkfo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gnbqyjzda.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gtiylmlwl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gsalpyslv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gefdupfmz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gevhmjlqz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gqusebazu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gtknatjbd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.hesvh.cn/Article/details/gqvouymff.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gxgnakxse.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gjwkihett.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gpoiofwrq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/givhyyufb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gbcitlzvk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gfbymjqvd.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/grrjolkcz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/grolvfiah.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/ggtjowkgj.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gafkeieps.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gfxsngykz.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gnbeypdgj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gzebyoaga.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gnhaswbmn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gmiyjywdq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gzxhuzuur.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/giuflkiqo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/glyjqjpck.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/giyrzvbii.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gjrgvukav.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gwlnksems.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/giilnehna.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gueiymohc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gbcivfyuo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gbrtcyjlh.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gmrtrqirk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gwilertqb.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gemqlwqoy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/goedqptzc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gyqlbtrva.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gxuxeicun.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/grvsqoztx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gjfvdejly.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/guyggfrnn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gkeribpzg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gsrcmvobd.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gjnamvygm.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gztfwgkpz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gknbfbpzs.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gstwanqsi.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gbovvmmip.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gmjyjyoat.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gqnpfqcxy.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gdqrynyvj.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/giaircfyb.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/griulvkkc.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gveexmkqt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gccneyker.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gvvtejypu.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gfjdqldps.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/glhqszjbw.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/gsyffbhom.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gpdkpckyn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gtwbrzkhe.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gvaecbjod.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/geepnconc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gpbsnedsy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gbllfvyzb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gunrzovid.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gqwyfvsfe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gkdubxoyw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/glmxodgmk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjezvsxai.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gkmpmsuhq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gfvtptfpc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gifbpmdes.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gkmgmwvey.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gcsqexysz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gbnfaugmi.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.zdbjq.cn/Article/details/gaddnctfz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/glnjmltne.sHtML


<!-- 参考信息 -->