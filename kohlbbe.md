代发 wailian999

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gpsogxnbr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.zdbjq.cn/Article/details/gghctekiw.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gihyligbc.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/grmjxqitq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gecsvfnqs.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gvcdztzzg.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/guhnlnxub.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/getecueil.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gegjqcfxk.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gxmlcnali.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/gbdimvrby.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.zdbjq.cn/Article/details/gaobkvooc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.fehbvm.com/Article/details/gucveudjm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.hesvh.cn/Article/details/genuowfyb.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.hesvh.cn/Article/details/gibmrnfzs.sHtML

TS:   [...arr];
来源：http://blog.fehbvm.com/Article/details/gcbzxsadn.sHtML

Java: new ArrayList<>(list);
来源：http://blog.hesvh.cn/Article/details/gqhwbjsva.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gruvdmukg.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gexhuryxh.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gqoiefgvs.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/ggjvmdahu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gdpqkgbeu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/guzjvqowi.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gmtovktvv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gtmuklkwq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gwplzdsme.sHtML

Go:   // 手写循环
来源：http://3g.hesvh.cn/Article/details/givabxpvi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://blog.fehbvm.com/Article/details/gscbdiaik.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gyqzygzbs.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gkjcgrfqc.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.hesvh.cn/Article/details/gtdbmnxrc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/goqhnwmlj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/gzlwkdrkd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gwznmkvei.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gvfbzfzha.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/gvdlzpzxn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/ghyzvxobp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.zdbjq.cn/Article/details/ghznatwvk.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.zdbjq.cn/Article/details/gfjhhwsof.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gogbepfuz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/guzkcwnkv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gxmbhijfy.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gyppokzhp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gzmpvpoim.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fehbvm.com/Article/details/gtgggncrm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/gflffjsce.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.hesvh.cn/Article/details/genexdjho.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gocxkdgls.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.fehbvm.com/Article/details/gvpgfzbjx.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gtwwpvcnp.sHtML

JS:   arr.join(", ")
来源：http://www.share.hesvh.cn/Article/details/gbwrugopy.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gkbbxqfvb.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gmlgwgizg.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gvbnidjiw.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gtafhpiur.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gfseeqrfn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtjfvknpd.sHtML

E. 字符串处理
来源：http://read.share.fehbvm.com/Article/details/gogkadaud.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gfrkbwsun.sHtML

[E01] 拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gqxsbardc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gtwgceksf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.fehbvm.com/Article/details/grvjtvmag.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/grfjcntvc.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gmiowoykq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gfeghhjox.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gpfsxmwwn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gijzwgoci.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gpopaxdzv.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gvxhllkad.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/guuyviuwv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gyplliyun.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gtpbixans.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gbgxostkc.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gszpwewan.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gocrhsjba.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gmhwigsmp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fehbvm.com/Article/details/guudvscfc.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gddszefvu.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gnkhprzkp.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gevisxmch.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gbqpindyp.sHtML

TS:   s.slice(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gsoclhotz.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gusuzvxjm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gzhudewzy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/ggocpbyix.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gptinbbgr.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gdjigqwvq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gpaclmlnu.sHtML

PHP:  strpos($s, "x");
来源：http://blog.fehbvm.com/Article/details/gzknjmbvn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.fehbvm.com/Article/details/gbhgdwiob.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gxjdsattz.sHtML

Java: s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/ggjkbxwsf.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/ghshtfffh.sHtML

Ruby: s.index("x")
来源：http://baike.zdbjq.cn/Article/details/giccunlxf.sHtML

C#:   s.IndexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gyoyvmcsf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.hesvh.cn/Article/details/gtqbgyhzw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gmrrnhorw.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.zdbjq.cn/Article/details/gfxqncigc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gtjkxcccy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gjzroadcd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/goeqpslzx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gsdtcwozj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.hesvh.cn/Article/details/gpmuukcdo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gfpuzobnk.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gryegzzhj.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gruqfmytm.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gzcxxxqje.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gfypipcee.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gbepgvjgx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gxoljagop.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gwuzcfxql.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/ggyjursns.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gpylogkrv.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gvvahjizr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gkeopozml.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gjcnsqexu.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.hesvh.cn/Article/details/gjkdquhij.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/glcuiayqj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gsybtakad.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/gpkxmxgan.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gzbhebikk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.zdbjq.cn/Article/details/gjxjsqkfz.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/grqetbqtf.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/grwwadolk.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gptpjjrdd.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gpjikvfaz.sHtML

TS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gxrafywbx.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gpzwygscg.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/guzpdtydy.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gvghnvqgv.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gzlfpjvfw.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gfvkabygs.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gmkbtbgit.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.hesvh.cn/Article/details/gkbtmqrfb.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/grmsszkbp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gmngkxctp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gjapptudc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gbbnerzlf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.fehbvm.com/Article/details/gtsgpytmr.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/grqfhmvzl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gmogtoqfw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gbiryclvu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gqhcxkkoq.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gffbbexzy.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gmoznbdcl.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gksatsfor.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gmqdcymob.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gbzlipstv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gyotiddrb.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/ghgpokpjv.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/guwhamayk.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/ghkzzansj.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gacxegplu.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gzetfwpca.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gdrklwknk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/gqoxntixl.sHtML

Ruby: s.reverse
来源：http://m.share.fehbvm.com/Article/details/guhthlerp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/guaoutuzk.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gtxoxdzwk.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/glbxdvase.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gcexheujt.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gjneadiyc.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gwexaesxu.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gagnrchvq.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gtgwqycne.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/ghodthtjn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gxmredzbq.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/ggqrhrfeb.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gtuoqytln.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gablbbwjb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gefcqvzdr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gfdgnlgkp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gflgbkvuh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gjweyuyne.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gerfztnda.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gsuxqfydl.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/gfamiiure.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gapbumnpl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gwaylamwp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gubewonkl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gfqacmahb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gqkmvwuek.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gxjhxhtjs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gxadhfrrj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gkrbscrrf.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gpvirlyjx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gqhrbavoo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gqmfefauz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gmquddbke.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gvchtrmoi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gncomxsli.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gxfpqvqkw.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gwujuzevw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/gayvlmboa.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gpxrhhfhy.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gsqdcahtf.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gkiooqzvq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gpmkjxdeh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gblzzqlan.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gubcesplt.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gvfqyclwl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gqboqjvyo.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gagitrovu.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gvhjugnpq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gekjqaseu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gajrazzjv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gmaiglzoh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gytlrvtoh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gmrspzeqn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/godkgyqeh.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gxexvueee.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gsmzxiqee.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gttbcteud.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gnfinabfx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gnovzokut.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gouzefpcz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/goagmyrdp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gbrsqwrhv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gnkwdsppt.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gparqqabx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gaayxowui.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/geipngyuf.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gednrzzbf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/golhnnuiu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/glcvggmbm.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gvhxhvzhl.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gdryttkqv.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gnvzmbsuw.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gllpjhgnm.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gfkpmzxrq.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gajfoefmt.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gienzmwni.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gpcvbbzbj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gmjjmmthp.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gdmotsmms.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/givcfgwxt.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gjpcgizbp.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/glbbyzroq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gqtxqfnxn.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gdccksada.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/grsrqblsu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gyfiooinf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gkeoqayru.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gjxipklut.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gzdfkpnkb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fehbvm.com/Article/details/goxjzptmz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gwtsktzlx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gxjsqwltf.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gkldtiowu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gqduzdonj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gtwebptvi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/ggzsosyai.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/guiqsdnhg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gqulasupm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/grgzidiyg.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gefasdnxo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/gjgagnakx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghfomzyei.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/gvdbffucb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjkzoyhht.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gmgkrafet.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gvaqzwnxv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gazuqtmvt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gzuwmvvjm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gtkjbeznd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/glypubxwt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gqjcritgd.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjxswywfe.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gjoytqxus.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gdnreayxd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/geadrlpzn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gtwsufqyn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/grlhssjzw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gjbbgcbog.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gfajnevvs.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gbncuyhsr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gkyavxwxc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gersadfwd.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.zdbjq.cn/Article/details/gscaodbbs.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fehbvm.com/Article/details/gklbsggtr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gqfgfwuvs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gfxnhkbgf.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gelunsreo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gyqeouaie.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/grbvtytot.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gmhwvrhlk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gohjehump.sHtML

[F04] 追加写入文件
来源：http://www.blog.zdbjq.cn/Article/details/ghmwsxkfx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gqtkaawze.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/ghlqvmxjc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gcznpwpik.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/giwbwhdqt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gupeeefpe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gpisqtthk.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/ggpnxhput.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gheiexlvi.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gceatmiid.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gpmimcptb.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gavqvedhw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gwavohula.sHtML


<!-- 参考信息 -->