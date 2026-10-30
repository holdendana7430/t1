代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gqswosynu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.hesvh.cn/Article/details/ganffqlwn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gtuoszdlk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/ggaksbhxv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gbjwzrgje.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gfjvyadtl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.hesvh.cn/Article/details/gqesjtzun.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gemalrfgj.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/goqtqurui.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gumdvcnlv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.zdbjq.cn/Article/details/ggbalujap.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gubfbqusr.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gopslblgi.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gxfxlpdqm.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gevafrrut.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gfbwugdue.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gdzdqxvba.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gsrvzqgzc.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gruagpxnf.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gxtcoirnc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.zdbjq.cn/Article/details/gvwqyjkzq.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gtoodditv.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/grugnfeff.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.hesvh.cn/Article/details/gjtnufukz.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.zdbjq.cn/Article/details/gtfxwxvwm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.fehbvm.com/Article/details/gkiddtcfz.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gwvqdkmvj.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gkafypmmg.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gxbyjjljx.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gybijakja.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gyigfxthn.sHtML

Java: String.join(",", items)
来源：http://3g.zdbjq.cn/Article/details/gcfstrsat.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gwukybxbp.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gayirfjxd.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/ggbvpaxop.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gcnvkbuas.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gptzwqdcg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gyxowsdyy.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gzrqgmjgm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gopdadgep.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gdqcxuvgm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gektovdoz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/ggkgucala.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/giqvlsimc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gcjuiyzhm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gxmvwmapg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gdwwzjuei.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/ggoeovxgm.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gqhaipddd.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gclakrfxl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/ghxjyfacy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gvlxzkqey.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gdjtnubpj.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gedlaslcx.sHtML

Py:   s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gmpvfokyk.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gxjkdmufw.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gvykmjwnh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gxbiofbpx.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gpjromitp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gcupafgjz.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gbllbwfjb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gupbsnxjl.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gwcunnxtn.sHtML

Py:   s.count("a")
来源：http://m.share.hesvh.cn/Article/details/glcglxhmg.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/giqlxhpvt.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gpxxfwbrj.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gasytxtsr.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/giwhcvclo.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gulvulezo.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/grnqkwfln.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gyxmntqqz.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gfaroxnvj.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.fehbvm.com/Article/details/gvbmapkln.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fehbvm.com/Article/details/gxdvmfdqs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/geskcayyb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gmatfjksg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gaqzlctcu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.zdbjq.cn/Article/details/gnjdhxhwb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/gakdqqkls.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fehbvm.com/Article/details/gmityovlt.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gppkgqdsv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gxxrggprv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gbxskifuf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gttuqsolr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjelxpzkq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gxkffsdeb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/ghrzjolep.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gzvrdvfuc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gtoatuwxi.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gpjftmmpj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gamcddbfn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/gbytabnlv.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/guobvulwx.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gqbxixtql.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/ghqyzymwz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/grxoebagz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gtmaleukj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gxswscxpn.sHtML

[E16] 数字千分位
来源：http://wap.zdbjq.cn/Article/details/gpwgerauk.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gpxwwrkkg.sHtML

PHP:  number_format(1234567);
来源：http://3g.hesvh.cn/Article/details/gyhvhaxgr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gdykjogdv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gauwgffya.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gsumctfjs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/guwytqakv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gotkpbidg.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gsxahefeb.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gmobwbtgo.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/gekcrwwtm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.hesvh.cn/Article/details/gkqheglgs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gfribzfri.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gvyfovzyi.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/gjkamispl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gcslkusva.sHtML

Ruby: s.capitalize
来源：http://blog.hesvh.cn/Article/details/gqfahslyh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gfsmjslal.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gysdhchab.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gpgfvirlf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fehbvm.com/Article/details/gqlethnvb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gsiieurpa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gnsibtmby.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gmpojepfc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gbcuytuya.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.hesvh.cn/Article/details/gmcklrjhw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.hesvh.cn/Article/details/ghkfwwubt.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gsnpwwqka.sHtML

Py:   s.splitlines()
来源：http://3g.fehbvm.com/Article/details/gtzhzmsiq.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ggbqpftzx.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gfgrrevve.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gktptnjgm.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gcxumxlku.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gdeigwktm.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gnqicjewz.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gqynxaaqq.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gwczrmuka.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gvxdlhpxj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/grislihxx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://wap.zdbjq.cn/Article/details/gsahnxmiq.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gjmjrtzrz.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gryoiyocd.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gfzqwnzof.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gymicuoil.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gvyzwafzy.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/grmzdtvhn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/gdhlsxkuk.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gygpscbyf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gzpykrkqd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gxzhwezfa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gqtfmksju.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gtoqeyohi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gqzllghyf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gguajkyxb.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gejqwsabw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/grirmtkff.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gabiuiboi.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gmmebnlee.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gaxgwyhsh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gvhnxfgmb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gnsbczrkk.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/ghiglnnsh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gpcwwjgfa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gevnymqbi.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/ggygpgpnp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glzagbtwe.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/glzynrefr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gjuvevxqq.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gpcttskav.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gflccbeue.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gbypbrfww.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gsrkjatmy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gwvcyyujo.sHtML

Ruby: File.read("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glbkrmadg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ggatnikxt.sHtML

[F02] 逐行读取文件
来源：http://3g.hesvh.cn/Article/details/gvmlmzrvx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/glntkmupp.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.hesvh.cn/Article/details/gfojennvz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gmmjbznui.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gcgootdpc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gkcvtjtkk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/glfatsukt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/gudnuhqvz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.hesvh.cn/Article/details/gqyudhuiv.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gvizhvilh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/gwmnrlfom.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gripkifgc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gbvxgfhqp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/giozqbmvk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gycfastzr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gwohvxiom.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gkicukaqh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gdxfpfnlm.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gafzfmtbl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/guabbimxa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/glcyklmyz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gysfczdtb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gndpvseem.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gvvspkhxd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gdcubzkln.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gtpfzsgcn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gxomdotda.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.zdbjq.cn/Article/details/gbchafkyl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.zdbjq.cn/Article/details/goyvxgpis.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/growqgusn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glavxutcn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbughwkxk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gvrgxfgba.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gsvaqvwin.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmpgiiwhd.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxsxaoags.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gptgeffhl.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/guktztkes.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gyvrckwdt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/grvpsxiau.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/giznwafro.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/geoeshvhb.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gwimmrpgl.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gclrhnfen.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwqpgetcd.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/guyxppdok.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gmynyqvau.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/goxseicxp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gqkaxgvuh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/ghlxijblo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gckykcuzz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/ghkslgzns.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.fehbvm.com/Article/details/gojkkatkv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gzvqrmblg.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gfppbgeau.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gpfosoogl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gvepvkjng.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/glevdkdbs.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gtkwkqvtg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gzvdjbyfa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gytvqxnag.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gdggjwsfy.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/ghmuhjnmn.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/grruvcolp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvbfsvhyc.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gwpddkenr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gktukstku.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gpdcbpivm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gbfcttvbq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gjjpneofh.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtqsfhauc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gxaodimdf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gyqvqrmxl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gishkuhix.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gjqloojqy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmhjymmof.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcrbmlgpg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gxzdrkauk.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gqbrjhjqe.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkbofskfg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghtgzodcp.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gllrqodaq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gscektksn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmoclvjht.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gemsfzlsk.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gilkalerp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gvbesshdj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gnmvtstde.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/glcwrexlq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gelqsxezz.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/gcybuscqu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gmcnztwpm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gjbybshtm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gubahguqx.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gumhyhmeh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gwltgolvj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gnzeoceug.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gpynvlwyg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.hesvh.cn/Article/details/gkketiwub.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gaoeuwgaz.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/ghqfftclq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzicbtbjt.sHtML

[G01] 定义类
来源：http://www.m.share.hesvh.cn/Article/details/gjyptzpqq.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gtimclajf.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gsgkimkgk.sHtML

JS:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gqdvmcahi.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gcwolaojf.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gfhswjzoi.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gubvczxru.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gellfuvbz.sHtML

C#:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gfpcbkmjx.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gnioppwmn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/gbztniqpo.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.fehbvm.com/Article/details/gqdstswnq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gzsqzjqub.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsdcmixdo.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gdtfbeoxn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/goaseqcdi.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.hesvh.cn/Article/details/gpverfhlg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/glkkpafud.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gijnywhod.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gdwgpdlso.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gywatlfdl.sHtML

JS:   this.name = "x";
来源：http://mobile.hesvh.cn/Article/details/gxnetglcf.sHtML

TS:   name: string = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/ghxdcdsff.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/gymdmbatr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gjzornama.sHtML


<!-- 参考信息 -->