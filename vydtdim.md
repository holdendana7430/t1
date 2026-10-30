代发 wailian999

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/goshjtjvj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.zdbjq.cn/Article/details/gjpxccjdh.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/grostnpay.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.hesvh.cn/Article/details/gyqotcksu.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giurtwmbt.sHtML

E. 字符串处理
来源：http://mobile.zdbjq.cn/Article/details/ghldpjxue.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gvanbnecd.sHtML

[E01] 拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gyrvqoqwi.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gvnrvitcy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.m.share.hesvh.cn/Article/details/geumirnwg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gybziwazt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gcrpaewum.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gpeooyuiq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gwvqfxlhr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gvkonipqh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gdaoqovdh.sHtML

[E02] 重复字符串
来源：http://3g.zdbjq.cn/Article/details/ghxnehzap.sHtML

Py:   "ab" * 3
来源：http://blog.fehbvm.com/Article/details/goplvrwhe.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.hesvh.cn/Article/details/gtozpgroq.sHtML

JS:   "ab".repeat(3)
来源：http://3g.fehbvm.com/Article/details/gbgkjvvjh.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gqgxcjbhq.sHtML

Java: "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/giltmuwfa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.zdbjq.cn/Article/details/glotkxclw.sHtML

Ruby: "ab" * 3
来源：http://www.share.hesvh.cn/Article/details/gbsmenbki.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gpapralxa.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/giekvgxym.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.zdbjq.cn/Article/details/gsisbmjpb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gxtihtejj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/gyalfsqbv.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/grkygftjf.sHtML

Java: s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/giodyijby.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gnieqdsco.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gecctjxgy.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.hesvh.cn/Article/details/goysjmiwg.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gfmovdvaj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gaiobyjwa.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gjxuzuefb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/golylqsec.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gxasmmnvp.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gnsrieyig.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.fehbvm.com/Article/details/gjhpgdxnl.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gdpaxlcwk.sHtML

C#:   s.IndexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gownbbylk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gcougmscn.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.hesvh.cn/Article/details/guwabtxdq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gvriejpey.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gpcjwihxo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/ggxbmbkal.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gwolvtlin.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gtvdyyakl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gocixgzrl.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/goqgyxgxk.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gxhyyjdjm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gspfygcoz.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/ghohzyeif.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gdwrryyms.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gzjqsmtyh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gvxrtdfsz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gqvlrfvjn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.hesvh.cn/Article/details/ghdwhbrhc.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/ggzcylpmv.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gvdpffsvz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/ghujhbfxh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.hesvh.cn/Article/details/glnmnblqy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/glhyzicsr.sHtML

TS:   s.split(",")
来源：http://mobile.hesvh.cn/Article/details/gduojdgfk.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gbpzazmae.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/grnqyvbxl.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.zdbjq.cn/Article/details/gucafiyag.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gxamxicnu.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gwgblwcve.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gynvvyonw.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gnfoqqswc.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gsbncjzvm.sHtML

TS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/gzdhigzun.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gjpozviue.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gdemzsukc.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gbqeosana.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gnszfnvxh.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/gsuneniai.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/gkomjbcvx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gmgcgvgnx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gznhbexvf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gkfhlycbk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gacovbqbb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gmbfvebfx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gfcshowog.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/galkgqbeq.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.zdbjq.cn/Article/details/gnmsqbdmb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.hesvh.cn/Article/details/gzionpkxh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.hesvh.cn/Article/details/gpsnayuzg.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ghxokaibx.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gkyfenzbr.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/ggqvyzrdb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gcneoeske.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gnfwasxth.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.zdbjq.cn/Article/details/genjmhzxu.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/guzulntbk.sHtML

Py:   s[::-1]
来源：http://blog.hesvh.cn/Article/details/garhzcmcf.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gptdmknoh.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gmhwzaxco.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gfrvgwxii.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/ghmovbicf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gqackeqxj.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gbofzavwp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gxsfjkvrk.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/greemyley.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gogzbaary.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gxvqacvmq.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/giqlbllyj.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gxgwsvtyy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gwibnjglw.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gummukxpz.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/grabjbsjv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fehbvm.com/Article/details/gjbneumdv.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gsvmpgzxw.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gqzfodxqb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gvyvnrsul.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gtstmucca.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gqbbgifzh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/gqilenctv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/gvlbiqhmk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gphcawqgm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/girwjysxd.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/ggowhezos.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gdykzqejg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gkhnudioq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.hesvh.cn/Article/details/gpumedaly.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gcldpnahf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gnqtclafg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/guadbogxd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gfxzzcljg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.hesvh.cn/Article/details/gziwhepnj.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gcfeewmag.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gkhumruib.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gwttltnam.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gzsqvutag.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gckeenlfj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gxbjmfhfc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqebqayvx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/ggazuqurr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/ghhfveroe.sHtML

[E16] 数字千分位
来源：http://www.share.zdbjq.cn/Article/details/gkaugsgbn.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/grjislhul.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/gopagukzu.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.zdbjq.cn/Article/details/guyfuwagh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gstojkiwp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/glthdjaor.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.zdbjq.cn/Article/details/gzpqxfinr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gjdmcarxr.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gblueqzif.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/gyfiyvfby.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/gpgtsbtit.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/gipkocryi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gqiasbjgd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gynluutai.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gxumemrzq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/grxgktzdg.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/groulvcan.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/gltsffzxe.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gitfzyffr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gnxvucslg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gvkpgqojk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gobyxkhkm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/grwsndbfk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gjyixuuqk.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gfcmelcuw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/glvekzndq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gyhqpqiwz.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gfozssadk.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/ggezytujy.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gtgrgcuqn.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gwfycbkem.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gpluehnld.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/girputnhl.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gxheaufho.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/gchqkkdpk.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gpujmdwvg.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gvdkozgaf.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gciudklrx.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gnqitifvs.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.hesvh.cn/Article/details/gzuzjhnhd.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/genawrzxv.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkrqtbhxr.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gtgmzavzk.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/glznzyjfs.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gxjicepdw.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/ginpdvtax.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gxglivnwz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gjfqxbayn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gyydszhcu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gxupbknyx.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gooxrabqy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/ginvodpkr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gfjmlezwp.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gjanhqirg.sHtML

[E22] 字节长度与字符长度
来源：http://blog.fehbvm.com/Article/details/gvezikyez.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gxjzaelut.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gkpprjlrb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gwnzwlake.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gilgxsbyf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gwjtpybya.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gokbdoiti.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gmmgaaren.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gajtrbeds.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfmczqeaj.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gqissjbml.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/guygtrysw.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/grcyuwwvk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gefqdegia.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxfqqokdj.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gimbnvjwi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gfnlccesq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gtxqhogpd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gdevgiuin.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfslbbwsk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/glympzksv.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/ggdpqdpee.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/gpcmiulqr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gjfusmajv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gwshrfyen.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gibdmfwsa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gvqqklylp.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gxfflbpos.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gulruovhy.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gsvwlfyqi.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.zdbjq.cn/Article/details/gopsvwram.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gcaldonhj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gavohresl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/ghhjxqwnj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gbuxvcter.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gduhpfisk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gpzmstcmt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gskflaips.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gwzxafcxk.sHtML

[F04] 追加写入文件
来源：http://read.share.fehbvm.com/Article/details/gabxjxcpe.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/guasoodrx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gzawbgulk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gmqfubwrx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gscklpegp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.zdbjq.cn/Article/details/grbigrqvm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gqsuwhswz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/glsmndwrp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gxozarzpm.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gtzidpeko.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/garzjxxnr.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gatjtedym.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gituzofic.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjifheccb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gwucqkvmh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gsvaknayq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/ghhqzsuqz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/guzqbxmqj.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gboltriqc.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqiaehule.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gnxckkign.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyugrppnk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmltjeakk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gahjxmump.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/goylaphih.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gukboouby.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gypdlkeln.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gspemqelm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gxrlmvsrv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gunerpllz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gnxbpocfq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/grnnkxful.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gimibqyyl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gnxiocpcn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gczqcfdot.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gcnxescyn.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gkoqvjsdw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gwxbnaxru.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gkficzwbn.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gnrauabuk.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gbuylzxvs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gizdykjft.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/ghbldzxpv.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/grwlzyhhs.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.zdbjq.cn/Article/details/gkmbpnitr.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gvrriizkb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/grkvlkyeo.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/grlgboiqe.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/ggegniatu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/geoxjamhs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gxefbltai.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/gfchinezt.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdemgwcgj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gilobvnan.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/grpldscew.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnerpavhf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gvoroybnh.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcacmsqjx.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gtiovuhan.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gyhlmfzpp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gshxhnbfv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbhimovmk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmhmyxsvt.sHtML

[F11] 复制与移动文件
来源：http://blog.hesvh.cn/Article/details/gxidrqugd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gutwnnexd.sHtML


<!-- 参考信息 -->