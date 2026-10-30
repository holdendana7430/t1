代发 wailian999

C#:   list.Distinct().ToList()
来源：http://m.share.fehbvm.com/Article/details/gouxvbhjg.sHtML

[D16] 求和与平均值
来源：http://m.share.zdbjq.cn/Article/details/gfadafeun.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.fehbvm.com/Article/details/ghlgepxsh.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://read.share.hesvh.cn/Article/details/gntrfascn.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/ggfgxdfnm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gfladdyym.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.zdbjq.cn/Article/details/gkjqywznl.sHtML

Go:   // 手写循环累加
来源：http://blog.hesvh.cn/Article/details/gbtvoaxns.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.zdbjq.cn/Article/details/gedeugxdq.sHtML

C#:   list.Sum();  list.Average()
来源：http://read.share.fehbvm.com/Article/details/gavfcvyar.sHtML

[D17] 最大值与最小值
来源：http://blog.zdbjq.cn/Article/details/gmusszrwh.sHtML

Py:   max(arr);  min(arr)
来源：http://www.share.fehbvm.com/Article/details/glduqdvhf.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.fehbvm.com/Article/details/gpypmbwpq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://m.share.hesvh.cn/Article/details/gukuqrjrn.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gyivphryw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://mobile.fehbvm.com/Article/details/gwzxrrizh.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gixpahqaf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.hesvh.cn/Article/details/glowmgqnl.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.zdbjq.cn/Article/details/gzmsivwzj.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gfzflynqt.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gcdohypjp.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gufuvavet.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gcfpnulnh.sHtML

TS:   nested.flat();
来源：http://blog.hesvh.cn/Article/details/gvtifhqlp.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.fehbvm.com/Article/details/gxwduzlaj.sHtML

Go:   // 手写双层循环
来源：http://baike.fehbvm.com/Article/details/gesnhsoqz.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/geuewecne.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://read.share.hesvh.cn/Article/details/gnsccfeuw.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gdvofplyw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.hesvh.cn/Article/details/gwfhmenrb.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gfdbohmhm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.m.share.hesvh.cn/Article/details/gqxcasdzk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.m.share.zdbjq.cn/Article/details/gifqfwlqw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gtssrrvtn.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gzgwqlafz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/goodvjmmf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/gtgblwxih.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/gpzzazwaz.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gcmntbude.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gxpnwpvwq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gdjyyqrmp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gjkjefxcw.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/ghvylqhmu.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/godirmjqf.sHtML

Ruby: arr.tally
来源：http://mobile.hesvh.cn/Article/details/glprqgcij.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.fehbvm.com/Article/details/gfejiemsr.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gqvtshoan.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gviqjfvkn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/gwqvdimjg.sHtML

JS:   arr.includes(x)
来源：http://wap.hesvh.cn/Article/details/gocsxnxil.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/grwtxsmtl.sHtML

Java: list.contains(x)
来源：http://www.blog.hesvh.cn/Article/details/goxpcvvoi.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ghclpautm.sHtML

Ruby: arr.include?(x)
来源：http://mobile.hesvh.cn/Article/details/gzuazlrzc.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gvqdshsia.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.zdbjq.cn/Article/details/gomtkrurg.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.hesvh.cn/Article/details/grmyrtszf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.zdbjq.cn/Article/details/gbmbzwmhp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gpkciernf.sHtML

TS:   [...arr];
来源：http://m.share.zdbjq.cn/Article/details/glcmsbroo.sHtML

Java: new ArrayList<>(list);
来源：http://www.m.share.hesvh.cn/Article/details/gbtvdthua.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/guoaptcui.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gbtugfmxz.sHtML

C#:   new List<int>(list);
来源：http://baike.hesvh.cn/Article/details/glurhdnbf.sHtML

[D23] reduce 累积计算
来源：http://baike.fehbvm.com/Article/details/ghhxqzlwc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gohgocxze.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gkivinedb.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gehurheje.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gpmblqwtt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/glehzjznm.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gxijxmsec.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gtmslejtw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.hesvh.cn/Article/details/gpayolkvn.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.hesvh.cn/Article/details/gnlkotycn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/gmovxtybn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gywncirnj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gtingtgir.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/goryosvbc.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gyrodgluk.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gvrflimjl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.fehbvm.com/Article/details/gwcpavtbs.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gqysgtwlj.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/ghxutvplm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.zdbjq.cn/Article/details/gecbwdcrh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gqelnitue.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gjgybemcw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.zdbjq.cn/Article/details/gukatsdiu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.zdbjq.cn/Article/details/gmiikeigq.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.hesvh.cn/Article/details/ggpjbdhxi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gqzjscfro.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.zdbjq.cn/Article/details/gvwovurcm.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gepwycsgk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gkvyzjtid.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gfdelxflq.sHtML

JS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gyqctqezx.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gqlvqjttf.sHtML

Java: String.join(", ", list)
来源：http://mobile.fehbvm.com/Article/details/gfytpqbkn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.zdbjq.cn/Article/details/gsxoklzrw.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gblkqovhr.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gfxfshvpj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gppewzxbg.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gsikgdlrd.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfofrille.sHtML

[E01] 拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/giypkztph.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fehbvm.com/Article/details/ghezkwtcw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/glmljzysu.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gihidlnqa.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gccrzddlu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.zdbjq.cn/Article/details/gdgbgifsn.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gsnipumcb.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gqznpskbg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/geojaaojg.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gcjhwbcqj.sHtML

Py:   "ab" * 3
来源：http://www.m.share.fehbvm.com/Article/details/gutqkyxjb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.zdbjq.cn/Article/details/gbeurkvzo.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gqiqosrif.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gccnpopnn.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gousocqgv.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gqrtlyiqr.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gqaayberf.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gzweccawu.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gsgjunmqj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.blog.fehbvm.com/Article/details/gxkaaoits.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gezyhldea.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gxpodqkdg.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gjggkmscp.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gkbluodmw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fehbvm.com/Article/details/ggzxhjcdk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.zdbjq.cn/Article/details/gweuvavdg.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gjxwczgoo.sHtML

[E04] 查找子串位置
来源：http://read.share.fehbvm.com/Article/details/gtzuepdwy.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/goxiygzai.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.hesvh.cn/Article/details/gqxyllzad.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/ghicddjmn.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gjtyxcohe.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gxzqqgpxs.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gkjgafjlo.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gujrwvzcs.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gdqvicwty.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/giekgukpm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gfiiwmgnr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gonqzeycv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gxscqzaix.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/ggmuorvzv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gxmdwcfow.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/guippttwq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gkegnfflb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gujsjfmil.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gabkmqxfp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gjwrpyzkt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmybinekh.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/guzovpcjb.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gjismfwgf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gdjxxbctr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gvsyfuykc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/glpkewaef.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gvmbbuhwo.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/gmneywlcu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gcadsifsv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gmgqgxpiw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gfganiiaf.sHtML

TS:   s.split(",")
来源：http://3g.hesvh.cn/Article/details/gttjrmdwo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/gyystyjgd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gldltgise.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gzrflxjxx.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/geujulpac.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/gfsukqkym.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gxdrgjmtd.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/grbsirulj.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gmelbitrt.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gnxxwpqmx.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/godelxxhn.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.zdbjq.cn/Article/details/gzefvpyjt.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gfbwqmsey.sHtML

C#:   string.Join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gtbasviqu.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/ginkyoaiv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fehbvm.com/Article/details/gsbsmkwbw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/ggqtfoxsv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gjsbbomef.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/ggnfwyqkq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gxfjkcmoc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gtwxksmdf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gusnwlpah.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/giyugdaar.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/grcqchmuf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gttviyern.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gmmebywmj.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gavmswwwx.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gfforfele.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gmbcydvgh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gsfxzopfk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gauxcaaju.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gzjcmguyc.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gtkccgyjm.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/geyiedjsn.sHtML

PHP:  strrev($s);
来源：http://blog.hesvh.cn/Article/details/geemvqfyh.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gdkxqodcx.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gnlhrdjhq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/ggkxinqtx.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gpquofcdt.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gkgdmxvsi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gxjcvpiil.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gwzatvaru.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gipijwjmw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gprgimecp.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/grvvfzjvs.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gfyhytyav.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gfcaciwjz.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gmewgwfqd.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/ggdkcalxq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gtsexvnyi.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/ghkzzeahm.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gdmvcgneo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gtkueplhl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/guffeocpd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/ggrlkqfmg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gxfczewiy.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gjldjqiar.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/ggyvvglwa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gkmpwhdea.sHtML

[E14] URL 编码与 Base64
来源：http://wap.hesvh.cn/Article/details/gwdeorgyj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gcovzwfhs.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gzutlfnhd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gswcnzxcf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/goooedibj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gfwxobiol.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/ghagljkip.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gqacfhtdk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gkvhqhybd.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gqimnjdoc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gvrarikcq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/giamngmpv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.hesvh.cn/Article/details/gypwsdtyc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gifxjenpi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gjhmitbbq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gmrekoevh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gslbtybki.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gckrhqlfq.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gzestkyze.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gxuxduyme.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gixsesiee.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gkesbolrx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gllboppyi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gqwvdfisd.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/giuecqkvb.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/ghehokcpu.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gcsxiilyq.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gyjobhioj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/giirqklan.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gzzvufchf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gbbjonrya.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gahctocdw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/ggparyxxt.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gzmumxddm.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gqttfcxsq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/ghgvmoiyc.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gyfifimhs.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gpavelcgz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/grrryxmce.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gchcxbsgp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gohmljcgl.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gzttdckdp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/ghlurrvvj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.fehbvm.com/Article/details/ghijfunhk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gpharozmd.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gzolemmmw.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/ggeoiolbm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gvcyftgua.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gmxrtpeyh.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gpmnayorp.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gszznwufe.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/gsabaorlw.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gyraogdgb.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gvglbiioa.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gpbsrqysz.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gicsuefyu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/ggnuiozvz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gxcjfvwcu.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gimtvyejm.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gccuywglm.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gcufskery.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gqdlozchu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gggqwxjst.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gihqflntb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.hesvh.cn/Article/details/guqbhrdrz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gkdpnttgc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gxevrhuvp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/glbthbhhq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ghprovsyy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gnzaflvlu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gbduqjrvj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gxwqktjxr.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gokvmuaqd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gqtwgxptl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gcdyvgqsa.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gbnwidsqe.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gkadkkdyf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gyvhaweoz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gmfnrakkc.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gsradbthd.sHtML


<!-- 参考信息 -->