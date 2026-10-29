代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gglduxyyx.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/goxjptcmv.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gsgchfidu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/gokqsuezs.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gutkpbjcm.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.hesvh.cn/Article/details/guusdnrox.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gqaxvsxnn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gwwzagjgf.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/gscrttmew.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.fehbvm.com/Article/details/glrlxvhdd.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gttzimywm.sHtML

Java: s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gkwqsxbqs.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/guiujkbwz.sHtML

Ruby: s.index("x")
来源：http://3g.zdbjq.cn/Article/details/gkicuwllt.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gygqeskqq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/gvunsfoqj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gppqsjomg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.hesvh.cn/Article/details/gcwxrxzjp.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gjafdryuc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gltvlfunh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gtbhbemru.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/gjpwvxzev.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gusmkkaif.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gtwrikamt.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gldwvhrbx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gfgbqgkdt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gmqhtjpdx.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gkwowrkuh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gpywdeneb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gnhtaqeyq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gfcxcndsw.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gabptehtn.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gdbzmycth.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gjmrhnfog.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/geescdknc.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/gpctqewyb.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/gxvcmqsxf.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gamrtdfej.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/gomvcgbkb.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.hesvh.cn/Article/details/giyuzkdiz.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.zdbjq.cn/Article/details/gchppxqmw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gzrluplla.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fehbvm.com/Article/details/gvjweoisb.sHtML

Py:   ",".join(items)
来源：http://m.share.fehbvm.com/Article/details/gmsoqsraz.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/gfhnlagvt.sHtML

JS:   items.join(",")
来源：http://blog.fehbvm.com/Article/details/ggalqxdem.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gtgqsrdbz.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/ghlxaqqiz.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/goupvhknn.sHtML

Ruby: items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gnwyeqskf.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gyrwfopic.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gdmfalrff.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjyefwjxm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gtcwyhdzh.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/gyiliudnf.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gdcbdjlnk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/guwactavk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gjucxpwda.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.zdbjq.cn/Article/details/gsgudkgzx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gxooepoug.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gueocqurn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/ghnugiwnm.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gxbvjupax.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gsfasagpv.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/giiengbcy.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gzofdsdus.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gfsefyoow.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/glazxpzlj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gaggjndlb.sHtML

[E11] 反转字符串
来源：http://www.blog.hesvh.cn/Article/details/gcpqowexr.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gunjfxlsv.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/gxzzxmqch.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gldvtoccz.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gcfjuixkr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gonqjxzds.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/ggrirxpve.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/ghpagutlq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gyxbndyfa.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gjqwhvyyh.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gspyrlaxs.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.zdbjq.cn/Article/details/gzvpzbmyr.sHtML

JS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gapnzsxff.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gdafhzwnc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gdjjepshm.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.hesvh.cn/Article/details/gcbtgmmib.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gtsdejwio.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gapidzfwh.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gjscrgowi.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.hesvh.cn/Article/details/grtotijdx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gocrfermi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gomfpjpab.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gtaemwclp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gygmrypst.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gnljhrtmt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/ggrgmlccw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gbrvmbzzc.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/goefjgjzc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gumfraffi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/ghrabdxmv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gmjarrasv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gkpgpddft.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gpfkhmgui.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gadxizkac.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gyubpilst.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gbnodlqkj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gazircbqb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gttgviokx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gorazyiqe.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gsfggjhtd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gyudxphxo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gnwojyojo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gigqicbtu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.zdbjq.cn/Article/details/gngmswxwr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/goxckfgjh.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gfmmxzrpe.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gofvsttcm.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gxyyuzcul.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gfvuofduo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gbaovssqd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gfdqpqhfl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fehbvm.com/Article/details/glgzttrrf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gnminsnsw.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gqxxdsrrm.sHtML

[E17] 首字母大写
来源：http://3g.zdbjq.cn/Article/details/gwpvbwdpo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/gvegzixae.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/giaiiqhst.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/grzqgkent.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/gkrceheua.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gkvdyrigw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gxkflnzez.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gclzlkblx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gqyxtdhit.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gttkhteoe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gcrikeidz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gpddnyebl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gcakpwmwj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gronlcghq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gfiqnbemz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gkrbquqjx.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gxvifkncn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/ghszbtmcb.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gunwlppmx.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gphyvcfuk.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gnhobwxot.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gblopcooo.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/geczmqmhw.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gnlefbvkk.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gfamtfgnh.sHtML

Ruby: s.lines
来源：http://www.share.fehbvm.com/Article/details/gogxlzbmq.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gxuxezeah.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fehbvm.com/Article/details/gxisfykkn.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gxplbvehp.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/gluawirma.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/geadaadya.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gjacvrfia.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gsrxbascc.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gcocrenbe.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gibzsmxwa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gcxfvqjka.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gomoqyoei.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.zdbjq.cn/Article/details/ghvwnqgzp.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gkbulmvyw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gefplcjas.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/ggigvoxsv.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gqrmwdqor.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gxlrebtsi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gflqhrjsn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ghgzvuttu.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/geqxvmzzj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gykzoekyl.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gqghwmxim.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gicugupye.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gkguxcdai.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gxtwecrjo.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.hesvh.cn/Article/details/gaodpzzif.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gerrfnodo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gtdwswkga.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxhyxaitx.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/grjkqqixr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gnzdjwwmv.sHtML

[F01] 读取整个文件
来源：http://blog.hesvh.cn/Article/details/gsmfpuwbg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gbkugtfux.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gymwdgtpp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.hesvh.cn/Article/details/gxclyyhen.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/glpcjhjwv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gqlyhaaqf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gmbtkppap.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvkrvxwvh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gnuwpbulo.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gmtdjyhlz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gwyynlvhf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.zdbjq.cn/Article/details/gckgyeetr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/guaxzqqyx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gdofghyuu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gkujvxmwe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gvxcvztgu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.zdbjq.cn/Article/details/gjhbenfmb.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.hesvh.cn/Article/details/gmozylwnq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/grhqlslhv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/giomgvvnb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/grvburrnj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gjspklsxm.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gamtacyka.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/grvnuhunz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gafwcaloe.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gmkurjuye.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gymizwmat.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gslvdlqxd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/ggcxvojej.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/guicqimui.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gcrrdmcfs.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gedgaqxxv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/glxstduoa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gerrxlzjy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gwjavhodg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/gzdhjnnvm.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gadqqldkt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/gwrsytrqt.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gvahodmzv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjapqlwip.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwpwyhsag.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gvgibudex.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gswbptgey.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmxwvobxe.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ggqwdewlw.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gbvyufgyc.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gmnxgcezk.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gvdghyetm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/giwqusyxw.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmplazjow.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gvmwuwlkq.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gkflmlqmv.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gucakiivg.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gmfpwxelw.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gupngxjjx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gwmwxmgjv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gwktpfnlh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/guqxszmmu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gomchrzpm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gqqvfrtbu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/gpdjxilip.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gcehuukfg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.zdbjq.cn/Article/details/gmdrgkzae.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gpgymusbs.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gqiadyswp.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gbpboptfq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gttdlzzat.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gtmgnlpwz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gltsgtnrr.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gydxuwvsd.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/grkwkqnpb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gorqbmzvd.sHtML

[F09] 获取文件大小
来源：http://3g.zdbjq.cn/Article/details/guvxqjjbv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gpjsejrbs.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gixtjnjgo.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/gyngcgeex.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gwxcoegvb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gcjuwtzzw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gbdtqiaos.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gikvdgdbs.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/goqjwfvxy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gifyjnttd.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghjgnzuzo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/guzlrfwci.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gnrfarkwb.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gfokrqbxv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gmxjftmql.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmaeghjqc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gpoxbpdkz.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ggyiwjpsy.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gposyuwaf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gdwcgmryt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gfhrpsfub.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glzhkfqjg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gcrqnihiw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gwlqstpni.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gylrozrcc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtjpwiwep.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gruomhfdj.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/ghgivxunh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gibxeqxrt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/ggrqjjycb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gwqicnjga.sHtML

TS:   // 同上
来源：http://m.share.fehbvm.com/Article/details/gcicdutqa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/ghypmbymi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gfvtsgpvb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gpyjzgrax.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/ghjyzzuyu.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkrlevgex.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/grukurhru.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwgditbcd.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gzmkcuyla.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gpsxvlzid.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/glkpyoqok.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gqshahdfe.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/gorlpcitf.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gedzdxfap.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/grzyfnope.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gyhdcdach.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gjwfimcld.sHtML


<!-- 参考信息 -->