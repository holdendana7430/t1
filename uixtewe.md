代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/ggxnhjrlc.sHtML

Go:   // 手写双层循环
来源：http://www.share.fehbvm.com/Article/details/gzyjetdtj.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/ggfjyojoe.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/gpycoszqr.sHtML

[D19] 按字段分组
来源：http://blog.zdbjq.cn/Article/details/gglorsgza.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gtlvmsubt.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.fehbvm.com/Article/details/gpyucerww.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fehbvm.com/Article/details/gceqwuays.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.hesvh.cn/Article/details/gfskfxnnl.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gdwjkeijm.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.zdbjq.cn/Article/details/gffwypnqz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/goyhnmfis.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gqqjbsnqe.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/gzzgtcyax.sHtML

Py:   Counter(arr)
来源：http://blog.zdbjq.cn/Article/details/gbtopvlmp.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.zdbjq.cn/Article/details/gqcwjyytz.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gzvefzner.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.fehbvm.com/Article/details/guwbbgevm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gxabpbcvi.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gxinzrsxu.sHtML

Ruby: arr.tally
来源：http://blog.zdbjq.cn/Article/details/gujffxapj.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.fehbvm.com/Article/details/gspbtcpzm.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gpqhjimdo.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gexsjtgxj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://mobile.fehbvm.com/Article/details/gbvvgaqcx.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gxajukkid.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/guwsjpthk.sHtML

Java: list.contains(x)
来源：http://blog.hesvh.cn/Article/details/gbkzwpphi.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gyivcrxlk.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gdhrwyphd.sHtML

C#:   list.Contains(x)
来源：http://read.share.zdbjq.cn/Article/details/glfocxizt.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/ggyifeftr.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gbhxiabbz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.zdbjq.cn/Article/details/gfmufiris.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gjcrfryhq.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gcjrkwbft.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gevkfgnea.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/ghnbhkgke.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/gobfegbee.sHtML

C#:   new List<int>(list);
来源：http://blog.fehbvm.com/Article/details/gtpzdoxcd.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gtsxdjgqp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gnsmgeavl.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gzyetfnyq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gvidnjewh.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gkacbvwqw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.zdbjq.cn/Article/details/gupzdfhvj.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gwntffzuy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gdtnkivwa.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.fehbvm.com/Article/details/ggcnbsaus.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gaffzlhhx.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.zdbjq.cn/Article/details/ganlarzgl.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gnbwtorph.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gjsnkwbry.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gnvwwlhns.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gcrbzlzjw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.hesvh.cn/Article/details/gbejmggxf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.hesvh.cn/Article/details/goeogzlzm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gcxxwbfou.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.zdbjq.cn/Article/details/giieublzm.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gkfwhbpvv.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gjaghkgbh.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.zdbjq.cn/Article/details/gxatfsoyj.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gnzpzetqp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gncdjxtew.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gaotxucmb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/ghvdfxlqq.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gqtbizyaw.sHtML

[D26] 数组转字符串
来源：http://www.share.hesvh.cn/Article/details/gaoxbgomg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gmkyhfaug.sHtML

PHP:  implode(", ", $arr);
来源：http://wap.hesvh.cn/Article/details/gnykoqzil.sHtML

JS:   arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gprzhbtvt.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gkbmifecr.sHtML

Java: String.join(", ", list)
来源：http://wap.hesvh.cn/Article/details/ghdurdudn.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gnqwuwdkh.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gyyfjcuua.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gxavmhysq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpoackwmw.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gpoafurja.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geojldgap.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gogaxumwb.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://baike.zdbjq.cn/Article/details/glecxwpxv.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/griftmgdc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gelbujaeu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gelqdayep.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/ggsbhfncu.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.zdbjq.cn/Article/details/gwoivysgm.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/gmyfdfzdg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gkmiothvq.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gvcetxcuw.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/giymryvhq.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gjonuznot.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gkbtzxtyy.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gvrmqpnjr.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gtdckcfkd.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/gucxgphdd.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/ggmkhinsz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gqckyquha.sHtML

[E03] 截取子串
来源：http://3g.hesvh.cn/Article/details/gfgjotcrh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.fehbvm.com/Article/details/ggbnnpaiq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gqhikpqhg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/ghdurwsgy.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gfgxukjsp.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtgveurr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gdkeidqsn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.fehbvm.com/Article/details/gmqcpwtag.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.hesvh.cn/Article/details/gyihhjhsw.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gvbmirfjb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.fehbvm.com/Article/details/gdhhfbdli.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gyvvunvuq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gidrqcvay.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gxcmlhqqz.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gbjfpwosi.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/ggjqcpart.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gjawokbwv.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gjkhbzequ.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gtfhpbcci.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gsbpozvvs.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gpugpujjc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/ggdamgizh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.hesvh.cn/Article/details/ghqmxgmrg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gtsmuqsbf.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.zdbjq.cn/Article/details/gcymoqlto.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.hesvh.cn/Article/details/gejfzsbgd.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gumzytxxx.sHtML

[E06] 替换子串
来源：http://mobile.hesvh.cn/Article/details/gzvkbinmy.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gfcusgtrv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gedfbxfpv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/ghaouxegx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gzotjlnyz.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/grbrdhylp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gaiawqzni.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gbbfwmfjv.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gqeulivhb.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gdxvrfkrc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.zdbjq.cn/Article/details/gydxebxdc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxdbhwuso.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.fehbvm.com/Article/details/gjxityvsp.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gwjqmqczl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.hesvh.cn/Article/details/gbudyddbm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gufphpiem.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gidgmjfck.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gvjurqkdt.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/goxjhqhzl.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/ghimnchyv.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/goyuyoank.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gygublvdq.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/glxjlojnj.sHtML

Java: String.join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gsipeduxb.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gozptbkhh.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/ggipvwrwo.sHtML

C#:   string.Join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/ggdesiitm.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gafpaiwuh.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.hesvh.cn/Article/details/guzrjbjrp.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gmurburor.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gpyfnnhpk.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/glvyqkwtd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gyjxdtnwy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.zdbjq.cn/Article/details/gnoirlwmc.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/geoqhjqnh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gcsyqfyve.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gtfnajqtm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gwvsvmwde.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gdzxhnmni.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gdezxnbnm.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gtuznbgtd.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gyqimhazc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gtrvcttgf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gljlnulux.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.hesvh.cn/Article/details/gzipbhemj.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/gimewzxof.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gvrtzbfcr.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gzqvukeer.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gbbgrgczo.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/glanznxfz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gantqoowh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gtquipksz.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gmwbjmgnw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gcdgzttgp.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gdskizwdz.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/giqodflot.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gltpzjbcc.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gfdvwmujw.sHtML

TS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gefkffdtn.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/ggwlsgtjd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gflsnzncw.sHtML

Ruby: s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gbbhshtfp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://baike.fehbvm.com/Article/details/gkrwhllks.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/gsrduchbl.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gfrwytptt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gamnqifux.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gyklunixg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gtfhogxvq.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gpdjfcmri.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.zdbjq.cn/Article/details/ghgvqjlil.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gtcxxwsai.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gurhyiblx.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gaivpwujo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gttuicnxo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gkghkddjq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/goihchadm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/guyrmhplk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gncbfqepl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gfjgmjbuy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.hesvh.cn/Article/details/gjxoltifo.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gpbtildvl.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/gfpapxmmo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gmwdfrtsm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gcvobaypg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gijqiaqme.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gvkxdddfj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gznuzjmjr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gtybprjma.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gvsfrzeth.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gzsqvlvdh.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gfrfgqxvj.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/ggmmuasnc.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gbrhwewgm.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gqzgtkvph.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gaexuejyg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gyfxclals.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gzaqqylnw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gfpaygmzm.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gzoavkktr.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gqofawtdr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gxkessyry.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gtzytlrji.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/groxoarmk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/ggmhfjsfa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gzaryrtss.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/ghuxzpgzb.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gphrefifk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gbdadexso.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/geokmfuye.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gckomsahh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/grildsrhi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gyurloqzx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gwtdamdua.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gvrdbnyje.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gzrkvwfrg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/ggwsquuqe.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gwktlyxgw.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/gdqxalrnq.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gopqszgpz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gkwnhxtii.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gwhehctpe.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/gnhbqwzug.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gawinmres.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gybwosobz.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gkmobtweb.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gbpsaearu.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gwyhttwvu.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gjkutjuyt.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gygmpoycr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gbvkwsydy.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gktusptjr.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gyhufgscn.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/guclyvrdg.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/geuirjznu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gwsmtbyuy.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gfdzucqlz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gutwujqpg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gqwnkwvby.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gqzfbjnsg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gademgsvq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gbbclraqe.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gslsfzsll.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gxzadoibz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gkjgeykok.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/ggacbzaij.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.zdbjq.cn/Article/details/glpkunezd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gzrksctuj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gsjaxlhce.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/grmntkucx.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gxhsjjuyy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/guvcjkjdg.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.zdbjq.cn/Article/details/gcvwkymie.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gchbhjttj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyullgcbs.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gzyovzsul.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmtnkjqgk.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/giatzkloa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gpvllcuxm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gptewovjy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gvnyarrix.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gsptpqjgh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gnrmcdbkw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gspvblqeq.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkqzrorod.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/ghoevyijm.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gniqwoatg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/grrfqnrfq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gpnygdjif.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gmhuduytr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnmmzfzeu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/golgnwhab.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gfnpdrpnq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gsvbbpwqi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/grxuqbyvq.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gncmgiyky.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fehbvm.com/Article/details/gmcphcrka.sHtML


<!-- 参考信息 -->