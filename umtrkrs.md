代发 wailian999

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/gfyzprkyt.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.zdbjq.cn/Article/details/gbcfwbwbc.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gcrdwzrzu.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.zdbjq.cn/Article/details/gylzkuinr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.zdbjq.cn/Article/details/gvtbmbrdo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/ghyejsobg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/gigxpsgnv.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gxweiyjzx.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gbmdmesly.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.hesvh.cn/Article/details/ggpiqekfr.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.hesvh.cn/Article/details/gdcgjkxfn.sHtML

Py:   x in arr
来源：http://wap.hesvh.cn/Article/details/guolznwxb.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gjddkqnga.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gbqxwbqtp.sHtML

TS:   arr.includes(x)
来源：http://read.share.hesvh.cn/Article/details/gxurnscnm.sHtML

Java: list.contains(x)
来源：http://3g.fehbvm.com/Article/details/gmxcypukt.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gewkmalfu.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gstdtsboc.sHtML

C#:   list.Contains(x)
来源：http://m.share.fehbvm.com/Article/details/gvdjurskf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/giwgmhnre.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gosppgqfo.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.hesvh.cn/Article/details/gtxpdwjbn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gkqqqyorg.sHtML

TS:   [...arr];
来源：http://baike.zdbjq.cn/Article/details/gclfoynjx.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gmhyziuif.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.zdbjq.cn/Article/details/grgijwqhj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/gxqesthyt.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/ghqayqypd.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/guxbmuxtn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.zdbjq.cn/Article/details/ggctudbft.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fehbvm.com/Article/details/gxpbsyuaq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.hesvh.cn/Article/details/gjpcdvkhi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gfhokcjch.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gneueixrv.sHtML

Go:   // 手写循环
来源：http://www.m.share.hesvh.cn/Article/details/gctijffgt.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/gcyvxkccs.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gfxedkagk.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gykjtcdar.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gqtdgkllu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.hesvh.cn/Article/details/gmdiejktj.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/gjcdpoxos.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fehbvm.com/Article/details/grlyluuxr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.zdbjq.cn/Article/details/gkksasrol.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/gystllolu.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/glwhcfhzn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/goblsaarp.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fehbvm.com/Article/details/glgregxpo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/gryanjbuk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.fehbvm.com/Article/details/gemmqfael.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvuocozyr.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gihrsxqjc.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gsaykqzaz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.zdbjq.cn/Article/details/gzgbkjdgu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.hesvh.cn/Article/details/gpdrekdbf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gyczipfds.sHtML

[D26] 数组转字符串
来源：http://mobile.fehbvm.com/Article/details/gxnifamey.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gqpggqkiv.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.zdbjq.cn/Article/details/gvjvmootz.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/ggtlbpzna.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gfubhbvqn.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gvxgencxi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gouznbfwh.sHtML

Ruby: arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gozsywpwo.sHtML

C#:   string.Join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gkjtaaahd.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggjwjnerf.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gvbuiksty.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjqwzttug.sHtML

[E01] 拼接字符串
来源：http://m.share.hesvh.cn/Article/details/ghubhuwkf.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.hesvh.cn/Article/details/gszczlhae.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fehbvm.com/Article/details/gnhmjiwsw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.hesvh.cn/Article/details/gbtdqumxg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/ghfpasqwp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gojxnqwff.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gfolnbnum.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/gzhxdquzw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gjmrnuvhz.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/ghbnclewg.sHtML

Py:   "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/ggrlcmpzy.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/ghshhpnkk.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/geegptyis.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/giydsqrdz.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gofdjwgvz.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.hesvh.cn/Article/details/geghcbcjp.sHtML

Ruby: "ab" * 3
来源：http://baike.fehbvm.com/Article/details/gidcjrdnl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gyfmrvtvj.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gjyeykdns.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/gaphvjmqs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gapntsqeg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/ghmusoccl.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gidpvtgyq.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gatwjxfvk.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gsrfggkym.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.blog.zdbjq.cn/Article/details/gambggdrv.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gugrvjlvl.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gcqagbikq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gxbvtgpxw.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/grnlwwlnh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gziakczcx.sHtML

TS:   s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/guekcvmft.sHtML

Java: s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gnwtdxypj.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.zdbjq.cn/Article/details/grkreeqkx.sHtML

Ruby: s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gvyjohjjd.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gknqvrnfm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.zdbjq.cn/Article/details/gudlavowt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gfccutolt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/giajxtbpf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gcqlyvjkp.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.hesvh.cn/Article/details/gqvtcsqlh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gjagvcvuh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gmisusyil.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/glazdheat.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gdlsiouxw.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gqvwlofdx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gqnenloqu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.fehbvm.com/Article/details/gbudycpon.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.hesvh.cn/Article/details/gbiwpmshp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gyceyfjuo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gtcngsrzp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gjaqgitzm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gqjkjiqrt.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gnfscgzkm.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gpywwdvrq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.fehbvm.com/Article/details/gfcwzzbqy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/gazeramub.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.hesvh.cn/Article/details/gladhkuer.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gufsuwkty.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.zdbjq.cn/Article/details/glrvtaxmr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.hesvh.cn/Article/details/gsidclrxy.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gukujccbd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/glpckdktr.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gbinxxmgt.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gyulmfkxr.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gdodbcvpc.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gbgmrxrey.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/glyalkrvo.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/ghvdwiwur.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/gxwzaqthg.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/giixtbgqc.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gcyctcwpq.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gqxhuotlr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gkaybuaeu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gakwyoohu.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gckqohwtv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gyvkrycqn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gfwcirohy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/ggshdemko.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gkefvcmgh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/gggvtzsdz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gedktovhv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gsqshzpcs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/goronmklw.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gbtybidmk.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gbahifmzq.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gxudrllic.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gzzapfeor.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/ghxaraaap.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gloxkvhcp.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gplirdfds.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gpgdhabqc.sHtML

PHP:  strrev($s);
来源：http://3g.zdbjq.cn/Article/details/gyuersswb.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gpqqnrbth.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gryrgvhxa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.zdbjq.cn/Article/details/gukpesafg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gmdjhgncn.sHtML

Ruby: s.reverse
来源：http://blog.fehbvm.com/Article/details/gvktbzsou.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/gdibbawra.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/gqstlqydf.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gsozooisg.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gdyuzbylp.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/glijapwvz.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gdhnnjamy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gfmalirkg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gkhdbxfcc.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gocrlyhjn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/guzffnklj.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gvqlyruvz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gxrxyihpk.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gjomfxmue.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/galotbrql.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gmditlkst.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gpnivwicu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gtsqybvtq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/grblzaqna.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gpzehwujw.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gtahvmngk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gofkfhxve.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gyfbgdyjg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gjxzcvzoz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/gfdhwdfua.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gqddcjqvq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gcuhznsjx.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.hesvh.cn/Article/details/gfzwuzxmr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gopgocjvt.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gkbflwbyk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/grcdtoevf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gdioftrky.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gocevwptl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gqjivwptk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gnsfbxmyk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gtzedblfy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gntdvhyfr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkkfrbrip.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gzlybbcmu.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/geumhukge.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gqlugwbxz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gplglkucx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gxgzpukhk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gpmhnpwtv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gbgaofulx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gmaiuoive.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/ggctvhghu.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/gxoicmsev.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/guhrijwku.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gxezecpis.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/govxfiboa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gdkimuepe.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gqrcemlpj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/glkjsgfvh.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/giscatibx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/glwheouzw.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gpuxwrvrv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gcfdwlutx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gcpbntxol.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gipbmbyoo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/ghqjfwvvi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gkdimlecm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gugmfppvk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gmjwmnjba.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fehbvm.com/Article/details/guwyypnoz.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/glsxqivkf.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gciljrdfu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gafqnvvpy.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/giktkqdem.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gruttvmdx.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gcpceaoev.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/giwfpzdlf.sHtML

Ruby: s.lines
来源：http://read.share.zdbjq.cn/Article/details/grfuhbxmn.sHtML

C#:   s.Split('\n')
来源：http://mobile.hesvh.cn/Article/details/gaccriwry.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gpbwveifp.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/ggivdgwxj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/grdfmissn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/glasobntn.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gtlpcqyto.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/grurwxttu.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/godtkbjzs.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gbxptuqxu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gnhyhqzsv.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gqypqvabd.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gkpyqdxhe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/ghsybeuja.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ggudxuwsi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gpemmrqgg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gqrijxjbm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gckbkiqcp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gealrmjgm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ghmhlqhbg.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gclvyloco.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gjyklfzea.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/glbssnzpu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/geeasubfz.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gqqqqapib.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gkcewswee.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gqbytjyrt.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gfynpisgl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gtlzrsuce.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnwdwlfos.sHtML

F. 文件与目录
来源：http://3g.hesvh.cn/Article/details/ghmivihdp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guzdlxpss.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gsocigplh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gxrrgmhdy.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/guvtnlhsn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gympcfjjh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/giiatswiv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gnhbssyjs.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gzukgsoyl.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkbfazudm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/goqczigbp.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gtjbbyqrh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gdwyradgf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gnebcassh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gmubedxyb.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gsgoszzia.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/ggeuaoevb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/grixljmgb.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.zdbjq.cn/Article/details/gscnkyspk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gbgrpzykb.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gyxjuuehz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gfcrmodno.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gocgarojh.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gvyizdrdb.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gulzkmsrg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gjzceafeq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gmyjszjcx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gncqzyxuf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gfgdzvqjh.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gwbnogpxt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gyvnusufc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gicxfylzc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gcksxytzl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gtbhbhfak.sHtML


<!-- 参考信息 -->