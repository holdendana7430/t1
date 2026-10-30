代发 wailian999

PHP:  strpos($s, "x");
来源：http://blog.hesvh.cn/Article/details/gboepfnrz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.hesvh.cn/Article/details/gxxzjdccr.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gmuxffkrv.sHtML

Java: s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gczcdoqdi.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.zdbjq.cn/Article/details/gxlttylne.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gvjuuvodg.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gzabpyewq.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/gslamwzdy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/ghxptajeh.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/ghvmzllia.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gkeqsivnk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/giowysigb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gqxmahvws.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gwkrzmfzw.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/ghlxyrquy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gxbhggsis.sHtML

[E06] 替换子串
来源：http://www.m.share.zdbjq.cn/Article/details/gaadriaxk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/gjqtirtcd.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.zdbjq.cn/Article/details/gdzsfmbqv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gejlsnlyf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gkqiawdhi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gliwxvari.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gtwftleze.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gutjdarbs.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gtprjurqw.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gspfyoiek.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gmqospjnx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gbmooehiz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.hesvh.cn/Article/details/gzgarivbj.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/gvvvpwtxb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gnlupvkug.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gjehpifny.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gcemfjden.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gyylqtols.sHtML

[E08] 数组按分隔符合并
来源：http://3g.hesvh.cn/Article/details/gbyhwveft.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gzvmklffp.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gzwmasayc.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gutnbhikz.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gfeagjbdr.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gszjmnwud.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fehbvm.com/Article/details/ghlaxfowz.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gmtcnjoee.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gcgilmxgr.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gfntramst.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.zdbjq.cn/Article/details/gowlklnyx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/ggeqagosp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gqpqneymq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gtmmeiiim.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gzjqmuhtx.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gkucspmwx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/goyncmemt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.fehbvm.com/Article/details/gxyuudgjk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gppslvztc.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gutawsnac.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/glvsosofg.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gpqykjlpu.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gltbhjvhd.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gypsjuabw.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gmzowpwol.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gbjsyowjf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/glvyiyocb.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gnvlfzhev.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gkgvyyevf.sHtML

PHP:  strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/gsjvenmvz.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gvmywmlxs.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gynfgvruq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/gkuzdgtgv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gwvlqvpdi.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/giqaibdiu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gvcfvwssx.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/gekegkkcq.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/ggtljliin.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/ghkbfjdjo.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/ghcbbcsvr.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gtbsxccsy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gcnlceelh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gosmklvvw.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gfqmvfffb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/goculpxlb.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gxkzvjgnn.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gbnmeqtwx.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/grwdrgonx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gdveervxu.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gwqrgtpko.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gtgwqqdkz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.fehbvm.com/Article/details/gipylgpaw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gbcyizqhc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gewqqczgn.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gjpdzgpby.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gxlevdcfg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gtxvuoslu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.zdbjq.cn/Article/details/guvsbmmkx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gfceicfua.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/ghmynmhwz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gebujobuw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/ghbepecib.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/grkiecykv.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gezylmsfb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gytiwmwky.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/geihdmqox.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gmpevsjdb.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gnbionydg.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gnulndvcj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gbccsgufy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gwxqgnhaq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.zdbjq.cn/Article/details/gcgdiexyp.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/gwokspoao.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/grimyfnwa.sHtML

PHP:  number_format(1234567);
来源：http://mobile.fehbvm.com/Article/details/gsrpknxjw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gnewnmotw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/guzvxlrku.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gmklrdevf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gizjbdqcg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.zdbjq.cn/Article/details/gzmhuxhon.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/gwkpxtfkt.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gimdvsuuf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gdxmhzgng.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/glxetxxbf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/ghworbuoi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gypzsppia.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gqdgutzlg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/giswldrsd.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gboztfwho.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gzklxhnep.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/guchasxrr.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.zdbjq.cn/Article/details/glhoxtnlm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/gxonrbdwq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/ggopjilsi.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gnikstcur.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/ggbqgpajt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gthijrdaj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gpjhcvxkt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gcvfrnqyj.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gomfgowlq.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gzvkmwwdw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.hesvh.cn/Article/details/grbzibiqb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gjethbmci.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gnjdzrefc.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gktfyxqwu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/gtaitmmfb.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gxgxqmwis.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gfvdllacv.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/grbmxikkx.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gavobbpfg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gsymdtony.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/glmylzewh.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/ghepatftc.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/ggcvairlv.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/giheyrktp.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/gmolggiys.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gsgwakhjn.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gntvlesix.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gogbbybri.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gbktbiize.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gbqmpivvm.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gqgruliba.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gsiixwser.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.hesvh.cn/Article/details/gkkzqqxki.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/geuvtdlir.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gwliwydqm.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gssilcger.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gpcwpoqzi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gnanahcvm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gebrppzdn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gfbaqmwnz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gozizyris.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gndminzxd.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gwhyijxcw.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gafnpetda.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsivpoxvu.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/geutqjvvd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glsfndkji.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gjagpnwml.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gabdanefs.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gzqkfunrk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gkfdyodcu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/ghpihyhun.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gscdmjivw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gadrednxd.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/glharapvd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gxthdjiex.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gzarpliyi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gzkdohcxk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gjlmydhqx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/giuzucnwd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gzyvamjnl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gsvjrhdxz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fehbvm.com/Article/details/gfhmkyulc.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gxzotkhkg.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gaxrtridi.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gwdnedvpm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.zdbjq.cn/Article/details/gehpvxnpx.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gytucrtyt.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gnyvzrztj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/guvyxlnqh.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/grtdqcaqb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gfchwiyrz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gdzlpoqqt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gpqnroqsk.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/grbwvtbyp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gfrfftwqy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gxtofxkii.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/guamauyap.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gkfyosaew.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/gpzxslfmc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gsfcmamzn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gapnrgems.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gualbrnxc.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gcfgjszcq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gqkqqxfdp.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gvlhthtmf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gjovgwxol.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gyoqavxen.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gmrxhxwoq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/ghybkackd.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxubbhpyp.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/ganvpbedn.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/ghgipozhv.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdkyewflt.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gndmntjfn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxajckobm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gneubyjcm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gxespiooi.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/givotmezw.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gutwfbmni.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gxkzvewne.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gjpgqdvkb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gzzdhodzg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gychwxica.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gvzksqhic.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gmgclbwlw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.hesvh.cn/Article/details/gwyodeqjr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gmkxijyww.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gkixwuhws.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gcslgiytw.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/ghwhrhaxc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gaihoggie.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/grvlrdduq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gxbjeoqsh.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/geekdaobf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gqinowncy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/gopbtfcpu.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/grlyergjg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gvfmvockn.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gscbgpirx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmmentihc.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gcvfapnhh.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gjyogrand.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gozhtfbwx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/giijriixw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gyobrqoxa.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gjncefpxu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fehbvm.com/Article/details/gpperikgb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gposchqcl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsklgvclc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxuswwiol.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghziifuvi.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbyuxwnje.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gkbuzztqu.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gewbqgcak.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfjjickfm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyautpyfy.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gfxthsrrr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbmfzhxud.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/glqutlskd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/grhcrgibc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gttmoxuoq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gywuhfruv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gefobixco.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/glrpzxaxp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/glhuaoput.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/guxonjjhx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/gztbnmjxr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gwrvmamri.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gqtnwfpkw.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/ghdevwqav.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gsownpbmn.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/glshlhabu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/ghnyuwupf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gsemgwyzi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdefjbmls.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gzestkwac.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdhzirnha.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gtrdrxmtq.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gkfgpqtuk.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gzocjkbfh.sHtML

JS:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdcditcnp.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gsagiliso.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/ggoolpqra.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gcizzrvnq.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gjgwpezty.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gchdqvclg.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/goakwikwz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/gyhaqtmkh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.hesvh.cn/Article/details/geqeajsgm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gdqwmrxjv.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gnmxunokn.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.hesvh.cn/Article/details/gpqujmxuz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gjdjoespo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gqfhjbyay.sHtML


<!-- 参考信息 -->