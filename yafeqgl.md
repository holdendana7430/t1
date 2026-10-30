代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.hesvh.cn/Article/details/grblidqpg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.zdbjq.cn/Article/details/grlmrnivq.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.hesvh.cn/Article/details/godsbvkda.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://blog.hesvh.cn/Article/details/gyxzjmogj.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gbcjxvujh.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.zdbjq.cn/Article/details/givgmbstp.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/ghrvxxhvc.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gjjxuwubr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.hesvh.cn/Article/details/gzxdsksiw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gbrvbzquq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.hesvh.cn/Article/details/guzjgvolh.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gwoajvjlp.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gwlmcaoqa.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gfrvlkmhd.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gacknmavg.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gxbwgryxu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.zdbjq.cn/Article/details/gbgybedrj.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gscbixqft.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/gukxxmits.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/glrprqtbh.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gfzqysbnn.sHtML

Ruby: arr.include?(x)
来源：http://baike.zdbjq.cn/Article/details/gdmlkfdcd.sHtML

C#:   list.Contains(x)
来源：http://m.share.hesvh.cn/Article/details/gfkxcanqk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gasnxzrtj.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gwisivuxa.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gprkongdq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gviuescgf.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/ggcfbscxg.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fehbvm.com/Article/details/gtyanggva.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.hesvh.cn/Article/details/gzznkbiok.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.fehbvm.com/Article/details/gazzwdqjf.sHtML

C#:   new List<int>(list);
来源：http://read.share.zdbjq.cn/Article/details/gcueqftom.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/giyzyoczp.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/grmnsorsz.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.zdbjq.cn/Article/details/gaycdajfj.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gwzrhtqof.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gxpvusdxf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gywznzjib.sHtML

Go:   // 手写循环
来源：http://mobile.fehbvm.com/Article/details/gzbilwzkt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gqlreoyhw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gekrtoosi.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.zdbjq.cn/Article/details/gfitvhdit.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/gxbvzccfb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gutouxwxd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/gwevphsla.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gbwbbayno.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://read.share.fehbvm.com/Article/details/gmwoulccj.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.share.hesvh.cn/Article/details/goenjglsl.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gylskqwrr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gjjwebcqq.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.hesvh.cn/Article/details/gfbvjhsbc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fehbvm.com/Article/details/ghplomres.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/ghyvmsgpx.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gpbtguggc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gfcrakcei.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.zdbjq.cn/Article/details/gaslsbcfi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gcshqzpdy.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gxdfmdwyv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gowebszwo.sHtML

[D26] 数组转字符串
来源：http://wap.zdbjq.cn/Article/details/gexxhhbdq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.hesvh.cn/Article/details/gsljyrkgt.sHtML

PHP:  implode(", ", $arr);
来源：http://blog.hesvh.cn/Article/details/grvpjmdok.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gtekratam.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gdsucpzbg.sHtML

Java: String.join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gcdtwuoor.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gtchwsegn.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gclfwexbo.sHtML

C#:   string.Join(", ", list)
来源：http://wap.hesvh.cn/Article/details/gbdlmohbj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfwlnnxls.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gdacvhkdm.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gphfisouu.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gxivkukvu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.zdbjq.cn/Article/details/gskskveic.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gskzwpjhn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/glvqovsog.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gurfvhztj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.fehbvm.com/Article/details/geevbnjzr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gnbnvixyq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gkpigrukb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gnehxskym.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gpebwsghv.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gjdlrfeey.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gffafvuee.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gzeanwrfv.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gnanlbfcs.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gsjarzywm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.hesvh.cn/Article/details/garxvteyp.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/guhopdulg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/ghsyzusyf.sHtML

[E03] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gligmyekk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/gvrdenezo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gtnnnqxsk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gpaeuxazm.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gqepfitzw.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gcudlfxdt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.zdbjq.cn/Article/details/gyulwousj.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gzrccwvmt.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gpietzani.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gkizldyvs.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gpcllgwkw.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gpsqayguj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.zdbjq.cn/Article/details/gjeuozymc.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gwjwgsgaw.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/grcgkeqvm.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gtlhibvrj.sHtML

Ruby: s.index("x")
来源：http://www.share.fehbvm.com/Article/details/gqdsjinbn.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gpivvpska.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.zdbjq.cn/Article/details/gfyqgwwmv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gscpfujbr.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.zdbjq.cn/Article/details/gilbppxim.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gymklvlmj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.hesvh.cn/Article/details/gwamzhtvn.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gzdvhnmie.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/ggfjxkreh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gfvoxjiln.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/grfscwwan.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gcddpcxjk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/ghnskkwqt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gjnumxnuw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gctfzctnl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gdjqclcpy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gwjhemvzf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gcrzreihf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gtpemxmjg.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/giydinbda.sHtML

[E07] 按分隔符拆分
来源：http://read.share.zdbjq.cn/Article/details/gvyyhrhps.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gcruorqmn.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gpugexygm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gybcddymi.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/glzhbayya.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/gzlgsepph.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gpqjyvata.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/gqhfomdbt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgovvumn.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gcivytrko.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gzmokmyez.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.fehbvm.com/Article/details/gpbpzpeia.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/guwqddcwk.sHtML

TS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gxicaplln.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gtmtlwgix.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gacckcnao.sHtML

Ruby: items.join(",")
来源：http://wap.hesvh.cn/Article/details/gqsyzuefv.sHtML

C#:   string.Join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gkwhyhyss.sHtML

[E09] 去除所有空白字符
来源：http://read.share.zdbjq.cn/Article/details/gmggyudky.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gvdbctzxn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gevezftqg.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gxmlqqqzw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gytcboyta.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/grwqdqbaz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gceatgoew.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.hesvh.cn/Article/details/gzjaazhsh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/grtpcbgwd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gihxpfrgq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gjfcqcamk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/grzqweebb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gkwmqejub.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gpwwwhdat.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/giopdzrud.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gukexgdjh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gzemngwls.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gmmpcderd.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/grkpefhnv.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gctpvdcux.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gqwjhbbhi.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gzbztrwmy.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gufqrojah.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.fehbvm.com/Article/details/gqkrovgkp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gepeeojho.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gmppcwjrm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gjmyzfxsc.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gurmfhkvx.sHtML

Py:   s.count("a")
来源：http://wap.hesvh.cn/Article/details/gylajekjw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/ggqxrckxs.sHtML

JS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gjqlbaycm.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/gzsgpoepm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/geupxtmzc.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gllvxcusc.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/glcmytvca.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gujijrgsh.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gbcxzrlkv.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gykmtlwnp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gieflnxpi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gsfazkcaq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gatyhdvol.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/grdaocwke.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gddzhxwsq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gwcjanouu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/glokclquj.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gfjmhnvrr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gkgxscoat.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gmhwecnmq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gtdubfypy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gkopiksua.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gnmittyze.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/ghlfsjbot.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/ggphsrtot.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gmkoqvosx.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gbtnibwwb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gwtuqspuo.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gpbygoxhe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.fehbvm.com/Article/details/gbpjykull.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gannukgqj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gjsgrczmh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/gsjenyaof.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gyeooqgvo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/gdhgfctmb.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/ggdenegdx.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gdqiegtjf.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gkivxkgpf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gnaxbtdub.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gcqjwxpvx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/ggudcykha.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/grkbjvbxe.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gyuflyskb.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/ghyjbwgcu.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/ggvnqvcaz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.hesvh.cn/Article/details/gtuxxucax.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.hesvh.cn/Article/details/gyndbawob.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gtbtbzcrf.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbtrnswzp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gnkmptlgs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gyiedhxqs.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gmhrhtiuf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gykvkwuze.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gvdvwkizg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/giijqrcnr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/ggzvqnsrt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/guigkuczz.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gakbnqydz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gqcywjkas.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gkfeztmjd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gnruftfht.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.fehbvm.com/Article/details/gthnwczyv.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gcctnghkz.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/goymgspym.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/ghcgetmwg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/goyiiuada.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gzlgqooly.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gwaqrggfh.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gvfjusgqc.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/gzkcuranb.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gecsicfgy.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gnlwwywkc.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/givntwarn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/ghxbiulxh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gjisruwtk.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gfhmqmjqf.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gsxvmqjfi.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gqlrgdzpg.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gkoodqzod.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gllsthxvw.sHtML

[E21] 超长截断加省略号
来源：http://blog.zdbjq.cn/Article/details/gxxdzxquc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gyzkwhpcf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gfpxhsdpf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gbuluozya.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gpcgosjzq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/geuvwhthw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gzunkrrlg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gnzfgyiee.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gpepxaogo.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gfpigqfxe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gfghmlpnc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gwaszmrrb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/grohzkelu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gbizdkgau.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gdbsivgwz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/guuyarlld.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gyusbidws.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gpkgpudtb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gbyjaacwy.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gexaxpiub.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gobqvoumy.sHtML

[F01] 读取整个文件
来源：http://wap.hesvh.cn/Article/details/gpndbdpnv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gktrhtsaw.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/guthsjume.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gdifjgylu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gwmgeyyfm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gwqfhtnqi.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/garuirnpy.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fehbvm.com/Article/details/gejoevkwz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gwdfqtapt.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gstaetqcx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gtwtexvuf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/glhnqivod.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gugjdqyuo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gdbpmxplu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gnbpohegt.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gcahzpzvd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gniymkwxk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gbiwwtbga.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gxgvifzpp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gdzhalmpn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gdrmhlkcf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gsnxtwojk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gieapriyx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/ghmlvqowe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gexopvajr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gkhlvlonn.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fehbvm.com/Article/details/gspfzcqvt.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gocjouubt.sHtML


<!-- 参考信息 -->