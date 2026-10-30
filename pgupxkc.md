代发 wailian999

[D15] 去重
来源：http://wap.zdbjq.cn/Article/details/gnqvsmjzj.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.zdbjq.cn/Article/details/ggiyumgch.sHtML

PHP:  array_unique($arr);
来源：http://www.m.share.hesvh.cn/Article/details/gghufsouu.sHtML

JS:   [...new Set(arr)]
来源：http://www.share.zdbjq.cn/Article/details/gbsonxkax.sHtML

TS:   [...new Set(arr)]
来源：http://blog.zdbjq.cn/Article/details/glxjkxunt.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://read.share.zdbjq.cn/Article/details/gtisylniy.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://m.share.zdbjq.cn/Article/details/gqrytdjca.sHtML

Ruby: arr.uniq
来源：http://mobile.fehbvm.com/Article/details/gjodpwycm.sHtML

C#:   list.Distinct().ToList()
来源：http://blog.hesvh.cn/Article/details/gjeyldrfv.sHtML

[D16] 求和与平均值
来源：http://3g.fehbvm.com/Article/details/gilnrnoyk.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://m.share.zdbjq.cn/Article/details/glgchmqcw.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.blog.zdbjq.cn/Article/details/glgmnsfcd.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gildniqaf.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.hesvh.cn/Article/details/gevyygfkf.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.hesvh.cn/Article/details/goivxwzjg.sHtML

Go:   // 手写循环累加
来源：http://www.m.share.hesvh.cn/Article/details/glriyrlzo.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gbqbssxzj.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.fehbvm.com/Article/details/glwjkxuse.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/ghocyqulq.sHtML

Py:   max(arr);  min(arr)
来源：http://mobile.hesvh.cn/Article/details/gstfejhpe.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gbvebgzfo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/glhnuthtq.sHtML

TS:   Math.max(...arr);
来源：http://www.m.share.fehbvm.com/Article/details/gucxnztlp.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.fehbvm.com/Article/details/gdvggpmdk.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/gvupggeke.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.fehbvm.com/Article/details/gbveweyfa.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/grqfbvrxa.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/gnpozvuud.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gfxslhqwn.sHtML

PHP:  array_merge(...$nested);
来源：http://read.share.fehbvm.com/Article/details/ghknefejq.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.zdbjq.cn/Article/details/gzrawrlqt.sHtML

TS:   nested.flat();
来源：http://m.share.zdbjq.cn/Article/details/gbclhbcaq.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gzdfaqazj.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gtgjeduii.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gmoeiovyr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gpqawjcmc.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gumopmtfz.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/ggqqxdkgq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gzlzfnovj.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.zdbjq.cn/Article/details/gakqsoivh.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gtowscxer.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gbdrhgwkp.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.hesvh.cn/Article/details/gtmvkqtxa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fehbvm.com/Article/details/gpkmzolah.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gatylwgup.sHtML

[D20] 统计每个元素出现次数
来源：http://mobile.fehbvm.com/Article/details/gvedvresf.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/glavdnfie.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fehbvm.com/Article/details/ggekvcrgn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gtuqetevz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gsyxurihq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/ggzzaenvh.sHtML

Go:   // 手写 map[T]int
来源：http://blog.fehbvm.com/Article/details/gjtxfpqre.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gumdaoowj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gxaqroleh.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gwrduawdm.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/gtcxbrwga.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.m.share.hesvh.cn/Article/details/gimkydork.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/gqpvxephr.sHtML

TS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gchmkyjgw.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gjkiobzue.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gjodtrgzs.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fehbvm.com/Article/details/gbxfrpmsx.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gcbcysojz.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gmpubpjuq.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/graowshgm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.hesvh.cn/Article/details/gugwkrmtd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/guzldfgrl.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gmrgsrblq.sHtML

Java: new ArrayList<>(list);
来源：http://wap.hesvh.cn/Article/details/grvmowqsd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.hesvh.cn/Article/details/gyzirehop.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.hesvh.cn/Article/details/gtylrxnhm.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gkwcnyefs.sHtML

[D23] reduce 累积计算
来源：http://3g.zdbjq.cn/Article/details/gztexjmhb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/gdovfdwjt.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.zdbjq.cn/Article/details/gdzhijpwt.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gwsrdahmk.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/grxauqkhg.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gyrczzkaj.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gxdptzdav.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.hesvh.cn/Article/details/gedwkeded.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.zdbjq.cn/Article/details/ghmjvsojw.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.zdbjq.cn/Article/details/gjpoahnnp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.blog.zdbjq.cn/Article/details/gzamuarkx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/ghkqgqszu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gbtnupbfd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gwzbvvjko.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gnzhkgmlk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gfwchysbl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.zdbjq.cn/Article/details/gbioznvsv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.fehbvm.com/Article/details/gdanruazi.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.hesvh.cn/Article/details/gqnkhvfuu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gzghadvnz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gjnzsqbbi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gufosqvom.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gxrodsiek.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gdteojxis.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.hesvh.cn/Article/details/gvhymahfg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gvsmqqour.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnbiuildc.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/grljvxfbc.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/ghfwlwikd.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gtnehmsyb.sHtML

JS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gjxfaviwh.sHtML

TS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gzuyjsmuf.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/guwkmqfbw.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.zdbjq.cn/Article/details/ghmacsgmj.sHtML

Ruby: arr.join(", ")
来源：http://read.share.hesvh.cn/Article/details/gzjfhxfzx.sHtML

C#:   string.Join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/ggscawrgg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbkiernox.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/gushxmjdt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gcvkkvlbg.sHtML

[E01] 拼接字符串
来源：http://baike.fehbvm.com/Article/details/gwedyyiyv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/goawhxaaj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gmxwqjsno.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/grxcjcjat.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/grhksyggs.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.fehbvm.com/Article/details/gadejcbwd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gsurjotmy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gpvpvfubh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gtuwwunfi.sHtML

[E02] 重复字符串
来源：http://baike.hesvh.cn/Article/details/gutfilaha.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/glrctwxvs.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gznetjtmg.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gxgkzusin.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gdmgimhrk.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gfwujldzz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/gdefinqpp.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gjtqkdblb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gzxosllxn.sHtML

[E03] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gbbpuwpez.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.fehbvm.com/Article/details/gykqxqotf.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/goyceccnk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gwseyrwtr.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gwqgbmqqg.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gbsijafyk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/gwgkjaoiq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gasarlcrn.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.zdbjq.cn/Article/details/gokxqflud.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/gzzwqorcb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gmqtmapwa.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gkknxovwi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/glqjxikea.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gudfmsnzm.sHtML

Java: s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/ghoyrhcfn.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fehbvm.com/Article/details/gbauyysja.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gmzxxpzgv.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gsihtovsg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gmhsjwhrl.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.hesvh.cn/Article/details/gdrufbbyd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/gjlmqppso.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/geqqsbelg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gdsmhzosd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gqkzvixjm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/ghorrcvkm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.zdbjq.cn/Article/details/gqpvjgjlh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gpnaofggw.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gceccylpg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gxwvcmpzd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/giaangamk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gelzolsit.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gepdmeqix.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gkevvsmsv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gcxdsknxy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gyjnzpthq.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gijnzigwu.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/glwgohznv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gcxegzksg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.hesvh.cn/Article/details/giryvffdf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gbzkadrqd.sHtML

TS:   s.split(",")
来源：http://3g.fehbvm.com/Article/details/gpmsessuy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gqeoizppn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gqiqxedmf.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/guslkogyw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.zdbjq.cn/Article/details/gekkckogv.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gxxxsjpqv.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gkxmwerge.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gywmbyuoc.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gdcfnanun.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gpdoyrlgg.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gbbpwqnbj.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gqvenhkur.sHtML

Ruby: items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/gxsvrzqow.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gzkzslqed.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gstbahhie.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gbcgsssse.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gxqhfnwhh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gpgrmecfc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/ghbcbfgio.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gndrslefc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gzvtoufmf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gtfgbrvgu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/geuchqnyj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gyrljjetf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gclzybumh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/gmeyonurm.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gqrnfsiky.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gjpwqqipm.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gebmwjafy.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gnnffpvhm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gxjgaitze.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/gdsjdmjtr.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/glqlszfav.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/ghgdqhnmh.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gletdepwl.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gmoetenpi.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ggnlxqdst.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gofcmwvvc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.hesvh.cn/Article/details/gtwdcuzqq.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/ggbxazoei.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gjiblwsnq.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gwvuboaqi.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gusqrqfyw.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gtymuvjpa.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gnqukelin.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/geadjbvrt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gbtlowdgt.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/gtlvngizs.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gjaqoktnd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/geqqtpwjc.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gpuuhpsjq.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/ghaobrijg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/ghbwnnzin.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gxofbiiyt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gmdpxmhmo.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gvimrrjtn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gigunoquv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/graxmrrvw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gbxlbutew.sHtML

[E14] URL 编码与 Base64
来源：http://3g.hesvh.cn/Article/details/giiyzxlla.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/ghzyzdymw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gekunhgtl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/guxufmnmj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gobluvqwr.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gvbozrziw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/grdqwghpf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gcbqlzuzp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.zdbjq.cn/Article/details/gkohvakkt.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/golpsnkgh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gugjhuuwo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gjrleubzg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gydvgemzu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/grjamewor.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gdzzfcbho.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/ghbvkbodo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.zdbjq.cn/Article/details/galmskrdb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gusmcnrms.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gqksddvnf.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gsqpgmsxy.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/guwujyxgc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gjwlfvfop.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gqwaohcgm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gmrlgymkp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/glguhgfap.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gexsroamr.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/ghnzsbkaz.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gipziolzi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gsrvlvxrb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gmqzohlcn.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/ghnbhdqqt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/grlpbilur.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gbigfywpa.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gsnpafphn.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gaygdefpw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/ggvvbzgnn.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gzlcncayx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/glqvmmkwa.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gbdntqyqr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gvayywinn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gpksmnfih.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gqduodnxk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gyjtkhpxo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gxqfrsyao.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gyenfasvz.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gktakhmuj.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gchivgfgo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gkhrfhkmj.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gznlomzln.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/goftztlnf.sHtML

Java: s.lines().toList()
来源：http://baike.fehbvm.com/Article/details/gdhkksfvh.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gheocljag.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gezxfgawq.sHtML

C#:   s.Split('\n')
来源：http://mobile.fehbvm.com/Article/details/gmkhfifyg.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gqlgwubqu.sHtML

Py:   if not s:
来源：http://baike.fehbvm.com/Article/details/gfeyebncq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.hesvh.cn/Article/details/gtdxyrujq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gvqjisgsk.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/gshzxrymx.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gswmrpnin.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gfwelgnmq.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/gzspsexnl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geusdqoxu.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/grzeikmak.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gysehmyeb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gvfkoemiq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/ghbynmbuq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gxkskelnr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/glmdpcqsh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gffvmpimf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gnsfajyhn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/ghflhwgbu.sHtML


<!-- 参考信息 -->