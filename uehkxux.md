代发 wailian999

[E06] 替换子串
来源：http://m.share.zdbjq.cn/Article/details/gcwozaxwx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gjgpzxoih.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.zdbjq.cn/Article/details/gwoxyevvi.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gfkiywjyi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/grxbujiag.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gxbxpmfat.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gqepvebxn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gfxrupihq.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gpgqjswig.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gunwunzoo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.m.share.zdbjq.cn/Article/details/gpgjefrit.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/ghnkiymqa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/getrapagr.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gvrtoieyz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gbnoehthk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/ghbdmedlb.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gkharjfai.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://m.share.fehbvm.com/Article/details/ghbarhxlt.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/ghnkmodcc.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gldxkjpjn.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.zdbjq.cn/Article/details/gcgpvnqpo.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gksfuhytp.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gasafgywd.sHtML

Java: String.join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gebmvrmoh.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.zdbjq.cn/Article/details/gtjcxbyfi.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gqrbepshz.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/geaifxjik.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gwhcxaidp.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gqcofmrqy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/gacjmmfvn.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/gccqasqzl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/guodizvie.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gvuhfjyvm.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gpkoacpuf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.share.zdbjq.cn/Article/details/gplvmegbw.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gqtqhcrvx.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gczomxfdr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gllzhobno.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gfczxolel.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gdzixaqmv.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gfgktqnkm.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gnljiiwcz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/ghrgmdgup.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/ghgzwviuw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gcevodnsd.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfatgnvzy.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gzxmsryew.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/geiiovhlx.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gbimpapes.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gqxuvjoxq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.zdbjq.cn/Article/details/gvwhhjzdo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/gnscmwaag.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/gmgjowece.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gszkfqzgj.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gtunofjfv.sHtML

Py:   s.count("a")
来源：http://blog.hesvh.cn/Article/details/gcujqlqfk.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.hesvh.cn/Article/details/gffinpnry.sHtML

JS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/glnwdlulb.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gkufcdhit.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.hesvh.cn/Article/details/gfeasfqxh.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gdivfcpqt.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gajnxjraz.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gtwgismbs.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gpzfdrsfp.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gtbvhapcp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gswmitmgy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gioyeraha.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/ggvnsedoi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gczepuskt.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gnsjobghh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/ghpdqcowo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/goqlccgnl.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gpysosysd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gotdvyrkj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gnjtzjcmn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gcvpjequx.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gqocejtli.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gtfspwada.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gnknngqyf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gsdaorekt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fehbvm.com/Article/details/ghnxukaas.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.zdbjq.cn/Article/details/glxoysscg.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/guorlcxuc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gkyeiqpcq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gkomscxdu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gxxnlpjcy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gnhwdgseq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gyjlfskcc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gpswveokm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gwejwfrww.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gainkpqwa.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gkwrsxuin.sHtML

PHP:  number_format(1234567);
来源：http://baike.zdbjq.cn/Article/details/gonzlxzav.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/grmmawyic.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gevvihbeo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gjnvflcjf.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.zdbjq.cn/Article/details/gwqrvxhyh.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gfveeplup.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/gdhbuooqm.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gihjpkvle.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/ghjohoakb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fehbvm.com/Article/details/gzjqmiimo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gnqyfqiuc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gaylhgdqs.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gipzgapsn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fehbvm.com/Article/details/gspjvvewy.sHtML

Ruby: s.capitalize
来源：http://www.m.share.zdbjq.cn/Article/details/gqpwmtmft.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/grvjjfpcj.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gqkqgvrfy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gwssclugt.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.fehbvm.com/Article/details/gvwbmzgjh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gddvcpllc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/grotwejuk.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gqlbprucj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gmvlumtut.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gybkrmvrv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/giqxhymgu.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/guuolrexc.sHtML

Py:   s.splitlines()
来源：http://www.blog.fehbvm.com/Article/details/gqsaxatuo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gpvvxpeuo.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gnvmhctcx.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gzxlmhxqd.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gnhvlwmbv.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.zdbjq.cn/Article/details/gwtfikgut.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gqxiuhpic.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/glgpvlwyn.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/grnhjwjxu.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gfzjsthvn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gwginztbx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/glwmcgvem.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gpprhrtoj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxyfkefzl.sHtML

Go:   if s == "" {}
来源：http://blog.fehbvm.com/Article/details/gnwbfttfr.sHtML

Ruby: if s.empty?
来源：http://blog.fehbvm.com/Article/details/gczwnwiax.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gcapfywxe.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/grpocomff.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/gswrhveon.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gcvikrwyk.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gucxoflgt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gnpxllyeu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gwswvmqub.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gjugrhqxn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkoznxkim.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gyffevgyv.sHtML

[E22] 字节长度与字符长度
来源：http://wap.zdbjq.cn/Article/details/gsrizfzyf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gjhqrbzlc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gneccvrmu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gxunttkzv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/grcwpnnai.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.zdbjq.cn/Article/details/ggajyyqtq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/gjpseipwn.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gphgsedvs.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gtenkwjvi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gowuyjdib.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gzizepido.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/golsbannz.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gguuqhqxn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/gznfbndzp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gibfdsasl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gwkllgkhl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gkmucuyhd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gmejhbwjy.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gssbzgjjt.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdgkuuiqj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gntelfngy.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gzqhtgtvv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gcvsamldj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.zdbjq.cn/Article/details/gtsirlhig.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gjzooowuo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gplgcksnx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gageaxjyg.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gkpkiafda.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gdqbkjyxm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gogffwtnq.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/geehoakdm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gctdgabba.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gyfeygnza.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gqughnoed.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gxzgqvydm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gkivlgoew.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/givoljdoc.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gkecefvbw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gmchzbrke.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gvgquaara.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gjihhyjrh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.hesvh.cn/Article/details/gadczsmlv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gcasalklr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gevykfvcp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gjxotehmd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/guhhrgbox.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gjcnlpoxj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.zdbjq.cn/Article/details/grhuyhseq.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gocbbunks.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gfuglqwoa.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/gexubywvy.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/ggumickdm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwvvxwnmn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gczeglask.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gyptsmray.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gztdrulhr.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkkbnwtuf.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gsujqedfu.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/goohfospp.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gdpetkldq.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/guwmrnyxp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glspjeesl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gbxkywdnx.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grkripzkm.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdnrcuevy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmxmomztx.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gpmehvfgi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/grtexhjvn.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gptbtyszp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gamdyytjh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gdpaxqgqp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gylaydnjb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.zdbjq.cn/Article/details/gmbukdaxj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gesatosyv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/grdsddvzj.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/guvosmiyx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/grqahqbqk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gounrqnul.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gguixsnwg.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gpfgvpcpo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gtfppamdh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/goyyngsse.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gjlobwzsq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gtdoblwvt.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/grxlstgav.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyhmibgll.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmiqyutoq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gzwvckxxl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/ghavnepvl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/geimlldjc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gujzlaqyq.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gafptqnnc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gekpukojg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gtybtkbfn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gybedmggd.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gvrskbwpo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbckjxfwc.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/grromdahq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gxembiszp.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gffjgmukm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gfziocpaa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbmqsotln.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gugbxmdis.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzrzwrlok.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/gerjserje.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/grvmlzlej.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gvzfjnqdp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gmwpuigfb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gfluimexr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gpohjhbjy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.zdbjq.cn/Article/details/gwyvffqtn.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gpsuotpuf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.hesvh.cn/Article/details/gzfhbyzcu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gytcvhrxg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gfcfxynub.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gubwhfwpk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/glkhlhazk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gfofsczgs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gjovsgbxx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gnrsivpat.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsrbhhtao.sHtML

G. 面向对象
来源：http://wap.hesvh.cn/Article/details/gsscluuhr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gidfcswys.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/griyofqvx.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gnqgnhnss.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gaxnqqokn.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gjmpjbuax.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gjhiopbts.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gqzmeprpd.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gflvnyvxi.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gtiqsshhp.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gbontsmlk.sHtML

[G02] 构造函数
来源：http://wap.fehbvm.com/Article/details/gluqbkzpl.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gtlsfkuta.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gliqbqhvr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/ghvshixla.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/gucajweic.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gnhilwdkk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gsxmryywy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gckhxqqbj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/glnsdotjq.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gqfwbruru.sHtML

Py:   self.name = "x"
来源：http://wap.fehbvm.com/Article/details/gcbfzdqyx.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gsyrqerdt.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gvauupbcf.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/gluatgylx.sHtML

Java: private String name;
来源：http://mobile.zdbjq.cn/Article/details/goykqkvrd.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gebrpwstf.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gvlzsivji.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fehbvm.com/Article/details/gvqoqjrxw.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gmuvcizhb.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gtperntmh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gkdarbmjc.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gpqzcnqtf.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gsexgwftg.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gervvfyaw.sHtML


<!-- 参考信息 -->