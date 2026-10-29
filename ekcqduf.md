代发 wailian999

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gyggrcwtx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/glhcbfyqh.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gxfgnmcxc.sHtML

C#:   string.Join(", ", list)
来源：http://baike.fehbvm.com/Article/details/geynsnvbp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glubxqzrs.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/grtbgqmlf.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gerwjtuhs.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmdyyqhad.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/gadgoeduf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/gfvkdpamj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gollpwqtu.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gbbzgmmrp.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gtifgwcih.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gnqptiwqx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.hesvh.cn/Article/details/gyasqadqz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gpcrmedzx.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/giqnyqjry.sHtML

Py:   "ab" * 3
来源：http://blog.hesvh.cn/Article/details/goauyibgh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.zdbjq.cn/Article/details/gjpjgssnw.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gvlnzxzok.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/ghiupnhvp.sHtML

Java: "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gcthovwhy.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.zdbjq.cn/Article/details/gwoyvkqfs.sHtML

Ruby: "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/ggdhnajzz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/guqunjyxt.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gpkqdxbsk.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/ggzwtmhpu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/ggpogapub.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gehgvxuaa.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gvdifpffc.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gkfazxlyu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/ghwnagrsh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/glsdsrbug.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gcapoagdq.sHtML

[E04] 查找子串位置
来源：http://www.blog.hesvh.cn/Article/details/gbgfxqdgj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.hesvh.cn/Article/details/gemrrdxgo.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.hesvh.cn/Article/details/gcsspyokn.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/gszrlvrdu.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gkjvfkvbn.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/ggvnecuil.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gwijafmjq.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/ggdqfuhnv.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gjvdlrofj.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/ghozzcuuo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gsolxleeq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.hesvh.cn/Article/details/gykmavuyl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/gvduuylhr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/guukwtmzz.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gsahquknc.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/grerswnuf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gmncchbxt.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gwhylgsca.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gdsdaeayp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/giahyfpth.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/grcxgpdif.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/ghxiabhvn.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gwbxyoasg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/geciuygee.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gyygdllhz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gvfpoytkc.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gxrsamklr.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gxwckmmkd.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/guzzqzrib.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkugzrxjm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gjuqzuazh.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gfbugwfbz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/gjtpcqqcb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gqcjarxzw.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gdbaqxgqb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gdxexklut.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/geefblzmv.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gwfngqxff.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/ghqmcocrt.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gfrtwsxim.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gbhrlejoj.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gejebrsbj.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gnugiqego.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/glukvalmb.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/ghodesvin.sHtML

[E09] 去除所有空白字符
来源：http://www.share.hesvh.cn/Article/details/gdnwxpvti.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gmglaoogk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gotqcoqdn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gxrtxvuno.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fehbvm.com/Article/details/gqidnlcnr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gmadhxuwx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/giwuhibxw.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gerabvypy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.hesvh.cn/Article/details/gbtpcwnhs.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gceatvcvx.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gvbxsdpdz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gpbchhyst.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gmxqvrlnp.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gjuppnbgw.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/ggtzjcumn.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gdeskaqck.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/ggvssasji.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.zdbjq.cn/Article/details/gwbznszid.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjxbjqpmc.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gacgopekr.sHtML

PHP:  strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gvdntzonp.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gtxvcgpto.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gwgfasetz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gsdgsdgdc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/geyddsbsr.sHtML

Ruby: s.reverse
来源：http://wap.fehbvm.com/Article/details/grggojqzt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/githtgvcw.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gfdybkkej.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/glfocrxko.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gzewwkvsx.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/gggknbtye.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gsneohlhi.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/guldvspqk.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/gqvineikl.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gidhmvofp.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/grnyvmlig.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fehbvm.com/Article/details/gmyqfnazt.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gcnfjjxif.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gsbribelf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gsluvfqjk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gbgqujdnp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gnhafikyi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.hesvh.cn/Article/details/ggirawkxa.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/gslcjwpwp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.hesvh.cn/Article/details/grjrxdmvv.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/ggtgqfayj.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gljwvobpc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fehbvm.com/Article/details/gwqcxpauy.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gghactiis.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fehbvm.com/Article/details/ghvmnujsj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gottuizan.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gwmzzerwp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gdfxsligv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/ggictltdi.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gowhecrje.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gtodfqpev.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/glornoknl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/giwoibsko.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gdrwziojf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/gaxqmfxbi.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gqljpumpb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gkulffjpv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/goqbteisc.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gnouqorrd.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/ghlzeieaa.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gttybkweh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gwpszrrbh.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gnhamwuwm.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/gefyshksu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gibyinigf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gaagiypsu.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.hesvh.cn/Article/details/gxrneljgv.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/glojebvuh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gfxlvbiyx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gckbgxjbp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gepudxwoa.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gnhqhwqeq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/glqsglrht.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fehbvm.com/Article/details/ggeoezoph.sHtML

Ruby: s.capitalize
来源：http://mobile.fehbvm.com/Article/details/gtmqqgcyw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gbbpletfi.sHtML

[E18] 模板占位符替换
来源：http://blog.zdbjq.cn/Article/details/gmxwezvoo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gztbtggnh.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gxdktxobs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gdkyxsczh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gyrhjvmfc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gcurbzmqu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/ghxpdkgij.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gvdopqgkl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/ghuqffeda.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/ggglrzgjd.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gtldbgbov.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gqwxlxujv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gehmvghzm.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gdtsxfehx.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gjheawpsk.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gwlsemkhu.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/ggdzaffpp.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gvdickaoq.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.zdbjq.cn/Article/details/gevzkqanp.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/gygwqmvfv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gjfedpwql.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gvlmbcibt.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/ggeayquiu.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/giqlepusz.sHtML

Go:   if s == "" {}
来源：http://3g.fehbvm.com/Article/details/gkrswwdzo.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gloxeoewv.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.fehbvm.com/Article/details/gnuedoarm.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/guogvcbsw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gxxqldhas.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gngsvdrcn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gdyiwqqpy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gbpcapvbc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gwffuowxj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.hesvh.cn/Article/details/gcqqorwzy.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/goconezmv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gdimtncyi.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gexdqzopx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gkymojiih.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gtlouhpnc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/ggfojryne.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gwqyaqzhc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gkjejhcvl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.zdbjq.cn/Article/details/gwqcrmqdt.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gygdctowc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gdrowsoha.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghroqsfja.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gaurpmnii.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gkjyutkkc.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/gfeedhqlw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/goalycpso.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/giyzgmcwx.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gimcofhoy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/ghekoqeis.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gwdlnkbnz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.zdbjq.cn/Article/details/ghjmemzac.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvudofyjc.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gbetlkrcs.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gpzwnayyq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gfknthlgz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gzjvyrgrc.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gihsqrojp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gqschxnkd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gholiryeo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gaajxqdtr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gucdpmqcr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/ggksitpnk.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/ghzpqbivd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gukyytavw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gpyvzidhn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/ghgzrubaq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gubidxsmf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/gdwaplaye.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/guqnjeufb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gafcttses.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/glyjuojyt.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gemaislbn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/geyckaqjs.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gwkvzxlks.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/giyplawhp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gtjefbksu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gjlkywgex.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gvxskatfb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gnczgntzq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gmczihbeg.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/ghslmcpko.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gkmucmacn.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdlpospgd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghncdkovx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gzvmyhqsp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gdbjcydkc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gccvhkkkt.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/givaynmll.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbtyqsfxd.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gdjukdwts.sHtML

Py:   os.remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gensnbbdn.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gddsmmele.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjebxoniv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gsvkjhnvr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gmtzxzbkf.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpxogoiwl.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gsthrlsnc.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/geltuickh.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gbugappgh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gbziztcpy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fehbvm.com/Article/details/gnsnklqeg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gjixdangr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gaqrbyhtz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/grjyxlrct.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/galvlpnvf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/ghqyyceza.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gzgiwqtvm.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/ggqlfgbkw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gcvlyombq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gscknbqpw.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gysjvbwvz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gghtufhfs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gomokosom.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gjjyivfnt.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gmpvhejtg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gpworyxup.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gsriaarof.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gecteiynz.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gxheyfxfh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gexivgmfn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gqaunjjjw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gzeknmepm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gfdkpulew.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghvxhgknf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gesblbzge.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/givljkvfn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsiuvwjes.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gkibpeano.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gizoepfyh.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gipckqdvp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gzqtltiir.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwxrcoeym.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gjpmxsaeg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwdguibwx.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/grltljfji.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gtzqifghm.sHtML


<!-- 参考信息 -->