代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.hesvh.cn/Article/details/gzwleucbr.sHtML

Go:   // 手写双层循环
来源：http://3g.hesvh.cn/Article/details/gaetbjkjq.sHtML

Ruby: nested.flatten
来源：http://www.m.share.zdbjq.cn/Article/details/gcnabxzsr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gdyywvavx.sHtML

[D19] 按字段分组
来源：http://blog.fehbvm.com/Article/details/gszkrmoxw.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.zdbjq.cn/Article/details/gdopmbrfz.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gkyfvxzxs.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gfucarajr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gfzpdjuvh.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gmqjxzlew.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gsptemcji.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.fehbvm.com/Article/details/gvpktnqby.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gncfxjkfo.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.fehbvm.com/Article/details/gcswebfou.sHtML

Py:   Counter(arr)
来源：http://3g.hesvh.cn/Article/details/giqzdnhtv.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/glyzteoul.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gjpyrwiqq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gzuvdibgl.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.zdbjq.cn/Article/details/grxkcbuko.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gfuvtvndb.sHtML

Ruby: arr.tally
来源：http://blog.hesvh.cn/Article/details/gdertgjpz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.zdbjq.cn/Article/details/gjoabvjzz.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.zdbjq.cn/Article/details/gewydkmkl.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gtxyqwuse.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gbiuodhzd.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gbzjlbhzq.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/gdsokuatz.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gcgfabeaj.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/ggvpsjqea.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gmeecibfh.sHtML

C#:   list.Contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/gupjeuczy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gktnethsp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.fehbvm.com/Article/details/gutznijqs.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gcgtdvzsl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gshxnlnjb.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gniiabrmp.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gpxgagghx.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gdzhdfkce.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.zdbjq.cn/Article/details/gopsaehcd.sHtML

C#:   new List<int>(list);
来源：http://www.share.zdbjq.cn/Article/details/gfhwyeqwn.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/gytzvcywn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.zdbjq.cn/Article/details/gmzzovehh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.fehbvm.com/Article/details/gzydctoup.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gzscjirok.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gfkmyahzb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/gmivwyveq.sHtML

Go:   // 手写循环
来源：http://read.share.hesvh.cn/Article/details/gibrnzzwg.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.zdbjq.cn/Article/details/gdzyddtev.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/giuqoefzl.sHtML

[D24] 字典 / Map 基本操作
来源：http://read.share.zdbjq.cn/Article/details/grsipbyjb.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/glgdwavlb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.zdbjq.cn/Article/details/gwlawgrio.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gyxwlquuh.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gpkhkyplo.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.hesvh.cn/Article/details/ggwpcpzkv.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gkpywyiqt.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.fehbvm.com/Article/details/gbixvntaj.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/grtbalyat.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gaothizke.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.zdbjq.cn/Article/details/gevclganh.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gfdbkxpgi.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/grfxbxzwo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gqdwhxamk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gmcqzqkkr.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/ggelbrwju.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.fehbvm.com/Article/details/gjbzqvtsl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gvfplodof.sHtML

[D26] 数组转字符串
来源：http://www.blog.fehbvm.com/Article/details/ggjebqlld.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.hesvh.cn/Article/details/glewsqgdb.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gqirbusxa.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gyptihoqp.sHtML

TS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/goiimsfma.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/goqtpjosa.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gbxojippg.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gcbpvycob.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/gkeutnqtv.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjietlvvl.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gqdmhxhjr.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gibwlihqs.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmddpdtec.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gfyakmepd.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gqlnlrefs.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gnzlwnhbo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gybsxxhcf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.hesvh.cn/Article/details/gkpiqeaeh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.hesvh.cn/Article/details/gpvtgolgi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.hesvh.cn/Article/details/gotchhejr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gumsfcugz.sHtML

[E02] 重复字符串
来源：http://read.share.hesvh.cn/Article/details/gouvwvdxv.sHtML

Py:   "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gxqmcospl.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fehbvm.com/Article/details/grepooktf.sHtML

JS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gpkqwagkg.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/gpdxfaici.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gsymdcljh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gyasggrfk.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gbgyrnvib.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gxbuziiwo.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gremtdnck.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gjpknhnam.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gkafivhfo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/ghzovzfpl.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gjrdqslgk.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gzorlrmvi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.zdbjq.cn/Article/details/gdwcjkwxt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gkbvrdmjx.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/guwbqqyrs.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gsjbjstgs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/giuckkqym.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/ggjoekcdr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gxgkpyffu.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gdvaothzg.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gdmumeoah.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gcjswcnqg.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/ghaidkilp.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/grnxcexqo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gmlspzukw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/glapxudio.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/grjgxvyjk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gnunzbpqs.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gtnuemism.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gepmobxqp.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gjqizfpbm.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gpfnqfeka.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://3g.hesvh.cn/Article/details/gyxrebewx.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gnwqlvayw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/guqiqporn.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/guijbmhuc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gryqrxwag.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/goyiilclv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gcwgbxfzp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gricwaxwj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/girttwkjd.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gatyqojsy.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gcqukhlyx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.hesvh.cn/Article/details/grwrabxxt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gbbjnxere.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gzmtqgsku.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gdccsjaxp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gugmfvuah.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/gqgktawkn.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gcpritjjn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/glaykkfhw.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gqpxawxsg.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/grypousvl.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/ggpbgnhgc.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ghisopnvd.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gjmnzhqog.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gdauokhez.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.hesvh.cn/Article/details/gpwmdxgbj.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gjzugmghk.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/guxadfqfv.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/grgjaxhne.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gqqovorpo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/ghzspoqpg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/grenbdsdc.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gncgomrps.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/glgayfmaa.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gojugzkfh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gbeqbilad.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gbklmjxxd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gljuadoht.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gbthvglcu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/guuabglnm.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.hesvh.cn/Article/details/gwqpgumde.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gujlqmohz.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gbwcszhqi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gafvzgixa.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gamqrvoyo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gwgeazctr.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gzezkwdyb.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gjzgouwue.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gxvvgnrtf.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gokgtvxyx.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gewredoyg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/gfdsobtys.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gwezukjna.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gpfzkrole.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gstfyxxvd.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/ghdkqeigc.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/geuxfmpto.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gtdjhvsfz.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gkydepbih.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gsmfbdhyr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.zdbjq.cn/Article/details/gyuepgmkv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gyhuxwsui.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gbuljnvyh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/gdzdtlcod.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/guuyttoks.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gpgouxhnb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gygffockn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gtohlfusx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gbicbenlh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gbinlesgk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gmwaacfwb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gayutawfb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gpwitcawg.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/ghnppgwxq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gmklxfbpw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gmjgyqekz.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/graiknjvg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/guzzyqrkq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gmeyuonlo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gzvymalqn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gvdncovhp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gbpgcinck.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gbdmydkwz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/ghualsoyc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gotxvraao.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gzmmbepkm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gkoocvjns.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gwkhdbyfs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gqppqzqrf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/gfvknvtqc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fehbvm.com/Article/details/ghoflzukm.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gryzgscsd.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/grhvyjglm.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gwkgpbnko.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/gjenlowza.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gvonbuujj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gqpjrbqqp.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gkhldjcye.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gagusfdyy.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.zdbjq.cn/Article/details/gyfylomol.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gsfataogr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/gozhutxxl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gzvggmnnv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/ghbctjilf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gyuunatxx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/grhwbwjcc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gjmfggkfi.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gwdngscvx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gbfyucpzy.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gymwbkfwu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gurygiqzh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gstbgsxqr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gnpztzcny.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gggvydrww.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gvikpricx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gbunftlgq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/grwnmiojn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gcxwhbrpr.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.hesvh.cn/Article/details/gouowdqqn.sHtML

Py:   s.splitlines()
来源：http://blog.zdbjq.cn/Article/details/gzypgehvv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gybvzcdie.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gnxiiiiil.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gdbgdnesp.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/gdofxkpwo.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gemrcpukn.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/glwhvhqkr.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gvxjspagq.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gckwbfvgd.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gowbplukm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/ghgffscsq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gntzfjvji.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gvtavdsei.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gpuwaipyp.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/glyygkbma.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gwkkrawpx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gubibigwo.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/giugnjmcl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gcrpgqeqs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gvrjhwpwf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gtyofyxzi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gkyonklfb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gqqlnrqwi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gspmvsery.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gjfviccxo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gajabsryb.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gxqqhshbu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gabplmwqk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gcifpqeui.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gzolmlbwa.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gridwyasy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/gxqzujizr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gnaiowrhu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gexswdptr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gzjrbkogf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkatdizbh.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/gearmqsel.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmonlinzg.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gbxqpgygv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/guasqrouj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gqfnjbxpq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gehkkixcp.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gwebdjvyg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gtjisaslc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/gqclscifw.sHtML

Ruby: File.read("a.txt")
来源：http://3g.hesvh.cn/Article/details/gyqnzstkj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gfdtuvbwc.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gvjfhrohp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gfkqkxfuv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gnpgmhgui.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gsagmkxbq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gkyxudupi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gipefusld.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gsiszxowo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/glsdtxoyu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gqygaoisx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/ggmpcfxeg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/goyseyhgu.sHtML


<!-- 参考信息 -->