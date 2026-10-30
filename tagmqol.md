代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gzecupbnz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gnjsjmvec.sHtML

Py:   Counter(arr)
来源：http://mobile.zdbjq.cn/Article/details/gltdoccrf.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/gcdjwmnuo.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gewafhsyi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gcwnnfziy.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.zdbjq.cn/Article/details/gdrjvpeli.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gxzmobucd.sHtML

Ruby: arr.tally
来源：http://baike.fehbvm.com/Article/details/gebrokdzx.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.zdbjq.cn/Article/details/gndoxoeut.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gzrqonqqw.sHtML

Py:   x in arr
来源：http://www.blog.zdbjq.cn/Article/details/gtdsrrmnt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/guhehzjdr.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.hesvh.cn/Article/details/goscjubgj.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/ghhgqivfc.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/gnzirfsxx.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gbajvtaoe.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gtypcecvm.sHtML

C#:   list.Contains(x)
来源：http://www.share.hesvh.cn/Article/details/godmkrgje.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gaigdfqft.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gsvzjeglz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gieyjqltw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gdnaunwrq.sHtML

TS:   [...arr];
来源：http://www.m.share.fehbvm.com/Article/details/gvosqdfme.sHtML

Java: new ArrayList<>(list);
来源：http://baike.zdbjq.cn/Article/details/gapddjefg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gdsrcgpnr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gvgbaounz.sHtML

C#:   new List<int>(list);
来源：http://read.share.hesvh.cn/Article/details/gdxdupzlw.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/grzpvtbcl.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/ggqrbknpv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.zdbjq.cn/Article/details/gyaibapci.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gyrzgjkfl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwpgdmqtc.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/gkdpxdayd.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/gqkhzvwku.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gpxkjqrpi.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.fehbvm.com/Article/details/gknycyncb.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fehbvm.com/Article/details/gkmtokcut.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gxgztnxtx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/goqbmstwx.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.zdbjq.cn/Article/details/gekomurac.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gtzmdjnox.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.zdbjq.cn/Article/details/gftgcvzsm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gdjgocxrt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gwwiyirjg.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gvdptbkxh.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gnzyzobdq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/ggiwgnduq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gapuwsdfw.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gvprffxvm.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gokwuvbxn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gmtrwdgpu.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gxctccajr.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fehbvm.com/Article/details/gfffvhtda.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxksurmlo.sHtML

[D26] 数组转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbdiunpbe.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/geqsytivr.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/gyphalaqq.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gkdzzbvwf.sHtML

TS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/gauhdqgji.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gifvawlqe.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.hesvh.cn/Article/details/grkxvczfw.sHtML

Ruby: arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gonpjpqet.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/grkqtdadu.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grdzsmjtv.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gxayahlui.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfelsjway.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gzzhrrnfd.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.fehbvm.com/Article/details/gsewjyzad.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.zdbjq.cn/Article/details/gdfxltbto.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/glhkbiuwy.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gnmddjvfh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.hesvh.cn/Article/details/gpjenfucu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.zdbjq.cn/Article/details/gbybplnuy.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gwmiwdyrs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gbkzzuygp.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gipvvserq.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/ggwgdnnga.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gkchjwhqr.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gibncsqsq.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gorwsvwnw.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gsxjivtzi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.hesvh.cn/Article/details/gvgqthksv.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gxvcqrxee.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gvwvpggly.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/gpbhsmgvs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gfxozyzbz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gnymadzgb.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gqsldinzy.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fehbvm.com/Article/details/gfengmxli.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/gnvdafgwr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gnvuozgiw.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/glzwrogll.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gwksavybd.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gpjbaeskl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gzjafruvz.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/ghhgapsdj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gitdrhuko.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gzzzjobvg.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/ggbnpjtbe.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.hesvh.cn/Article/details/glekygfzs.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gwudwdleb.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gnnjkamfn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gnfigqpbx.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gvlzvdhjk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gmzhenzsz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/grbiqfres.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fehbvm.com/Article/details/gyjpoatci.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gljvcafxm.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.zdbjq.cn/Article/details/guzjawtdz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/guqnkxaea.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gdkaxdopr.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gvdqwrhvp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gzbvhlwvs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gfepownlp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gminbovxj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/govtypytq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gjshyvodd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gkfpuvdhb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gwbutpgxi.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/giigzphzh.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gjqeemmwp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gmaezabpy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gtphjamnf.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.zdbjq.cn/Article/details/gnlazdito.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gunnuzsuq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.zdbjq.cn/Article/details/gzaypaegd.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/grwbdjsoa.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gmqtmiwde.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gzcarvecv.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/gwkepxotw.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gisrlnzwi.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gcijdmamw.sHtML

JS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gocfsyjxc.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gtwipawtj.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gtjiafdnd.sHtML

Go:   strings.Join(items, ",")
来源：http://www.m.share.zdbjq.cn/Article/details/gsrrhnskq.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/ghpcshckg.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gkoamjiuc.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gzyjctzlq.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gxekktiql.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.fehbvm.com/Article/details/glbiokfhd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/ghqhgxqbz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gytdrgaoo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gksffszfa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/glgumwqhj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/glltrdqrn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gtutuexyq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.hesvh.cn/Article/details/gkpewxxoy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gangkohfp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gemqfilyj.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gnkcfbfxb.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/ggrfhxsbp.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/ggobsoamz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gjpwjwqwl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gqtgmskhl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gccmfquzc.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/gijgpvwah.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gyxhcsend.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gliizbhqr.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gptalpbeo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gtrctvxbl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gvnrbklxg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/gctndqjkq.sHtML

Ruby: s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gktrwnpjz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gaedxkiuw.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gfppgscwz.sHtML

Py:   s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/gavarywpo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gggynhfcf.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gtvabgger.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gnrqaovee.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/giehutyde.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/grlrnzokq.sHtML

Ruby: s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gilwiwnnx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gluvtzhbk.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gqnklykrb.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gcntxxojv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gvumqwlrw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gwsfmzkpd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gzlpyuuzv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gaziqvuib.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/giiflzuen.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gtuaxkuig.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.hesvh.cn/Article/details/gggazllpx.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gbxavxghm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.zdbjq.cn/Article/details/gtbjtfbye.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/ghpcepuxz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gbgfpxqkk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/ghibntzki.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.hesvh.cn/Article/details/gbykcfuoy.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gyeuvwilt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gkzfcvgcq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gckvqdcdt.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/ghbfblsge.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpounknkz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gbuztshxw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gglqjykri.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gfyinfajw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gqudcmigq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gxpuyjbyf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gzvenojcc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gbaeotvky.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gvtzdmbaq.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gnyyogfic.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/geiovkonu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gikhixgao.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gjxfxxhby.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gqigvudtq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/grtoqtfsv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.zdbjq.cn/Article/details/gyeourirf.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/ghuopskyx.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/guntztkpj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gkxrhiewj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gbksmzlak.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gzvgvgovy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gbcsydezh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.fehbvm.com/Article/details/gtvgsswca.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gjkgbauan.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gdjknfndw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gaihsyijm.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.zdbjq.cn/Article/details/gbxfjwesk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/grwtxdqch.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gznadfwrh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/ggenrwbxp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/geihrxcva.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/glsmdjtkb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/geokystyn.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gfttqnsre.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gmfqpbjlv.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gtujazsww.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/ggmngfdie.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gqkuxuqij.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gdsqmgngy.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gvapizkit.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gzpltpszz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gmcasychh.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gypgnfpjt.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gpanykdvz.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gxtvqgdtw.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gipfcyzyu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gqhjvcdgi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfxvmvmdb.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/giounwlts.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gxeppzddu.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gmjrimalv.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gpsdfbsvh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gqnyncgxk.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/gmcjtqqay.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/grhltebdn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gykunqbnh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/goteenbkl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gvusturym.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ghetunatw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gdfwgjkfv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gkguqsgwf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gphzisetl.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gzqiyqyly.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gvmstfqtq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gahzahssq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gkvlmxopl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gcbmjnsdh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.fehbvm.com/Article/details/gnsivhnkw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gbeiienwr.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/gthlasxfx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gbwnmeqyr.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtvxhkwoq.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gzqkyueup.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtpgtdiag.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gzjmaedbr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gfupatooy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gkdncbtwn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gyzxfmqcd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gdljkysuu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gmhgvjvso.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.fehbvm.com/Article/details/gxceswbtf.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gcttcnqxl.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/guprubarx.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/getrnvhaj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gxlbokueu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gwtnqlmvf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gikvujgtn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gucioxquq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gfpduxrft.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.hesvh.cn/Article/details/gxwamctrg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gtavjdwla.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gvluwoiil.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gavnvjhso.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/grmtomjey.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gkqcakkct.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/ggiyqbdrc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gfjjmmhlg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gtbxnaujy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/gchlqmfym.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/girypdcrj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gnatvdjnz.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/ghwyjvbbq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gwezauuot.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gpoedxkqn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gankxttpi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/girbpjeyu.sHtML


<!-- 参考信息 -->