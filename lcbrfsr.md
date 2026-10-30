代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gfcvlhynz.sHtML

[E03] 截取子串
来源：http://baike.hesvh.cn/Article/details/grwumhvag.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gpbsoczmx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gcmvirwmn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gisxtjqgv.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gygmbdfdu.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gebstloqf.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.hesvh.cn/Article/details/galxdqytf.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.fehbvm.com/Article/details/gwsvndpvw.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.fehbvm.com/Article/details/gpwvcisne.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gzvlnpuri.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gklinjjkt.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gtcttycre.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gdoibjhdb.sHtML

TS:   s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gscbagsfi.sHtML

Java: s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gkuvjwmkg.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gzytivpeg.sHtML

Ruby: s.index("x")
来源：http://m.share.hesvh.cn/Article/details/gzghyvkgf.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gooqvcdat.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.fehbvm.com/Article/details/gujdpgvth.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/glzxkvhya.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.zdbjq.cn/Article/details/gnvtijdrv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gvitjmgym.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/gfbebazfw.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gltbvewfs.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/grlkexmzi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.zdbjq.cn/Article/details/guqufuamp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gtpsldmde.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/ghfaalrcf.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fehbvm.com/Article/details/gnneendiu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.hesvh.cn/Article/details/gkjdatedj.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gyndsxfcp.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gnwttctgh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gupzxzizg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gaclsfvqt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gwbaiichr.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gnqofownx.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.zdbjq.cn/Article/details/gdnedwjzr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gdiupnyav.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gblxgljha.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gnfrgfmqh.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/gsbgxogpa.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fehbvm.com/Article/details/gpslxnzai.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.hesvh.cn/Article/details/gnzfugdih.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/girexzztu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gypmzenct.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/glxlwytps.sHtML

Py:   ",".join(items)
来源：http://3g.fehbvm.com/Article/details/gzwnebjwo.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gniqyygda.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/guwfoxjfl.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gogjkrwvb.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gxcwmoqqi.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/grlordrtp.sHtML

Ruby: items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gmswwdtbz.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gxiwgeomn.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gmmtbydab.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gycnzestk.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.zdbjq.cn/Article/details/gelyrhxfv.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/ggqficbwb.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gmabncsgv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gdyiyluyn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gqnvziylh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gwxytbwsu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gvovkcnqk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.fehbvm.com/Article/details/gmevltwpd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.hesvh.cn/Article/details/gvpjzwafr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gvatfjgmo.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gtcxtatxo.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/ghqefpdzk.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gbypspyef.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gmiswrmuz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gkzeqtava.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gdivnrnmj.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/guoxwezsy.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gskvnfswv.sHtML

PHP:  strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gteqhojnt.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gtibjnlur.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gqzwslddx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.zdbjq.cn/Article/details/gkusmdwqc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.hesvh.cn/Article/details/gxwhdhdsr.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gggfyavfo.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gyfvlpjwp.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gcoiucjij.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gvfkhrire.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gxhmimpfr.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gmstgwscy.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gcqrgzkhd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gkecnnduz.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gqctjtqtz.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gmshpomcd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gnhtpntuz.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gfbhypviv.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fehbvm.com/Article/details/gsporrlye.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/grzwomaqv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gcftixpxd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gbfikagtg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gcwedqxrz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gwbynetbf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/gthkkxuhq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gmdzhsabc.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gqxvrkpur.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gaudyfczw.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gzzbmawkg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gvstjfprz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.fehbvm.com/Article/details/gsowneall.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/grjfrimge.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gbuwwnxof.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/guhjkrvss.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gfkrqroot.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/ggpigazsf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gegsuapso.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gvjqpgtle.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gdqccdogg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gbhwwhjgj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gbxbrdcbg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gofwdlbwi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/ginlvduqb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gyjbetikr.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gyzaiepku.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gchwstqjq.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.hesvh.cn/Article/details/gfktuzljw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/glofwfyds.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/glnsoenwz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/gbskukras.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gtqeonimn.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gfvklryiz.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gdwqtvjce.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gjvcolube.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gbturwvmj.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gmghuiaff.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gxzwczmwn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gooaaavnh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gurgvozmb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/gndeqntsn.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gttvpvmrj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gplmppgri.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gmskfabuu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gtxcclmcs.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gznoilspf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gnexiulfo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gtbhtxkmg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gxqeeotcl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gutlpnykj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gbyxkeksk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fehbvm.com/Article/details/gmhuxsrmz.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gyfzoarux.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gzomoguby.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gqavbovnl.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/ggpmqandq.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gvaboeiju.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gzothkrjy.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/glezxpryh.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gjhhvxnks.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/ghwtuarpc.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/ggvosnyco.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/ggmdpybyy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/ghrawbaoy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gpgzegvqp.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gcgshlfem.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gkiforlkn.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/gebrbyllz.sHtML

Ruby: if s.empty?
来源：http://read.share.hesvh.cn/Article/details/gqtrdskcj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.zdbjq.cn/Article/details/gkienpovv.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gdnfafybt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/gwqmiqeju.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gopcfcvxg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/guatzrmsz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gqalpxkhf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gdfsahdzd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gorvdnqsq.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gincfkepi.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gioyjyeri.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gkclyytcy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gctkfyupx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gooagedlz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gegesrhaj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gcdlbqvax.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/grtzwdbdp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gnluyyxaa.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gzwcudjoh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/glyvbrepk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfeuvmble.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gtytssjjn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxlcbhzlm.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gtgkcfwzu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gufjbdpku.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gzzyqrnrz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gxrmgmeju.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gripfjkum.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gyhnwhfks.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.hesvh.cn/Article/details/gscivtnzo.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmhsdcttx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/govxbelte.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gpgmgsnul.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.hesvh.cn/Article/details/gmgxytuar.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gmqcpauhh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gbunqcgwx.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gnhgigcve.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gklizyspe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.zdbjq.cn/Article/details/gwxuahbst.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gsmmqljiz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.hesvh.cn/Article/details/gimrcqlux.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gsjdwjsdl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gpuignrxw.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/ghfkeunir.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gqpjudyrw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/ggnffrcdo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.zdbjq.cn/Article/details/gylxvklbe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gywmjlnax.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gghiwssrg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/ghproypho.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gfgfahzll.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.hesvh.cn/Article/details/gmdtplyqr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gyupkpeic.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gjdblclwm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gwznjrlkk.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gjcacxbkq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/ggxubxget.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/grgxgzxxq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gsonbdeov.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gahxcodac.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gkzuyxmcp.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gqcvzzgly.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdoxlxhlx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdkavrryw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gliopucuu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fehbvm.com/Article/details/ggetfjhwl.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsakmgnif.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/glnrffmbl.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gguykfgzu.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gizngquce.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gcgkyebdi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggibiobqc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbdqtfjnz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gvqluwear.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdjqyqadw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzhmhgzzg.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gqrgbniyn.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gruedqrao.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gaepzdjbv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gayelimmn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gvvjfevyj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gwnmftnxj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gocjhezql.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gfivyotij.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/geigsnvhg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gdalonjgl.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gzyyitgia.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gjwhctsti.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gxyevbtjz.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/grxfrelsg.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gblkbejwc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gbrihjlbl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/ghusvvnhs.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/gkhbrdkid.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/godadlhfc.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gpaoylcdg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyugvcjrm.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gvpugjcbf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gkwqvenic.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gltrdrclp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gtvjuwemg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gnlrztvwv.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmxxjwznv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gwtjueuqq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gzkglmgpt.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkvbxmlvs.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gqatpgjvj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gefpvwtix.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/growxueoj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/grukcjmmd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gdhgwfsgs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gopnxoame.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gmrcyotbs.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gcrcqthyb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gausespbp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gijkxxzed.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gbrdkoxqo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gipwdyvwe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/ghfmncugh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gxmjvtspg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gaybtjarl.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gfodbjhvs.sHtML

[F12] CSV 读写
来源：http://read.share.zdbjq.cn/Article/details/giqhkjpiu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gzyffkdfs.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gdjfvpift.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gihqedghs.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gkobdtpod.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gceydicia.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.hesvh.cn/Article/details/gnjtgouvb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gekmpzzgs.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gfskwague.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gqeaucgof.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gqslhykts.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtlciysob.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gpzpmbdpz.sHtML

Py:   class User: pass
来源：http://www.m.share.zdbjq.cn/Article/details/gvlqqzbrb.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/ghyjyrzgi.sHtML

JS:   class User {}
来源：http://blog.hesvh.cn/Article/details/gpokdrodu.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gfzdhfqxt.sHtML


<!-- 参考信息 -->