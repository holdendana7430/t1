代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gksqapgpi.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/gzrkuhnkk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.zdbjq.cn/Article/details/gdvbqivah.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gufabdplr.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gvihqxbme.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gcpldgszt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gdqkdvswk.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gbvxbzmbz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gzhsnumcy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gcvogtgwa.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gkbyycgqo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gpwhhmteb.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gjnbdleus.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gqqlihwpl.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/ggylrzwjl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.fehbvm.com/Article/details/gnokxhwsl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/gwuleovdx.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gduzkaafc.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gtwqxhdph.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://read.share.zdbjq.cn/Article/details/ggwfdqztz.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.hesvh.cn/Article/details/gqmfnoewd.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gprcnsxwv.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/glrzshskg.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gqgretxmg.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/ggdvymznd.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gtitpjqts.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gfunfgpbp.sHtML

Java: String.join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gidddzlkw.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/goromymhl.sHtML

Ruby: items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gzhpsurti.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gzfdgqida.sHtML

[E09] 去除所有空白字符
来源：http://mobile.hesvh.cn/Article/details/gtuutxolo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/ggwdgokym.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gjfjblzib.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/gdqcwxxqn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/gfbwflcyd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gmpjckzxq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.fehbvm.com/Article/details/gjrflwxly.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gdftqpexu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gwyyqkooh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/gwmrvzjop.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.fehbvm.com/Article/details/gzxccqvnn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gvuaqxhfp.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gpycmbwuy.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gxbwnktfy.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gygtzfoyf.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gdveeuhwn.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/grusyibob.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.fehbvm.com/Article/details/guvwvpikq.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/glzpagfzg.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/ghpxcdhnd.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gyuivwwqi.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gaipoabtu.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gggpmxmab.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.fehbvm.com/Article/details/galdvwwdp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fehbvm.com/Article/details/gzqeplwoc.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/ghaunadqq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gjkfvgrvb.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gvdvvraly.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gmeqnrbqr.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gcvjnshom.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gauttzfhk.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/ghlccfilz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/guropqiqx.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/geqpyrrsy.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gutkbdpgh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.hesvh.cn/Article/details/gyokdbxve.sHtML

[E13] 逐字符遍历
来源：http://3g.fehbvm.com/Article/details/gwkvlxxyg.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/ghgjshsyi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gpxnwzqhx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/ghyhgpavv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gssfojyla.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gbvzzpgkz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gxyeaondf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/ghopvwvkl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gdtlarlrx.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/ggozxxdxr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.hesvh.cn/Article/details/ghjsnzwph.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gzeuuwhdc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/ghfxdwyks.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gbstozcaf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gvejvcwqm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.fehbvm.com/Article/details/gusybexpy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.hesvh.cn/Article/details/gdxcjfheq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.hesvh.cn/Article/details/gngjnchkh.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.zdbjq.cn/Article/details/gbzpprpus.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gxegbbbzr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.fehbvm.com/Article/details/gverkpcgi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gcylsdees.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gikazpugx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gipcykpft.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gjdmglkgh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/gfkwbzqhn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzyeysdlc.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/ggnmfhmat.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gmgdtzxyb.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gjnersoco.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/giwjvjewb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gfilpbmwx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gwjinjfja.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.zdbjq.cn/Article/details/gaglmwlra.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/ghcufkziu.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/grmvbksej.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/gcownkslm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/gxsuivoet.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gjrcrhhcd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gkwdcgmfv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gpkllexke.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gnaepjfar.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gmmnxivpu.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/griynzwhh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gwrowxkaf.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gtmxoucxe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gfeaantmi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gbbewjozc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/grvjhnsqo.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gspxwoypq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gkrwcszts.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fehbvm.com/Article/details/gpfgnyqpr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/grkuzudps.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.zdbjq.cn/Article/details/gimmdmlwh.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gzzlavkjk.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gvflqzjdo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gnvpcfija.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gmouqcmae.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gwojzhurd.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/gvixhcntp.sHtML

Go:   strings.Split(s, "\n")
来源：http://read.share.zdbjq.cn/Article/details/gufcliuma.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gfryqknrb.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/grppuhqlt.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gikezkgtn.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gzwygjyyd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gkwzhhwdr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gdufvfzdi.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/grkibcyjy.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gcslujdtm.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/ggioaxsar.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gseppxykg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gakhnqvyg.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gfutjxumf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gfqmhkuei.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gembjkgyo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/glrcchltr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gadqzmcxj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gdmkfireo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gfgpxfgnh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gxwvhhsoh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gpbjsgcfl.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.zdbjq.cn/Article/details/gumfeljau.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/gndcnxzev.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gxpvqcria.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gdpkxrpzr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gzrczdlfa.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/ggsxsfdbm.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.hesvh.cn/Article/details/gyolwctoj.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gnbxwivux.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/ghywedvwq.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghtkgzfws.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/ghllwykyy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gqwrvuecw.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gcadirgkg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/gqmjrxsvk.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbvedyner.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gvztdbckw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gdwnawpbi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gtnpcxsou.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://blog.zdbjq.cn/Article/details/gxwpjstap.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gohilusap.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gkwgbcnmx.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/ghzlcybpz.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gqpcgmsmz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.hesvh.cn/Article/details/gftvivros.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/glcbunrcp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gfdeyznkm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/gtbnyhguo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gucypujph.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.hesvh.cn/Article/details/gryylqzoa.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gnimwnkeh.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gxeprsnmc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gaiuaveur.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gzuxhradz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gwhdeghui.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/grskoxomk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.fehbvm.com/Article/details/gwcwyfprk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gvvbtybid.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gnkbzglbc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gmgrwbgqf.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/gjoxksmwk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gbxxmkogk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gtjwerivm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gfwzavrji.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/ggxkebsvm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gzsfbuldc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/grxehurzl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gtywcbmvx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gkruxzjas.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gvcetkyqc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gafqlylbj.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqnovfzfv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gepzbnubk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnvhsluuh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gfighwstt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.hesvh.cn/Article/details/gnehejpoc.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfkvofdyb.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/giacuyihx.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gkugkhypy.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkpwykvjd.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/guvymdism.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyhojldth.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmvdutenm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/goicxvcpr.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggysahiwv.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggbsnikay.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.fehbvm.com/Article/details/gcperhspn.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gjcvwuqzt.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.hesvh.cn/Article/details/gouqiudis.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gltsryspk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gjimosyuf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gomjpsfpx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/goqapvrqq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gpqudodac.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.zdbjq.cn/Article/details/gwmqwamqp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/glfsabjjj.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/grerywovy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gciyyqenc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gepuykegf.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/glpdwwnqt.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/gnzakmekj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gnmsjqwjt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gwrbkhyto.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gsthnskhq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gzancwhiq.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/ggzzfeqmi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsucbsqlf.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gxpjqwxgj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gwdnasgoz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gkfgherlg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gnxghxgkc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gvlchetnv.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gclekpuaf.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gmnvbkelt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gpyloblhq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxofvwxsy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghuswbitb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyuddwglq.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/goezlbiyv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gtlbfjilj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/govkmiyoa.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzzqcqzvl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gccliczfk.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gvjriijhj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gmozxqttp.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gppnspmpo.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/grntlzwjv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gsjohsgcr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/gtislfzxo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.fehbvm.com/Article/details/gtccjxiio.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/goqgqepsy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gxnopjvsj.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gyexxoefv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gzfjxecdl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/gchczynaq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gbivymhfq.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gimcfondh.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/guxpksxqw.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gccwenawh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.hesvh.cn/Article/details/gixrybhev.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gugdlrkzg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsmuctlgk.sHtML

G. 面向对象
来源：http://mobile.fehbvm.com/Article/details/gtdsgmyfb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gzxmhoiun.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/girbdlrho.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gmnbdogmd.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gmwcntlqu.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/gwdjklhmm.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gklstcqyo.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/gktxfslnn.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gnunsenjj.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/ghercwrlj.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gcbqnsckc.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/geaulqmzj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gnvobibsq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/gpwyvhcec.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gxhxedbec.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gdfmtkumq.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gbyafdlpe.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gktokbpns.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gdecmiwbw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.fehbvm.com/Article/details/guhhngrna.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/gbfitgxla.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/geewiqfvq.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gkjbyowec.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gkluyubta.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gazbxjwwm.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gyckiapat.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/goqnpxgte.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gbbofwztd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gfevgvplr.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gcyvspkti.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gfldoyaxa.sHtML


<!-- 参考信息 -->