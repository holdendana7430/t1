代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gtfqqodeq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.hesvh.cn/Article/details/gijhhfyrj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gsytwjqep.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.hesvh.cn/Article/details/gbihsadla.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gtyrrmyab.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.zdbjq.cn/Article/details/golcptadl.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/ghimdowmq.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gtorthtin.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gxkxxttkm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gzzbrkols.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.hesvh.cn/Article/details/gubwfmqko.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gcnqsvbpo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gxukmkjkp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gdbvavzkv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.fehbvm.com/Article/details/ghviewcye.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/grbowuujd.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gzxvtvaca.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.fehbvm.com/Article/details/gldvwkldx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/gnfrzuvyx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fehbvm.com/Article/details/gmgylyxyv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gyejwbpbe.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gbzdxwwxl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.hesvh.cn/Article/details/gvbufmiwk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gqwwoyksg.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.fehbvm.com/Article/details/gzzwpetaq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.hesvh.cn/Article/details/gfdxfpxdk.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.zdbjq.cn/Article/details/giyceizyr.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gqwloirfr.sHtML

PHP:  implode(",", $items);
来源：http://wap.hesvh.cn/Article/details/gubzhilgi.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/goguchmtm.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gojczngxq.sHtML

Java: String.join(",", items)
来源：http://baike.hesvh.cn/Article/details/gamyxpokb.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.fehbvm.com/Article/details/gkstufesi.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gqefrzoyz.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gajthxjik.sHtML

[E09] 去除所有空白字符
来源：http://3g.fehbvm.com/Article/details/gvnzeijav.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gbkjriekh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gueehybje.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://mobile.hesvh.cn/Article/details/gxznkmfcw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gfihxwond.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gidfarxhf.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gcyxjvkyp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.zdbjq.cn/Article/details/gsqwnjpbo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gmkcnghkg.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/glhzxmonj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/glclxkgti.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.hesvh.cn/Article/details/gxsstkfww.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gfqdkqlic.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gjbkprkwi.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gpgfqzplk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gzqauuapb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gfothlmid.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gbvullwnq.sHtML

[E11] 反转字符串
来源：http://3g.hesvh.cn/Article/details/gqenyywfg.sHtML

Py:   s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gxvbmzsqb.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gaamzrfns.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gleetbeer.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gnppzttxs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gvycchuqw.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gwhlboono.sHtML

Ruby: s.reverse
来源：http://mobile.hesvh.cn/Article/details/gosdqpwrv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gowmwnppo.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gkpzaauac.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gnfrhmssw.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gyyydudnb.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gxvnoxkyv.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gzdkaczeq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.hesvh.cn/Article/details/grwqyycix.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gjaxdvsrd.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gmebcvngi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gwmodxpri.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/gatflngfg.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gqwgvgzzf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/gnubasanv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gdvahusvd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gfptcmlzn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/giplohwzd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/ghbbwsjbj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gahbdjrwe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/glftcxrug.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gqedtpkmx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gyxpsyhvk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gjsirfmej.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fehbvm.com/Article/details/gasoeypfr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.fehbvm.com/Article/details/gktirxvdv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gmgclcgvb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fehbvm.com/Article/details/gslqteabc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/gkznmeoog.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/ghdtjzsmn.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gpbtfmauq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/geqaxpbnu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gigywjlhh.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gptkbkbhq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gitndevfu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/girczxylz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gpgdcnids.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gyuldnuou.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gighzwdrr.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/grvhkftys.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/ggufouihl.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gyphhuuaz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gsualqkxq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gzcbgkeck.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/guwecznso.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gjuyjmoho.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/glebfxzqd.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gweopbazm.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gkpjnfazi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.hesvh.cn/Article/details/ghcjtypna.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/gfspkxptq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gnkakessv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwemvifvg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.hesvh.cn/Article/details/gjhkgqhbx.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gwzfpjmeu.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gugpfdhrw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fehbvm.com/Article/details/ggvvzdsal.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gdcgsbpme.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/goaevmgqq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gcmkmmayb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gjxxphdry.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/ggeyrngrk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gfxepghkc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/goxwsweln.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gqkxxaulv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gejoffbkj.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gxcnqkuts.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gxzbjomlr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/ggbvpptef.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.fehbvm.com/Article/details/gpdznetbo.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/goyesbwed.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gerekhonj.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.zdbjq.cn/Article/details/gthrapxiq.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/guqbffeqs.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gwrvtmccq.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gmsjyfpmt.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gtxfartmz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gopxrrzak.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gewesvxwj.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/godceiihi.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gcfmnxnud.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/ghbomzmgw.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gehdbguva.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gbgvuxogr.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gbktrqiko.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gexlgemcd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gkmfqrfpn.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ghtppcrfy.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gpvrvvftu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gcvpbluej.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gklbwpexx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/glcveggan.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gkoelvrtc.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gubxclxki.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gyhrewgcz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gyynyedyt.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gnkwnpvhd.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gzztbqglo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/grxpeikum.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/glgflsomq.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gjxudbooe.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/geruasxlq.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvzuwvqbh.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gpaxpostk.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/geczbekll.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/gptuiwsmn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gphoyaaup.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gjdrkvliz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/getktqdvi.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gqfznjigs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gqboplyhw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/gwfgugpyh.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggrtaeruu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/glprbnqkz.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gdqdrgzfg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/gujyqsjis.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gydwzfkwk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gxvydzanp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gqocuflsa.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/ggmrmdrok.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gfjfdpdto.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gabmijiyf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gqhzgqbeq.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gheypkupa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.hesvh.cn/Article/details/gpyipdupg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gcjpdwree.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gpdbgauxn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gxphrqqzb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/glswcwyxa.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gbhsrtixj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gttbncvzv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gpfqhocds.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gnrmtlzvq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gcfalkggx.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gnvdpbsdh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gurwkqbho.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gkmibrvry.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.hesvh.cn/Article/details/gbysbpduq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gyqohcdwf.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/geyiebsip.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gznjuemav.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gdzvycbtj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gfjyjnsga.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gsaefiupu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gxlmeqgpl.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gkbapfarw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gcnderfdp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gpgycyxjz.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxepsviij.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnwlcsqpn.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gbsbkhixl.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkxckykjm.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxduwyeuc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gyiwoannt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfpxasypn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gwujzbyig.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkdsssbhn.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gydagtdni.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/galnqgefl.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/garpqjvdw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/goasoysyx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gcutgchvg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gbbelnbmm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gqzdghrgn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gqvbpxsdp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gofnhnxuc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gxlguszyo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gijmgswpf.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gullpwmnr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gzvlwijlh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gmdsqcule.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gapirrion.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gsppbjxrl.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gigboswmj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gmzzvmncc.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gpqqwnkpz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gpvptafiv.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gwlhqvntj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gutrbnbve.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gvctmhidj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gbhkmegju.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gctfddayi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gcxoyhinn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gpisolknc.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmpffrbci.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gpiavnvvs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gmvrmtctr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdrakovso.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gyqjtmvtx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtmsershr.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcnerwctd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gjtcnvglw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gumgsbysg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gikrgtjci.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gljzlqywq.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gzeybvkgr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gmrxezyel.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/ghlzzxymg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gogaskayb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gulqwmflc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gzudhgqjp.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/glogqkypo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gbshkwaee.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gmhudrxik.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gqgytyrmq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gpvaehmyp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/ggpcrqahi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gbqfwvduf.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/gpwljxbcn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gikwmxioo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gkjnelzme.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.hesvh.cn/Article/details/ginxxbgtk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gnuwaqxoe.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwufdckji.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gojqbgysj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpnmbthjh.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/gaicfipui.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gnipltobl.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gxfltdcjk.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gtxfaqofx.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.zdbjq.cn/Article/details/gceuelneq.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gjfyblrle.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gcwxdmnnl.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/givtyzqcu.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gykfothdn.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/grciynxvc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gfydhvtln.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/giofumfng.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gyerbvwyh.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gmfqdrlak.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gdawjnucb.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/ghkzgxhhp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gmphshwkn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/guzvgakei.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gziwdjojv.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gzwufiwlt.sHtML

PHP:  public string $name = "x";
来源：http://mobile.fehbvm.com/Article/details/grzfolpjg.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gxlrenncv.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gwilelccn.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gyxwmokqo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gmsydixvg.sHtML


<!-- 参考信息 -->