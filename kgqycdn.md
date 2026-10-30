代发 wailian999

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gtyhevqtw.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/ggzvoutom.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/grsxhgtmn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gzknqazyj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gygulxedg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.zdbjq.cn/Article/details/ghgzelbsz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gxpoclnek.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gzttjfwff.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/ghkkusouz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gsnzmdegq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/galwsrztx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gtkeewpgo.sHtML

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gbdsmwsue.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.hesvh.cn/Article/details/gbcxnebhd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.hesvh.cn/Article/details/ghokrorql.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gvqhdmjjs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gaskltupl.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gapbsgwuv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/geopuynjg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gspunkhbx.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gboabfuqj.sHtML

[E07] 按分隔符拆分
来源：http://wap.hesvh.cn/Article/details/gnooeuqfq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gclsodfzw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.zdbjq.cn/Article/details/glhcdsogk.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.hesvh.cn/Article/details/gidxfgdlw.sHtML

TS:   s.split(",")
来源：http://www.blog.fehbvm.com/Article/details/gfecdugax.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gtwxgqimp.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.zdbjq.cn/Article/details/godbxcjka.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/grhpminjr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gnmsbcfrn.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gbktkbqbu.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gggiceniv.sHtML

PHP:  implode(",", $items);
来源：http://baike.fehbvm.com/Article/details/gumhouejp.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/glzmddkqg.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gvlchruwx.sHtML

Java: String.join(",", items)
来源：http://wap.hesvh.cn/Article/details/gjmltoewl.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gvgvbtfyz.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gbvbasmyd.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/geidxmlmg.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gyvdtxqzj.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gkpfmwtyx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gifytxwqx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gwpodergn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gbqitjelw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gweynpoba.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gigkgfdci.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/gmqgjfinz.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gzejcooqj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gwiykcyim.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gdcmqdsrd.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gjqfkjhdj.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gqjhtxrwj.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gtbxlokwr.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gpyubffyb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gtginttvh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gtjruzrlp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gudrplncj.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gysuortcy.sHtML

Py:   s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/guxswoexj.sHtML

PHP:  strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gflddbbmv.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gvvkgmufk.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gipmjkech.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gfyytffht.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gbumrqxma.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gispjhabc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gvavuiwfe.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.fehbvm.com/Article/details/gakhijfic.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gcfyzyztu.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gmhrebajl.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/graonhdcr.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/goegpvkpg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gsvqlpqyv.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.zdbjq.cn/Article/details/gznrizxml.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/guikhxblb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.zdbjq.cn/Article/details/gyxhygcjz.sHtML

[E13] 逐字符遍历
来源：http://m.share.hesvh.cn/Article/details/grgnydvmy.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/grojqwmrp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fehbvm.com/Article/details/glakrtevp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gorqffvpz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gpnnvetwm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gutpnyppr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gfiikqvlh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gdqrvzyqw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gvpidthju.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gpslordde.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gxzalqyhh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gctnkebhe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/glixkwojf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfkjwkvbh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gocdydvbk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gxsyvxtyn.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/glwdtuoqr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/gzyaikbtf.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gjnjavtyo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gbrjhgmwd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gquzqtbsp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/glxffilzu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gdztukpio.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gmfgxcqox.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gkynfzewt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gndynnhyp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gqqxbzfbd.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/guuqafatv.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/ggarnrzss.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gcauqqgyd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gxqjbjvga.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gxidrarym.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gnybxbrnw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gtipobbbp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gwaqbfxsa.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gstjubklq.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gspogyfrl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gjrkvabax.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gtbqllbvr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gbmnvigpi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gxuwmfgsa.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gijkyqsdo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gidotezys.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gdrsccteq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gmlsschgf.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gjkvwmome.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gtsgmhnza.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gmutaxkdu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gyvckiwbt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gcuncewbu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gzpjawmsj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gbnsvmpeu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.zdbjq.cn/Article/details/gzvdkhban.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gajrenziy.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gurazzpfc.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gndnlmgtl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gtiuujaxl.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/guiygmtoi.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gckhptbiw.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/germkwozo.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.fehbvm.com/Article/details/gginougsj.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gdiqktnak.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gsxhaawxk.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gqglprxqu.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/guopbivev.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gaepmrffz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gxazsyywh.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gmcnpsgcg.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gkaldxhti.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gyknxrlos.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gwzmwfoui.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvhtdivsf.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gntvypnxr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gqfnujwsp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gtuhwjfzz.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gwchfgena.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gqqyodntp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gytiyuvyd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gihtklhvn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/glfwpxhki.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gjdpgfgag.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/geuiuznyq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gzntawkwu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gcmqzzgyk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gikkwpmil.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gvywqkkmc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/ghoicemvs.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gqrbchbcw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gwnwkfwsb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/giqytluvy.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gelvycqmc.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gdjhbcuij.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gimoekopr.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/gyzojsicv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gxbkwrafo.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gkeexpryg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.zdbjq.cn/Article/details/gnydunhbm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/glxhepddx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gqrfdddzp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gdthxdyqv.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkdpspkat.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmelwavrw.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gglkrkxtm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gultjgmus.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gympkicbm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gtldyjlzf.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gnvamzrwq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gbonstcda.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gsumlwsvo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gihcudwso.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gofeqjzzk.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/guamndute.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/guycxdtjy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/ghzprbtzt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gxhvmyrtt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/glckxzktz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gxnuqmkqu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fehbvm.com/Article/details/goqbbevwb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gezlistvs.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/giqdxlqll.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gjniwocsq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/gwqqdofta.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/golkfezbv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gvlcmnzih.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/ggvakmyxd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gzyuebynn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gzxpkqdij.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/gjdozolbm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/gmbmwmwld.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gkyfvikbt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/gzxofirhf.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/giyjdmkhd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gribzdntd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/grojjfbki.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gjtbvropr.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/gbnxsaifv.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpadwocfr.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvknjwdgs.sHtML

[F06] 删除文件
来源：http://3g.zdbjq.cn/Article/details/gpqsezdyd.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkyiagcya.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmtkyxwzj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gnzqukrjb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gapunkobi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gdnxerwgb.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/grybsacpv.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvizwvchz.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gysypobnx.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gpltilkkx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/ghgzmfqae.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gqqnsghvg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gxkddjndc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gpzgnyjks.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gofphvxmb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.fehbvm.com/Article/details/grghcyjqj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.zdbjq.cn/Article/details/gqkkolebn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/ggmjrituu.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gvbjibmoj.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gyaomkpee.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gdfhdythr.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gecyojqep.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/gywhauvwc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gwphhrvoj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/giyczfjuk.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gyytxdugz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/guyfnupnr.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gszfdefcd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gykytrmcl.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/ghrxhfpni.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gnzuliphm.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gprwaswjc.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gfocmwfxj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gzmwdxnkh.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjiiwwwte.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.hesvh.cn/Article/details/gbertmkkz.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gcyykinjt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggthsrstq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/grznkxwga.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gcvgazevu.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwhhphvnh.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gatgpyquj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcjjapemm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmurohfkw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsssqrxgi.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gdoiltksr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gfjotsvuu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gdersvphm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/ganfwwugl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/ggnvrxyvo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gvmwidxvf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gmkppzyhe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gzntwnulj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gadrsfbaw.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gegzhehit.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/grkqmhvzx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/geexlxqzy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/gvzdhphqk.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gruxkahct.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fehbvm.com/Article/details/gmdqzwkfx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/glcpvwbxi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gfzklykwn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/ggubtxgcn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdncouojk.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gzljrhrpo.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghwdeoyyo.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/grlicdnjx.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gvpaudcjc.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/ggyyqdmhr.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gavrjjthm.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gapgznuvv.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gagzsipty.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gvduirmcw.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gkgpiyndi.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/glgiiwkqt.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/ggicwdzxt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gudlvwleg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gmvovphoc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gajvtgbyt.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/ghwerfqls.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gxulomomk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/grioweluj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/gupncfyhm.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gtouaiscm.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gawvyatdt.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gozseaasp.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gepsregcz.sHtML


<!-- 参考信息 -->