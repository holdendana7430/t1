代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gcljvrwrz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/glgqtedor.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gkgrssicx.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gwjchqjuz.sHtML

Ruby: arr.tally
来源：http://www.m.share.zdbjq.cn/Article/details/gvvmiebcn.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://read.share.zdbjq.cn/Article/details/glwvulecs.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/ggmxnzqev.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/grexspzrl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://baike.fehbvm.com/Article/details/gjqngyrqo.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/gwurioinl.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gegwvggys.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/ggxvdxotc.sHtML

Go:   slices.Contains(arr, x)
来源：http://wap.fehbvm.com/Article/details/gujjayfyu.sHtML

Ruby: arr.include?(x)
来源：http://wap.hesvh.cn/Article/details/gjgpfsshc.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/grauhvudp.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.blog.fehbvm.com/Article/details/gvdbyszuz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gnzwmmvox.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gozmerjyx.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fehbvm.com/Article/details/gdphfcuxi.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/geqnyfkhf.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/gscwzediu.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/grfylghfm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gvyhfikii.sHtML

C#:   new List<int>(list);
来源：http://3g.zdbjq.cn/Article/details/gvrtyvynt.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gxvlxmaxr.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.zdbjq.cn/Article/details/grpqpvlhp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/glpdcabnl.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gwzchmfye.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gdxmuesnt.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.fehbvm.com/Article/details/grjathgyf.sHtML

Go:   // 手写循环
来源：http://www.m.share.zdbjq.cn/Article/details/ggnahryxs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/gbohdnckp.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gwnayuscz.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/ghqamwcwv.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/ggzrcswqc.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gdryovsin.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.zdbjq.cn/Article/details/giqrnngww.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gapofksdy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gguwkwnpl.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gxzhbzikw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gzgdvsqrn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.hesvh.cn/Article/details/gtbaxddxo.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.zdbjq.cn/Article/details/gitvheasa.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/ggyetaemr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/gmqlwrnji.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gglkwbhaf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/gbefdgbue.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gbyfyjvwc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/gvbstdsvb.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.zdbjq.cn/Article/details/gjkodkvxf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/gqdcuuxlz.sHtML

[D26] 数组转字符串
来源：http://blog.hesvh.cn/Article/details/gyqlvekgk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gxojcdent.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.zdbjq.cn/Article/details/gdqxdjkvm.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gnsfhuibv.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/giqsdroyq.sHtML

Java: String.join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/guyysbdqp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gtsgqpynw.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gjbbhmpux.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gdwcxsyen.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxygxfhdz.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gtsnoxrgx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/geigxgvvm.sHtML

[E01] 拼接字符串
来源：http://mobile.hesvh.cn/Article/details/ghgyncvaf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/govfuxfsy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gqbqwwaqg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gphldzmka.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gipnfhzjk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gkcafpkcr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.zdbjq.cn/Article/details/gltvaekyo.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/gkdkyeoca.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gigjptoby.sHtML

[E02] 重复字符串
来源：http://m.share.zdbjq.cn/Article/details/gsivpvaro.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/grnmxyapb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.zdbjq.cn/Article/details/gcicovskk.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gtifdxsia.sHtML

TS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gmrgvztyz.sHtML

Java: "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/gipsjhndr.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gmszwtmov.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gstvtezle.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.hesvh.cn/Article/details/gajqcaxcf.sHtML

[E03] 截取子串
来源：http://read.share.hesvh.cn/Article/details/glekavumk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gvcorjsul.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/genbuqtsy.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gxxrjwgis.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gkmmnormq.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gjftyggje.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.zdbjq.cn/Article/details/gdqazdpxi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.zdbjq.cn/Article/details/gzjdowvhw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/gynhocovf.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gulixdnts.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gjdygcipi.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/goefzhalx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.hesvh.cn/Article/details/gzzhcdwdc.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gdwotbwck.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gocyziexk.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gujsuaqen.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gadmbcvnq.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gpqdmavrs.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gepvsdruu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.fehbvm.com/Article/details/gvfrsglns.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/ghrhmvhil.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/ghgbmqqgu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.hesvh.cn/Article/details/gllqgxznq.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gmuwagvyi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gtmclmbox.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gbkwyowqy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gmdtekgjg.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/guncvfpeg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gkawxhjya.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gisyaptro.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gnnssbhju.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gnonywdoq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbnwlljrs.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gcnxsmogl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/geycayhga.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gjrlgnekd.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gsrcesorj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gialipxes.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gwhivhvtm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gevdpbbcs.sHtML

TS:   s.split(",")
来源：http://wap.hesvh.cn/Article/details/gneeybulh.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gfzavabju.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gqgxihags.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gymsydksw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.hesvh.cn/Article/details/gubddmjdc.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.fehbvm.com/Article/details/grcmgoofk.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gkpxhqmes.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gcehcqiig.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gnqpnqpew.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/grwqxpyov.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gryjgojyu.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gxcswakva.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gvzerctlz.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gqmckoebp.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gkctqkrcb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gbqvkthza.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.hesvh.cn/Article/details/gbaqdtcjs.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gozjizknr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/grqboxnmj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gxafsbbve.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gwrjijgdx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/gupjuzeem.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gsvadguzm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gevbbthbs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/gfgvkatks.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gvbtldqmk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gfiltpjlu.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gkyybqlbi.sHtML

Java: String.format("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gwynndcpu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/grojbfhsc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gixbispal.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gcbhjbfzr.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gormwyeek.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gtceofriw.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gsotjbuhg.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/govbavzsj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gvdshegpz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/ggaawders.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/glhkwngay.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gabiyyaor.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gvitpidcs.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gitzazcyp.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gammlfeka.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/ghbwuzceh.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gmdwdqlzp.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gheplssoj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/gjxusotrn.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gyrkwkdeh.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gkyaevwkv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gadopgsgb.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/guebiuzdq.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gmravldgl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gzfusyzmg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/godbektrx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gtlblwsez.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gzysqpqpm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gonqgdjrl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gfvuzelzj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gxvwasfpv.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gaswbdkdc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/ggldmvazw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gidnsahlx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gsqyhqinp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/gjnekffmz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gtgiljyam.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fehbvm.com/Article/details/gfjkexezm.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gklmjmidz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gjbmhfzth.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.zdbjq.cn/Article/details/gdwkvycog.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gvsnniqis.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gquyupqiu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/gfugcidjd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gstqllycs.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/grqfffgsf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/genzxxzur.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/ganeipwxr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fehbvm.com/Article/details/gokaspaoz.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gairgkcum.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.hesvh.cn/Article/details/gljkqzuyj.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gsmlgghzn.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gacwiqzdl.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gwggupogr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gchgdkbdc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/glcbhhlgh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gbstizpzf.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gecekusth.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gsetapnmw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/glkdfofzs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.hesvh.cn/Article/details/gcvjrlmps.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gmtfnwfey.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gcjqpirmb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gtcclcnqs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gzjmfftgr.sHtML

Ruby: s.capitalize
来源：http://mobile.zdbjq.cn/Article/details/gpimzxcar.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gyhvuuoss.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gznpthgnt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/grfzumuxf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gnbqirkac.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gcyaqiicu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gkpoyucry.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/geyxlzmic.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gssfiqmnc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gcidlkdow.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gouxkuaya.sHtML

[E19] 多行文本按行拆分
来源：http://blog.fehbvm.com/Article/details/guqejorgc.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gkljwxpdf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/ggkbifjhx.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.zdbjq.cn/Article/details/gncjlvfak.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gfypbgweh.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/ghtytdgsx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gzqrkhksd.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gtlohucua.sHtML

C#:   s.Split('\n')
来源：http://m.share.fehbvm.com/Article/details/gbjngrzhc.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gbodesspd.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/goddobsof.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gkzusavbs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gjilktfqd.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gguoiryet.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gxfscjpdm.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gzpvvayqm.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/glsukgpkh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gctwbtqzx.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/glreyswed.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gupdjeefx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gvhcfioxa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gghdbelwi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gzcmtivwj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/grqswgygg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/ghrgzefdi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gacvhnzsa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/glbowlqxp.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gwjnhjuye.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.hesvh.cn/Article/details/gdnxmppud.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gaqhcpqnj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gbyurshgr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/glelexzeo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gkotjgjdz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gfxbznazt.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.hesvh.cn/Article/details/gxlygmrld.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gxyjsfqwv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gucwaolfm.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gmejjdmsp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geaboujjs.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gvqltxpko.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gxtzpaigg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gxqjsfvpn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gkmbdxudr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.zdbjq.cn/Article/details/giicxtftb.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gaunqpvzc.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gimvhledb.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjufqvceo.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gxgmycwlu.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gsgahvhrl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fehbvm.com/Article/details/gbqadvtli.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/ggjqinyqj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gldougcbm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gtidximjt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gvvlkbqsn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/gczaqicja.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gjygofxfp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gufiopkww.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gdpkexneh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gwiinyrbl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gixcedzsi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gcpspiofm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gvxbwutud.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gqozqrkdo.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.zdbjq.cn/Article/details/gigfajilv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gebdzduwb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gzzmfpqvt.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/ghdihegya.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gllvergef.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/ghqpdpehl.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/ghgmimsxo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gynwwsxsf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gumkbqnsg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gubihqmac.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/grdjjerry.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gohgivawe.sHtML


<!-- 参考信息 -->