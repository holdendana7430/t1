代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.fehbvm.com/Article/details/gxjsxtong.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gmauqznjl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gmolnmyqo.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.fehbvm.com/Article/details/gxpwvmpdb.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gezxwrtdm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/gbmlezdgo.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gxiiiwlbu.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gwqwaruvq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.hesvh.cn/Article/details/guoaesqkc.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.zdbjq.cn/Article/details/graepypws.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/grccetghd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.hesvh.cn/Article/details/gcunknxhz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.zdbjq.cn/Article/details/ginqhcwpt.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gumddyxfd.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.fehbvm.com/Article/details/gsiqrsort.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gmtnrjowx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fehbvm.com/Article/details/gzswmkczm.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gntqwxjfo.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gihanhtgm.sHtML

TS:   arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gkfeiwgcz.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gzksospqs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/gghsbtziu.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gooboanlk.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/glzrgubhq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcgenzhsq.sHtML

E. 字符串处理
来源：http://www.m.share.hesvh.cn/Article/details/gbugosdzn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gdrcemjgo.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gfxmtxpwh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.hesvh.cn/Article/details/guxzvwikf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gdfkwljbn.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gremjaksz.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gryjibhta.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gqigickqx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gjipqybxd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gsgnskzyu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gzqltbiwd.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/ggsgxelex.sHtML

Py:   "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gtnsyehhv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gnblwrfpw.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gajyhhdqd.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gqpkykezu.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gammdhxun.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/gbyoxdpdv.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gnypphxbp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gsnbasmsu.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gvklovxxy.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.zdbjq.cn/Article/details/gxpentgdm.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gdypyfyqh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gydjdhaie.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gsermavwi.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/gplomoqey.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gcnpjblmn.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/ggxfayrct.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/grfdrnrrh.sHtML

[E04] 查找子串位置
来源：http://mobile.hesvh.cn/Article/details/gykmxrnww.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/ggqtxfsnb.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/gjfagsayz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/glngqryhk.sHtML

TS:   s.indexOf("x")
来源：http://baike.hesvh.cn/Article/details/goeqralsy.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gbvqmnuia.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.hesvh.cn/Article/details/gqzmiqqnl.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/gnsxycafr.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gwblkgnma.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gijfjvosv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gyojmnkpt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gweuvuhnd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gitmgrcye.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.zdbjq.cn/Article/details/gwjuzzwxd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gywvzyqrh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.zdbjq.cn/Article/details/gtktdmonh.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gwdgecvtt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.zdbjq.cn/Article/details/ggkhxjfxo.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gozlkoshl.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/goyhkekbe.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gmgmxcmun.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gwqqajvpx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gbwpijbgr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gkphilnew.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gvohfjfxe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gfrawkfak.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gehmmikhe.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gdyfjrmbf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/gsouvstxt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/giojfybdr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gbwegcefg.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gsjdxlttz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gykbesmza.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gwqionypz.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gbdlhbsup.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gzdnqjmwr.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/givyccepb.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/ghvvgmkur.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/godulruun.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gxqytfqgl.sHtML

TS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gmmxlsjjw.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gbpdnvvbf.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gaiwcemys.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gynmefkkm.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gnpxvzvyf.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gvejqqnyy.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.hesvh.cn/Article/details/gqtevwxfe.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.hesvh.cn/Article/details/gzpjvxbpi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gkmultkyn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gksmpcnsx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gfpvscupg.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.zdbjq.cn/Article/details/gnvrwgqtn.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gugfnkwbf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/grpdpmwff.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.hesvh.cn/Article/details/gsftusklb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gfnhysgxm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gfturfyqk.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gcnnxmztx.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gcaljhrtn.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gqgszxjmo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/ggldlcuhe.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/giqpwsaer.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.hesvh.cn/Article/details/gfiblnulo.sHtML

[E11] 反转字符串
来源：http://m.share.hesvh.cn/Article/details/geowheqdg.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/ggyxrzwap.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gmzjdzoto.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gyiinjqht.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gbqatmxwu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.fehbvm.com/Article/details/geesfarle.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.hesvh.cn/Article/details/grpuhpwyt.sHtML

Ruby: s.reverse
来源：http://mobile.fehbvm.com/Article/details/gjuhksdia.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gdfvogrln.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/ghisuzqlm.sHtML

Py:   s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gpkwnqvvn.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gwxazmlsw.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gcnswuzei.sHtML

TS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/gfgbmozef.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/glfwisvdu.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gueortqdu.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gszalhffz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gnyixodsd.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/gbwsqymoi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gpkzjrljs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gtctujwer.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/ghlwpvhij.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gkaghrztg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/ghrefsgtn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gmoxkepsa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gjphxrcss.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gxckzzeuv.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gpwmswboc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gcbxhqoen.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gpifkcvoe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/goinilkbv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.hesvh.cn/Article/details/gbfzbcpyd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/gselckoli.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gsohkqlyo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gmvkafunk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gbfdoteex.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gwfkuycnj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.hesvh.cn/Article/details/gstcuzlqc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gngmvucxc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gzdiqhslk.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gmresrfzz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gctydtcsv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gqyeidifg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/gcljwrbjl.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.hesvh.cn/Article/details/gugkijpqn.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gxnaelwvl.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gfmhccrev.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gazsbcukh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/ggunqiwfr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gxafmneje.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gxylfsegi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gmootbvqv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gtfgsdppo.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/glnyateoc.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gstqkzykr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gubskfuvg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gghwrlfxh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gzdybwfvq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/glpvqhzja.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gtpnvqdbk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gtitsfdjf.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gqnsqtxrf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gfngssrqh.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gfpmrjfkq.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.zdbjq.cn/Article/details/grpdffccf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gnixlcsap.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gchqnlfwu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gemdvmpjm.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gckjenpxg.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gzhrkosvp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gannthwyb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/grglnpwtc.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gfbrkihri.sHtML

Py:   s.splitlines()
来源：http://www.m.share.hesvh.cn/Article/details/gaonwwazc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gbmzyuibq.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gcqdrrnel.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gdgxsaytf.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gynollrxs.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.zdbjq.cn/Article/details/gedajhwwe.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gsugrvpnp.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gcjgrrxxy.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gxzypjwah.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gezxuolet.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gpwvvdjps.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gewnlzoif.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/gzwlcfyeh.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/ghwmzueyd.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/geimyppzq.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/glbcvafro.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gnhtrvguq.sHtML

[E21] 超长截断加省略号
来源：http://blog.fehbvm.com/Article/details/gxbppdyqw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/ggvuddnju.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.hesvh.cn/Article/details/glowvquii.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gnafkckiv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gggooypby.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/glvvozvgj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gglgrjtxc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/grxcmgqll.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gphiqnmhz.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/goicydzlt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqrwjmtuj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gyeoxlaru.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gyofwhjnj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/givuggivw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gdednjitj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gusgrzbbh.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gqcifaxix.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/gjhrjjzuo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwsiivngi.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gvxwglymg.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grktjsvwp.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gbyefsoks.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.zdbjq.cn/Article/details/gjwfhbokt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gixkxklow.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gqsdgpcga.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gyuthimwy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gppocdldg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/gjzlkxtdr.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbwnvqpuv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gclgkvkdu.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gbkhsdfah.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/glgaoscjh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gsbgzpvoy.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtjckcuem.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gwtyctycx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gxtkfpamo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/granzmxkj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.hesvh.cn/Article/details/gwxndjgqq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/glagmfpgb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gzbzmcxyb.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gdenzmcwy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/gklphdyhx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gatuceclj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/ghwjsrtiq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/ggyanxzrc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gbwexazqa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gvkigujhu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gpyrcbbbq.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gajfyqlix.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gfuyzqxpd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gprewhdyn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gltuipzef.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/girypnqej.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gbpwawdxw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gcsimtcdv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.zdbjq.cn/Article/details/gqcgdynlq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gjqwxxzli.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/guqldsvwl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.zdbjq.cn/Article/details/gifmgupxn.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/glhfexwvv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghwsoupzu.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/godqysfrd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gwmxlowuu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://mobile.fehbvm.com/Article/details/gylhuuujj.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzfbetrvm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmqzqclfs.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gafzyczuh.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gymxgsllw.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gmnjsoyfl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnypqnunx.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gptuvzwdl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gajugnwec.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsypukimq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnrlsbtnn.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gfnfbkhdi.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gdiggbjcw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gxcxgsufy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gwkwlrbpn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gxgoivpks.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gsqcdullh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gceqasdjg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/ggfmhpcxf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/grvwhdwqa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gofelssuq.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/gimymvoom.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gtrjtxzsd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gtvfczitk.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gimlkhczs.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/geuzgpevp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gxcoabyib.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gzuqisclg.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gzvgcftcc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gojfyojmj.sHtML


<!-- 参考信息 -->