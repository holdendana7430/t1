代发 wailian999

[D23] reduce 累积计算
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcwnuubc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fanxiaobao.xyz/Article/details/gtxxjijzj.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fanxiaobao.xyz/Article/details/gofdvjruq.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fanxiaobao.xyz/Article/details/gajmcnbtb.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugjxcfbj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpotordnt.sHtML

Go:   // 手写循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdiynjxs.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fanxiaobao.xyz/Article/details/gxeenvwok.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjcnzjii.sHtML

[D24] 字典 / Map 基本操作
来源：http://3g.fanxiaobao.xyz/Article/details/gipxmjuci.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fanxiaobao.xyz/Article/details/ghxlxqejt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gczwgelhr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpbbbihd.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glhspxhxk.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgkfuzex.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtflijrlx.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fanxiaobao.xyz/Article/details/gbojrwatn.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqoekzpm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobdsqyoy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnyxopev.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxfytdzl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gekxeeqjg.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fanxiaobao.xyz/Article/details/grtzbvsxn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzmntsbx.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvedafsja.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqtslsjth.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gsnrxzizo.sHtML

[D26] 数组转字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gtvuswkbn.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fanxiaobao.xyz/Article/details/gughfdqhg.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.fanxiaobao.xyz/Article/details/gthkhtzna.sHtML

JS:   arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gueschint.sHtML

TS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvvghsbc.sHtML

Java: String.join(", ", list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gyudjzupo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gmvbnegph.sHtML

Ruby: arr.join(", ")
来源：http://3g.fanxiaobao.xyz/Article/details/gyykdcbja.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfzqrqub.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gsirkhokd.sHtML

E. 字符串处理
来源：http://3g.fanxiaobao.xyz/Article/details/gqszolrhh.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glfqyoasb.sHtML

[E01] 拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gbesrunua.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdymgeae.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzfmxlgnb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyuhhcbg.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fanxiaobao.xyz/Article/details/ghfvpsdlj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fanxiaobao.xyz/Article/details/gbkocvoho.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gnfzbwjlh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fanxiaobao.xyz/Article/details/glpzglrhb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiczykiz.sHtML

[E02] 重复字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gjgvhbhsv.sHtML

Py:   "ab" * 3
来源：http://www.share.fanxiaobao.xyz/Article/details/gfpnuhjni.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gavakwsve.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fanxiaobao.xyz/Article/details/gmjlmpjrg.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmrqmhiv.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gublbfqrc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gabaafchy.sHtML

Ruby: "ab" * 3
来源：http://wap.fanxiaobao.xyz/Article/details/gygcbyaab.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/glkpbbahv.sHtML

[E03] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gqyocptge.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpukydngi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqevuies.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gkhmhkxdu.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gqmfilyqt.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbsvutji.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.fanxiaobao.xyz/Article/details/govoohtgl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fanxiaobao.xyz/Article/details/gexvvvyfq.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpkaqhqv.sHtML

[E04] 查找子串位置
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwnoragh.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/guylthvfb.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhvjfmkw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fanxiaobao.xyz/Article/details/gkvdnydak.sHtML

TS:   s.indexOf("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdfshkkp.sHtML

Java: s.indexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gavagesre.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fanxiaobao.xyz/Article/details/guvblqdfu.sHtML

Ruby: s.index("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwchjzcbn.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fanxiaobao.xyz/Article/details/gftytfyrt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyavbgpw.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpggvtewu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidzrhpwf.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqffaztin.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gfhyrnrij.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gbcpkirum.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.fanxiaobao.xyz/Article/details/gddpvqeen.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gouxkegds.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhtlhcjf.sHtML

[E06] 替换子串
来源：http://blog.fanxiaobao.xyz/Article/details/gciamcmss.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gukkzpeki.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghedqagtx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjivghfs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/ginyxuolg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehdobhni.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzetnyoic.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogunvgiv.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gdzutsbtu.sHtML

[E07] 按分隔符拆分
来源：http://3g.fanxiaobao.xyz/Article/details/ggcfyrxcr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fanxiaobao.xyz/Article/details/gdkatpjip.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzedsqbce.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglmmnexd.sHtML

TS:   s.split(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gubfmqyfa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fanxiaobao.xyz/Article/details/gyvurclnq.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwaygcrl.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fanxiaobao.xyz/Article/details/gdeyhdtuh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaymrvpxb.sHtML

[E08] 数组按分隔符合并
来源：http://baike.fanxiaobao.xyz/Article/details/gfgzmmqzt.sHtML

Py:   ",".join(items)
来源：http://wap.fanxiaobao.xyz/Article/details/genhzlofn.sHtML

PHP:  implode(",", $items);
来源：http://3g.fanxiaobao.xyz/Article/details/guefwxtpw.sHtML

JS:   items.join(",")
来源：http://baike.fanxiaobao.xyz/Article/details/gipmidtyg.sHtML

TS:   items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjvlfqqb.sHtML

Java: String.join(",", items)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghshhwwsy.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqlkfgyu.sHtML

Ruby: items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gcacslqeq.sHtML

C#:   string.Join(",", items)
来源：http://baike.fanxiaobao.xyz/Article/details/gmgrffezm.sHtML

[E09] 去除所有空白字符
来源：http://blog.fanxiaobao.xyz/Article/details/gyktqcnme.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtvawydy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gherchrif.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gkkeazqfm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjmbmime.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/grrwnssre.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fanxiaobao.xyz/Article/details/gaksnvdzi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqlsqyco.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjwdfvby.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.fanxiaobao.xyz/Article/details/gnudzoymy.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtmwkwns.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fanxiaobao.xyz/Article/details/gfbcvxgtf.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfolbpat.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvwcgjcxw.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowrknxec.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjslqhkrl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggtztsibl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudmlpahn.sHtML

[E11] 反转字符串
来源：http://baike.fanxiaobao.xyz/Article/details/ggyzlcljy.sHtML

Py:   s[::-1]
来源：http://3g.fanxiaobao.xyz/Article/details/gqoxypgkq.sHtML

PHP:  strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyssadua.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsltgots.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fanxiaobao.xyz/Article/details/gwldcflkc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fanxiaobao.xyz/Article/details/gotyvpfcu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gvfqzlfvm.sHtML

Ruby: s.reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggupmywnb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqdcnetm.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fanxiaobao.xyz/Article/details/gssyioegn.sHtML

Py:   s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gidptfovc.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fanxiaobao.xyz/Article/details/gljvzedgj.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgwsidql.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfclnoawx.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fanxiaobao.xyz/Article/details/gfxqsmpvl.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fanxiaobao.xyz/Article/details/gxlshayuw.sHtML

Ruby: s.count("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gmgnanzbo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzlcjhru.sHtML

[E13] 逐字符遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gxddqoyod.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fanxiaobao.xyz/Article/details/gakseljol.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjnbakbzn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqvqathc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwuyrtls.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxiikwuwb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssxgeijs.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fanxiaobao.xyz/Article/details/glwwjlyot.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxheweuhv.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctpviewv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbvpxkef.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gcjpvwkww.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fanxiaobao.xyz/Article/details/gsybmiqeu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwnrpjru.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhjspbpj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzglltihd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.fanxiaobao.xyz/Article/details/grnbvyayg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/gpepkkynx.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fanxiaobao.xyz/Article/details/gsdljmkyy.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrzlgsdq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzccylki.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghjeguvao.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gzebazbbi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsmxstnb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmshyryap.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gqbqsleoh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/guuufocum.sHtML

[E16] 数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gijstunac.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghejtdmdb.sHtML

PHP:  number_format(1234567);
来源：http://baike.fanxiaobao.xyz/Article/details/gljiaoloc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhehlgna.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fanxiaobao.xyz/Article/details/gcavmocep.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.fanxiaobao.xyz/Article/details/glsgtuezc.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fanxiaobao.xyz/Article/details/gdgqpmtnt.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnkpwhax.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoagwakb.sHtML

[E17] 首字母大写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawwldzrq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxqhvcjm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfizndzc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzjlcwgl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhxumwzg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gruvntygi.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fanxiaobao.xyz/Article/details/gncmcmmir.sHtML

Ruby: s.capitalize
来源：http://baike.fanxiaobao.xyz/Article/details/gusbpkbwo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fanxiaobao.xyz/Article/details/gakarykoo.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclmhmqms.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fanxiaobao.xyz/Article/details/gaitgrlxt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghohxixqd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqhiddect.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gytnelbuv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gckkjnlwk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxurodylk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grmbfmqob.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiajgucp.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fanxiaobao.xyz/Article/details/georkapus.sHtML

Py:   s.splitlines()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwqiueiw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gipwyyqxn.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgdrfdoy.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/gtipzhnja.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmjygzsf.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gymqshfuw.sHtML

Ruby: s.lines
来源：http://wap.fanxiaobao.xyz/Article/details/gesivpcid.sHtML

C#:   s.Split('\n')
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfjcqggx.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fanxiaobao.xyz/Article/details/gelrepcil.sHtML

Py:   if not s:
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcubcpoac.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fanxiaobao.xyz/Article/details/gxgddbulm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gsghbbake.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckghxafs.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtimhhimw.sHtML

Go:   if s == "" {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdvbkbfe.sHtML

Ruby: if s.empty?
来源：http://www.blog.fanxiaobao.xyz/Article/details/guezdfvrz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwvblhzr.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzbolxwh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrcmvdug.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxofvykes.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxttoxczr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gvsfzgecy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrdutmfz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkrmlztj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzzqdstv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gjohkgvfz.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxqvtqwp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzmixfdp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gosadowbu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/gryvpwswq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaazlqcck.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzfjciuy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfpznqxr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefbtpbtt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fanxiaobao.xyz/Article/details/gucnziryu.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gyucaovsq.sHtML

F. 文件与目录
来源：http://read.share.fanxiaobao.xyz/Article/details/gezfwieuj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/goossezid.sHtML

[F01] 读取整个文件
来源：http://wap.fanxiaobao.xyz/Article/details/grspkalmu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzbujjyg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/grreceuwj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.fanxiaobao.xyz/Article/details/gvdlyitaq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/gnhhnokjh.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/gvjaudzpl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.fanxiaobao.xyz/Article/details/ggfzctopd.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gftrdrcgd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjunlfzi.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpgabhxh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fanxiaobao.xyz/Article/details/gkykbvxrq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/grpiyngnu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gipzrshru.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfvsmmzzt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywpwjald.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fanxiaobao.xyz/Article/details/gootoyouy.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fanxiaobao.xyz/Article/details/gfeyxhnsg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fanxiaobao.xyz/Article/details/ggymxdaqb.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fanxiaobao.xyz/Article/details/gxtlwpevl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fanxiaobao.xyz/Article/details/gdvqjgrwf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhnoqjxi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsalhcvu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/giqthtqes.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueebykwy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtffujkki.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdamgttog.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gxhswbjwp.sHtML

[F04] 追加写入文件
来源：http://blog.fanxiaobao.xyz/Article/details/gujwgjsem.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnoazlrw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwsurydi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gmaiheqhl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxnabfel.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzihwhoik.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmazwxwke.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpgkxiqy.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fanxiaobao.xyz/Article/details/gitbepvrg.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/grnfvpoec.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeythdyh.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gmvvjrvys.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgpuhzrq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gceazvlsx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqmxaawi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fanxiaobao.xyz/Article/details/goiyfefwq.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggevybvqa.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnltybqoi.sHtML

[F06] 删除文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gucjnajoq.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkniurofw.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/goqdtnqyp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnihzuqrt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnnfhssvo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvqoytdh.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gepcutlph.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gvkitlxsu.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gsnejyvnn.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fanxiaobao.xyz/Article/details/geknrklkw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnhxkdxd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtenxksr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fanxiaobao.xyz/Article/details/gnnhckpre.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fanxiaobao.xyz/Article/details/gjmqnzkhp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fanxiaobao.xyz/Article/details/ghlwfrzwj.sHtML


<!-- 参考信息 -->