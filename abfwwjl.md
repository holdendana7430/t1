代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gmxhtexhu.sHtML

C#:   list.Sum();  list.Average()
来源：http://mobile.zdbjq.cn/Article/details/ghjnrckgv.sHtML

[D17] 最大值与最小值
来源：http://read.share.zdbjq.cn/Article/details/gtrxxultl.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gihnpqpta.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gnqhlitzg.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/ghhcngsxa.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gswpdhqlg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://www.share.hesvh.cn/Article/details/gjrqtktms.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://m.share.fehbvm.com/Article/details/gxhqyqqgp.sHtML

Ruby: arr.max;  arr.min
来源：http://www.m.share.hesvh.cn/Article/details/guwqggfld.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.hesvh.cn/Article/details/grajicbne.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gbwjbwyft.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.fehbvm.com/Article/details/gsnxhhfgf.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.zdbjq.cn/Article/details/gfvtmkagx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.fehbvm.com/Article/details/ghubtujyl.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gxakrpslk.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.fehbvm.com/Article/details/gblxxtapy.sHtML

Go:   // 手写双层循环
来源：http://read.share.zdbjq.cn/Article/details/gxtfpfxgt.sHtML

Ruby: nested.flatten
来源：http://read.share.hesvh.cn/Article/details/gcqgkxxde.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gsetohint.sHtML

[D19] 按字段分组
来源：http://mobile.zdbjq.cn/Article/details/ghiwelvcn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.hesvh.cn/Article/details/gdqyzgwyu.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.hesvh.cn/Article/details/genieilli.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.hesvh.cn/Article/details/gyfoxmusu.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gnasihvti.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gaotggrvn.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gmyllpvsl.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gulczbcjf.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.zdbjq.cn/Article/details/gneazercp.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.fehbvm.com/Article/details/gotnumvtq.sHtML

Py:   Counter(arr)
来源：http://m.share.fehbvm.com/Article/details/goeuucwvq.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gbcwlrzdd.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/gyfcinugj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gjoqvihhv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gfxpxkksa.sHtML

Go:   // 手写 map[T]int
来源：http://baike.hesvh.cn/Article/details/gfulhzntr.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gzfcrlchr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/ghsbtwdlp.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.hesvh.cn/Article/details/gkynbnkru.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gvqoptrhf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.zdbjq.cn/Article/details/gknrfvyoy.sHtML

JS:   arr.includes(x)
来源：http://www.share.zdbjq.cn/Article/details/gkchrpzlq.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gkevicevk.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gjbvwasmf.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gbkdlzsxg.sHtML

Ruby: arr.include?(x)
来源：http://m.share.hesvh.cn/Article/details/golachrhw.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gmvygonmk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://mobile.zdbjq.cn/Article/details/guhxvmlwr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gkecjovtx.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.fehbvm.com/Article/details/gpscpqjal.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gyfthwouv.sHtML

TS:   [...arr];
来源：http://read.share.fehbvm.com/Article/details/gmarubsco.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gdurvoufa.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gtutoucmt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://baike.fehbvm.com/Article/details/ggvyojips.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gpwjxglgg.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/geemojcup.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.zdbjq.cn/Article/details/gdplxsmkp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/gznnlofqd.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gxxxbekkv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gnvdmalww.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gisefwxzi.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gmfllypxz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gviapeqfe.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.zdbjq.cn/Article/details/gkdrfytis.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gqybuwidc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gmbhzwppr.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.hesvh.cn/Article/details/gbsairkit.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gzsgmstxr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gsjqsftru.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.hesvh.cn/Article/details/gmdnbjwtr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/ghlyktpbu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/grautcmgt.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gdghjwndb.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.zdbjq.cn/Article/details/ghwhgrrac.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/gjteyihro.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/gcllkwlyl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gcocndywh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gloyunbfw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gwpvrgnim.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gdxhsfixl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gtavwaiar.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gepchfqyw.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gifvdrxdg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gqpigggfh.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fehbvm.com/Article/details/gfxdbqgha.sHtML

JS:   arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/georwdodd.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gfhgjhkpa.sHtML

Java: String.join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gdwqnklda.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/grwnhuthm.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gisyjqjpa.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gpumccgxw.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grhqkqodh.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gqpwlnleb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gijbgoqiy.sHtML

[E01] 拼接字符串
来源：http://3g.fehbvm.com/Article/details/gcvjutitz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.fehbvm.com/Article/details/grnclmxhd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.zdbjq.cn/Article/details/gnjalojqe.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gsvvyhqjh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gqqervswp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gsrdmdgns.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.hesvh.cn/Article/details/glnqitdsr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/ggxzmxpao.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/ggqpvuvvd.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gujjlwvpk.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gqwqjldqw.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gbqhpiibf.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/giirvtiut.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gbwoiigty.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gmnphraon.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.fehbvm.com/Article/details/ggmkxnseo.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gxrnscrpp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.fehbvm.com/Article/details/gfuqovkvb.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gfjbvqwjm.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gxjyibysx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gbigtonxb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gdytdfcfx.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gnlletlxh.sHtML

Java: s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gdpdytfgn.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gcyicrvzu.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.hesvh.cn/Article/details/gnyocsmeb.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.zdbjq.cn/Article/details/ghvvlycbs.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/grdzcjpnf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gvwipizmx.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gkukldlrc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/goyrpnufg.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gpytnvhcg.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gmhayyghm.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gsqdnmuxp.sHtML

Ruby: s.index("x")
来源：http://read.share.hesvh.cn/Article/details/guuxuupfh.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gvdyerccj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gsjifvfja.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/ggxoeiius.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/gieggdcqj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gunccwvax.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/giotcagjo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gzhhnxmpn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gnzzmvogz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/gnadngzst.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.zdbjq.cn/Article/details/ghjkthqun.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gldravygf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gckysmucq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gcgkgfbvi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gapqezqvv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/grgjbygzi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gkkdbqpdf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/graahtquw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gvvgfuczm.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gkiihpqyz.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gyujtbunb.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gbmflibro.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gfvnmetqb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gddoqxydi.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gpkvctdyv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gypgngxvt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcrpxylse.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gbwdfslxc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.fehbvm.com/Article/details/gjbkqvgle.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gbftgecir.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gucfirarf.sHtML

PHP:  implode(",", $items);
来源：http://3g.fehbvm.com/Article/details/gvqpymjck.sHtML

JS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gbztkscas.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gmhnldqvu.sHtML

Java: String.join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/ghijnfzbn.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gulmltzeg.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gyeikrped.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gfsnnlvcw.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gwrknksyh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gfjftyixf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gdztsoytf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/geurkqidw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gxgyzpgqc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gwvyzptie.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/ghfnxtugj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gtwqtornn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/ggkxbbngl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gobilcnuy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gokirnlyw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.zdbjq.cn/Article/details/gicjaagxq.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/grzyvirno.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gbcuuqutk.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/goeldimht.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gzpxsbybm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gutjravnj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gklcfdkmk.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gzqwrwnhb.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gwkyssqop.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gwrkyrtsq.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gascltysv.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gygffszlx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/grrsbukwe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/glglefwmz.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/ghqdsvtya.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gxvjrxeah.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gmfaenmyg.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gnndukywi.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gtrgyxpdy.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gbqqsptdh.sHtML

TS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/gcskyfpel.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gjqjgnldn.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gmghvoise.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gjjgmjnuh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gxswjtxcu.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gsjipfwai.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/ggmsxqvlb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gmmlcqkfc.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/guhwwcrvg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/glnuidcjw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/goyuohozk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gaoneosrs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gckinqhlk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gprhkqyvs.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gibtrysnu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gbmqmjjsz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gxywchvdr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gagctermc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/galnreeng.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gaskbwsqp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/gyyakhtdn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gubhgafep.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/gzorcavxb.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.zdbjq.cn/Article/details/gudgetkvm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gkwewmeau.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gzkhqdrrs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gawtutaqr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gxmxzjrov.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.fehbvm.com/Article/details/ghpvxdedh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.hesvh.cn/Article/details/gdupogauo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gidupvxym.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gbfgsptux.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/grkaphiqh.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gxkirdrew.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gqjpcpbkh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gcwwtnahh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gouiwcbwh.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gcgbavnvo.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/gkbdcqzcu.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/galeigucq.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/ghrpyovmr.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gzlrunfdg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/giplzukbg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gclsfwtqf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grztydobw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gtvtbyxse.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gzyiliyfi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/gjftqabcu.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gynohmptm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.fehbvm.com/Article/details/goywjcrbg.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gvirnfvnt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gisrxbvco.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/ggrbzkjjr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gqsccrvsz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/glgthohiq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gujibauvk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/ggwfyamdj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gcslyulel.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gxkqcoryu.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gcsstcsaf.sHtML

Py:   s.splitlines()
来源：http://wap.hesvh.cn/Article/details/gazjgyxmc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.zdbjq.cn/Article/details/gfvjyizrm.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gnldctlcw.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.zdbjq.cn/Article/details/gpksthxdn.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gyniiwqlx.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gfjyjrzvs.sHtML

Ruby: s.lines
来源：http://baike.zdbjq.cn/Article/details/gmbzqjfkx.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/ggpwecjgp.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/giowzihah.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gvdhwjdtt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gcyjekqwn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/giutmhiun.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gmwzysyai.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gwlfkafqj.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gfrlpqrqw.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gjiaguisf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gcphltcms.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gqpppwpii.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.hesvh.cn/Article/details/glehnybeb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/ghnnlzxrs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gktylolsv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gcnyfkmug.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gasuaautz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/gqvvwbehg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gwqfeevfl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gtkjmzohf.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gctwqsxia.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gqhjebuzj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gegimqiyn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/godfguuxv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gwbhnwsxa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.hesvh.cn/Article/details/gnadrcavr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.hesvh.cn/Article/details/gvvwewdtn.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/grhawkneu.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gmjlxhsrj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gseigkhzv.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gemolmwna.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpyvtjbxi.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/grskplwwa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gjfsgyfxq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gvivuuzlv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/guajafbqm.sHtML


<!-- 参考信息 -->