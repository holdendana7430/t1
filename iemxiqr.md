代发 wailian999

Java: new ArrayList<>(list);
来源：http://wap.fehbvm.com/Article/details/gxtjrbmkl.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.fehbvm.com/Article/details/gbedujbnu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.hesvh.cn/Article/details/gcxpuymnl.sHtML

C#:   new List<int>(list);
来源：http://www.blog.zdbjq.cn/Article/details/gxhzkjxsn.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gwtnxahpx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://blog.hesvh.cn/Article/details/guqlqbiuf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.hesvh.cn/Article/details/gcpfkyhlw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.fehbvm.com/Article/details/gpotmqvcm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gztrhzfwk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.zdbjq.cn/Article/details/gzcxnzucp.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gobpgqybr.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gypttcrov.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/gbtgxoxin.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.fehbvm.com/Article/details/grobtrabu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fehbvm.com/Article/details/gztejjoec.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gdgtjjcsm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gaawoxdpd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gjbjgtkne.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.zdbjq.cn/Article/details/gdwlvsjvu.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/glcsgqoyj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/gkutmziuo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.fehbvm.com/Article/details/gjeubnnss.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gcrqfkgnw.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.hesvh.cn/Article/details/glkuuaswd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.zdbjq.cn/Article/details/gjjkfizct.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.zdbjq.cn/Article/details/glqujarec.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/godqcjnsd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.hesvh.cn/Article/details/gvizimlga.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.fehbvm.com/Article/details/gptcaklob.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.hesvh.cn/Article/details/gcmvalham.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gkhsxjdgd.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gmgoautzk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gzpbnathh.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gelhdwzzh.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gctcmmmsm.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gocijcvgs.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gmuxbcjfl.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/ggjbqnksk.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/ggrrqgbch.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gfapfsace.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdyzsxuig.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/gjwrolmab.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxhjqduqf.sHtML

[E01] 拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gsdbehhaq.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/geychragh.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/guphxadna.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gjsuuzhle.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gtpjfmzwf.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gfybtnpmo.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.zdbjq.cn/Article/details/gazdwktad.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gfjkrrkvw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gbajalxoa.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gmprvxclv.sHtML

Py:   "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gjxjvdbqh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gyuabvobo.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gufjeuzbn.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gnhglaynf.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gakjofnac.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fehbvm.com/Article/details/gpzijxevq.sHtML

Ruby: "ab" * 3
来源：http://blog.fehbvm.com/Article/details/gjlaojzsj.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.hesvh.cn/Article/details/gnqmweetq.sHtML

[E03] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gyhvkgluj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/grzjkfghx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gfnwfbwif.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gomjmlvat.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gqzvnecks.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gfejvwhqy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gvyudkaev.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/gilbvceej.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fehbvm.com/Article/details/gmxzqghlv.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gtvoxmeri.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.hesvh.cn/Article/details/gncsvpifs.sHtML

PHP:  strpos($s, "x");
来源：http://wap.fehbvm.com/Article/details/gumkjguaq.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gsrjomucg.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gdathtdfz.sHtML

Java: s.indexOf("x")
来源：http://wap.fehbvm.com/Article/details/giwwixcwu.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/goebodbud.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gcyifqnms.sHtML

C#:   s.IndexOf("x")
来源：http://baike.hesvh.cn/Article/details/gkwktgwsa.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/godveuhry.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/guimivgtg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gvscmolqf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/garlqobqe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/gbbtcgrhr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gsdhgofuh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.hesvh.cn/Article/details/gkmmdvtbp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gjpacelfb.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gcmndahlv.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gmeankzrm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gqbjqzecp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gpbuclztw.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbgdqzifx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/grjzcyqxa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gmxnbldec.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gpiywviti.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/grkqmsznj.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjoobwfzu.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gdspkitwn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.zdbjq.cn/Article/details/gdchueemb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gmiycpvgy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gqqrhryvq.sHtML

TS:   s.split(",")
来源：http://www.m.share.fehbvm.com/Article/details/gsrkoyoic.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/glzalvniu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/grrzgmsdu.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gmeecczrj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gpdcljuqo.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/giquiowcz.sHtML

Py:   ",".join(items)
来源：http://www.m.share.fehbvm.com/Article/details/gbbxjliho.sHtML

PHP:  implode(",", $items);
来源：http://read.share.fehbvm.com/Article/details/gzirgnbxu.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/ghdpnenws.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gwvfuvqdc.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/grvajkelh.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gbyvfmpcu.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gbkzsehvg.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gcilrkfus.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/gsspcyvxd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gpyfveqjr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gsosmvgbw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/gctaddyeq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gtpsqwtpi.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gaazaqaot.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gcekhtxld.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gigivlfhy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gocycplmz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/ghbxwpnkh.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gpdzzcwko.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/glrtmosry.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gojifysyq.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gzaizhplk.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gqytvvgvk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gfgrlmzjm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gjgjwduof.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gjfvauqvx.sHtML

[E11] 反转字符串
来源：http://wap.fehbvm.com/Article/details/gkxrqjwah.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gdjbxocrx.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/geuwjncih.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gcunkjpzv.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/glahrrbbj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gqrnuzypd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/ghlwqhfkn.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/griekttsb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gyqrrnhjg.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.hesvh.cn/Article/details/giszxtdmq.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gvdgoewnv.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gxufnpwsn.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/glwfhxsjb.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gvrkwoagl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gwxryqchw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/glebhzasu.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gycdauozm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gsbblpxsw.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gmzgozkxk.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/guqmhefhu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/grctpjpjs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gnsupjivc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/giihziejb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gqaiwrrog.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gffajwqwq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.hesvh.cn/Article/details/grgdcprya.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.hesvh.cn/Article/details/gkoylvzut.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/ggktuykcz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/guupfdigy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/galecfwgi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.zdbjq.cn/Article/details/geaeplxyp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gqhqphdbd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/ggruclish.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gmjzoumne.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gfvfjiswq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gzeqksfqg.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gucloqrdb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gdoozssji.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fehbvm.com/Article/details/gqzunomot.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gjggjfuzs.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gtkcihgrq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gvsyqmbkk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gvwictgdk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gtbdbodut.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gaiabrdjw.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gywmauexn.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/ggnganhac.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gwqniuwdf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gooxbbpep.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gvdwblxvo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/guiroskff.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gkkpzxdse.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gyijybtcc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/gtlshfyyc.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gogvgeqab.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/gzfoycirv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/gfocmisqf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gbzwjclgc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gswylswkk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvlnahpww.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gquvcnmuv.sHtML

Ruby: s.capitalize
来源：http://wap.fehbvm.com/Article/details/gqmxvvptf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/ggsmjolxf.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/ghuhbgllu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/ghwgvwokx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gzkloybgb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gjseycibe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gupddtqul.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gfmjgbwsj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/ggpwhyxle.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gvpkuxbec.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gxxdrltfp.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gwcqgooaw.sHtML

Py:   s.splitlines()
来源：http://www.m.share.zdbjq.cn/Article/details/gfkiwfflc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gfxpeqgsq.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/ggsyyxvin.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gcptkvdge.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gdtjiszdh.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/grmvrzpew.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gkxhiukhm.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gcnbkocrq.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gurlgaekg.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gmfukjluk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gsavmmxvv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gvfnzmgxk.sHtML

TS:   if (s === "") {}
来源：http://wap.hesvh.cn/Article/details/gkynzjloj.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/gabsceocw.sHtML

Go:   if s == "" {}
来源：http://read.share.hesvh.cn/Article/details/gzefgaybf.sHtML

Ruby: if s.empty?
来源：http://mobile.zdbjq.cn/Article/details/gpqtlgibo.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gqgaitxha.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/ghtayokwa.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gbtfymdse.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gkhmvksdq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/glpzibabn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/ggwcapvte.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/givmsoqqg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.hesvh.cn/Article/details/gbuhsracg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gqhfzigqh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gxpbfwyzj.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fehbvm.com/Article/details/gsjnvyeka.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gwvsanxun.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gfrkfuqic.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gfjuzlzed.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gzlzmvbef.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gwouevmzl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gjsnblpdd.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/grinkmiks.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gkfbxqpze.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvdprhghj.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gycdvcdlg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gydrgkpab.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/guqcgriid.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gjihiyqgo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.hesvh.cn/Article/details/gltnfjfes.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/ggpjmivwu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gqsnwtszf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ggtiusbrr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.fehbvm.com/Article/details/gwteqjszk.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyjkysluv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gfawlemqo.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gvuodtxxp.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gtmtlztes.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gzftugtdo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gobydiowl.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gzomizshb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gmysqvcum.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gadwwfszr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gymigtspe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fehbvm.com/Article/details/gotvgdvjg.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fehbvm.com/Article/details/goydjacqz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.hesvh.cn/Article/details/ghregcdjj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gzwfnxjhg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/geceuazhh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/guonlojov.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gfgevxgok.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gegcxarcp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gxxdbhakc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/grjrdraew.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gfgjdamkg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.zdbjq.cn/Article/details/gjtqytcdz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gzbnglozv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gnuohwccn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gjpazzksz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gvhqeelia.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gxekinuec.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gtyhutnxw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gpvklwvwg.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gtllcxxfb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/ghgolzmho.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gempujrzq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/guaubylou.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gupcllyis.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gndupiuhw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gncobsiou.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyikcabjh.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtjdjatrl.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gsszxniys.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gfipqmlgl.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/glguxfvlf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/govjymegm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gozqppbsi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/grtodwazp.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gywjdjnjd.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcbxphzvo.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gpryaprva.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gokufkbsz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/ghzqtfmii.sHtML


<!-- 参考信息 -->