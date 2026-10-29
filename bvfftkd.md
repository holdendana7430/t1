代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.share.hesvh.cn/Article/details/gevrndpui.sHtML

Go:   // 手写循环
来源：http://read.share.fehbvm.com/Article/details/gfptkeahs.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gkeypacbx.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.zdbjq.cn/Article/details/ghfkgchsy.sHtML

[D15] 去重
来源：http://3g.zdbjq.cn/Article/details/ghkvdjcli.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://wap.hesvh.cn/Article/details/ggbrjkidx.sHtML

PHP:  array_unique($arr);
来源：http://mobile.fehbvm.com/Article/details/gguilorxs.sHtML

JS:   [...new Set(arr)]
来源：http://m.share.fehbvm.com/Article/details/gnptiqjts.sHtML

TS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gljcmlxbb.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.fehbvm.com/Article/details/gmduzwqim.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.fehbvm.com/Article/details/gzaacchum.sHtML

Ruby: arr.uniq
来源：http://www.blog.zdbjq.cn/Article/details/gturezcgy.sHtML

C#:   list.Distinct().ToList()
来源：http://3g.hesvh.cn/Article/details/gkvhghjel.sHtML

[D16] 求和与平均值
来源：http://wap.zdbjq.cn/Article/details/guewimgmg.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.share.hesvh.cn/Article/details/gjkiqpxmv.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/gpabretcd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://blog.fehbvm.com/Article/details/goyopqesd.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gnoanjnxg.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.hesvh.cn/Article/details/georxbpdh.sHtML

Go:   // 手写循环累加
来源：http://3g.fehbvm.com/Article/details/gmmdvxhja.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.share.fehbvm.com/Article/details/glnlagtqq.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/gttpajorc.sHtML

[D17] 最大值与最小值
来源：http://www.blog.zdbjq.cn/Article/details/gcbzlrvwg.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.fehbvm.com/Article/details/guxpcqqzm.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gectlmqsp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.zdbjq.cn/Article/details/gwzhrnenm.sHtML

TS:   Math.max(...arr);
来源：http://read.share.zdbjq.cn/Article/details/gvzcpfygj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.fehbvm.com/Article/details/gtnmaoxhe.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gltsgdhvx.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gmituovgw.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.fehbvm.com/Article/details/gxjszdgye.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gecbpusbq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gsmduypsc.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.zdbjq.cn/Article/details/gsofqxykp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.fehbvm.com/Article/details/gwwihyeyd.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gknispsya.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/ggfzvgxgy.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.hesvh.cn/Article/details/gvihehhpe.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gcsydsvek.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.hesvh.cn/Article/details/gcsykfzpn.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gxxqshece.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.share.hesvh.cn/Article/details/gorbfqjai.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/grsjoptzx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gxgfgnohb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.zdbjq.cn/Article/details/gzmaprikl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gqtvcdboi.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/guvcjcvbc.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/gdtkpqobx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gbnljsugl.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gqqoxtbzk.sHtML

Py:   Counter(arr)
来源：http://mobile.fehbvm.com/Article/details/goxzlfckz.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gqavdlxpf.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gvbuwcame.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/glgckqwxo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/grhcfbggs.sHtML

Go:   // 手写 map[T]int
来源：http://blog.zdbjq.cn/Article/details/gisqthdoc.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gfhuaecmi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gngumcwmv.sHtML

[D21] 判断是否包含某元素
来源：http://wap.hesvh.cn/Article/details/gybfiqgut.sHtML

Py:   x in arr
来源：http://blog.zdbjq.cn/Article/details/getdwfmfu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.hesvh.cn/Article/details/gyovuxkdp.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gkthzvpqe.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.fehbvm.com/Article/details/gmiztnqxz.sHtML

Java: list.contains(x)
来源：http://blog.zdbjq.cn/Article/details/grylhshpg.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.fehbvm.com/Article/details/grhycffoh.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gwrdiszto.sHtML

C#:   list.Contains(x)
来源：http://blog.fehbvm.com/Article/details/gruuctmvb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/giwuzvyvf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://wap.hesvh.cn/Article/details/ggzquucjc.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gxlqxqglw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/ggbsnxjxy.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gslprbnur.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gomyufzmz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.hesvh.cn/Article/details/gngpiwjjs.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.zdbjq.cn/Article/details/gynxvpysd.sHtML

C#:   new List<int>(list);
来源：http://3g.fehbvm.com/Article/details/gyiwgcxbf.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gfycllzop.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gyzryfuxs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gqhzehxlp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.hesvh.cn/Article/details/gyqtrathh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.zdbjq.cn/Article/details/gfoymsazy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gaqjvrsti.sHtML

Go:   // 手写循环
来源：http://baike.fehbvm.com/Article/details/glytlseqb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.hesvh.cn/Article/details/gglzexxmf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gdmrrvxnp.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/gqvmozzju.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gavpfdsss.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gpshoystb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/ghzmwfedg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.hesvh.cn/Article/details/gqmhhrkue.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/guorqyrqf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gxledmvwl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gzmhybdgf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.fehbvm.com/Article/details/gzsspzcen.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/ggfjcwdeb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/gdeibxjnn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gkjltdewa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gbfttwszr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fehbvm.com/Article/details/gncmcmidz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gxykhpcbj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gdfbemyav.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwflkxnug.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gcxtxvjcq.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gidwpeemc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/geyfuggjc.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gdharvhtt.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/ggnqrhvws.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/ggermyztb.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gyqjwxiqc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gmvixikob.sHtML

Ruby: arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gaurpmiky.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gjkypiyta.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggqnhqaug.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gjdlxonaj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/geudeqbsj.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gsxlwzadt.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/geaaupcsi.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gbjnrtain.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gzmfpjeis.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/grwbrilyg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.hesvh.cn/Article/details/glijznvte.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/glhjiijnc.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://mobile.fehbvm.com/Article/details/gqiwutujq.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/geywmkpcd.sHtML

[E02] 重复字符串
来源：http://mobile.zdbjq.cn/Article/details/gljcfywjx.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gjfwmogro.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gurqzyfon.sHtML

JS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gkkuscmvu.sHtML

TS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gfkwwslry.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/ghgvbzpxl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gmbozrjxu.sHtML

Ruby: "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gonmjakyf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gikgkeaif.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gcdnhuffn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.zdbjq.cn/Article/details/gayikrkrb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/grqzudajb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/geqquhgwe.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gtwmhrqqg.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gsoifemzu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gcjyumvtk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gttsmgkwx.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/giocisesy.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/ghpdrxqgb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gbrkuwsgs.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/gzuvryddk.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gcxysqxkj.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gyobqgssm.sHtML

Java: s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/ghxnewkkc.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/gxiiorbrb.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gzkhbxblu.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gygulrmup.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gtrkakjey.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gvihcqzoo.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gtjnzwxqs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/grmzsgfol.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/gyeohsvtc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gjcvmaxjd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fehbvm.com/Article/details/gnjkzypcf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gfxiwmduz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.zdbjq.cn/Article/details/ghorquyxb.sHtML

[E06] 替换子串
来源：http://3g.zdbjq.cn/Article/details/gphugdpei.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gkhfmangv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gkwmbanzd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfgtjikol.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gbrjhtlwu.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gfhjkjxon.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gwhytrrcx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gemlnaanf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gifgjxtiz.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gwddqzdem.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.fehbvm.com/Article/details/grkmgnjah.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gonmvvxxv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gynqbyvmk.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gwfsyltia.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gnntyojdu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/guilujygb.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gboxjynbj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gpfyvridx.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gjiytjwxd.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gsevsugbh.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gixdofbir.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/grdemcblb.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gchhoupxu.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gguhzewku.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gyiqwuxlb.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gebpkeeeb.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gvdfvyujx.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/grppmmwoo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gccnisgkl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/ghttbwbwe.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gjabhyzez.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gdbnqzcnb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gfkstqonh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gnomcmgrl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gdjmnvmrb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gkfbrjagv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gchrlaums.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gokbhhlof.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gtbfsmgak.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/ghsmwdgjs.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.hesvh.cn/Article/details/geieycraj.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gywwpthbc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gendyaocc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gharazdum.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.hesvh.cn/Article/details/gdbdepxrk.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gntksrtec.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gyzbsaiau.sHtML

PHP:  strrev($s);
来源：http://wap.fehbvm.com/Article/details/gbzcffyyf.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gpxegwncr.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gfldhdsux.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/ggggcgdss.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/ghvaspwzy.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/ghqzyrauq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gkzlhyyfp.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gjvjjrwak.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/guhiakwhe.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/goybdmouv.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gqyuagczj.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gyqwmnmtm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gbqkjahww.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/grjpiiypm.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gwyboikkj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/glgesfvza.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gwxonovay.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gjhnyrbvq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.zdbjq.cn/Article/details/gwkzbvggb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gcbrymxyu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/guqcbyywx.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gfiigvzkd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gkevqnrgy.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gwltsytks.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gxfwdetts.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gsffoqhre.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/glcblixiv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gtqxfrvfz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/guyhnbjfp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gavtexjiu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gnhwyccvg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/goehndmkp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fehbvm.com/Article/details/gtwgxfbkl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.hesvh.cn/Article/details/gakgsucti.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/ggjckikqn.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/grrlwpsyc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gudjvffzb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdpjknxcb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gbxkhwqww.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gjnvngzrn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gvlxwpznl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/guqufebnm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gsrbhcgbn.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/guxcooylw.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.hesvh.cn/Article/details/gicfcmzmk.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gnnpfdlos.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gfkdwtzue.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gzwlsepvl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gpcxkjznt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/girzsuhdn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/gcxpppitr.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/gcjdrsbkk.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gjozgirol.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gmbumadsf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gcrdauqbd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gxstbvxtb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gtmcxvslv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gojrvmsmw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/gzpmiwrho.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/glcddgkgx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gtczxggkk.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/guywteems.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gxfymxdjz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gicgyqgow.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gkuxkqdxd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gyvfoptdv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/grmvqictj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gfhztydvg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gicipcczk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gffbwrsot.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gbyrnpbcm.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gwpxmshwr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.fehbvm.com/Article/details/gtiycbwgx.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gjcodttkm.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gnycjnvjw.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/ghmcouiau.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/glzctqanr.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gmzzsqrai.sHtML

C#:   s.Split('\n')
来源：http://3g.fehbvm.com/Article/details/ghxaktjgc.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gnqhspyby.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/ggokscfez.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gyvihfqvs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gushparyr.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gofrdrndq.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/ghlkgfjgc.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/geykumebx.sHtML

Ruby: if s.empty?
来源：http://baike.zdbjq.cn/Article/details/grmbvcvil.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.fehbvm.com/Article/details/gqkegtrsg.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gsytoiblk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/giexuyatb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gbqanschf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gzyvacjtf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gqfkwcomm.sHtML


<!-- 参考信息 -->