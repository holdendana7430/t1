代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/ggcdjiqmh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gzdjgmrgj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gzbqvwmsf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gvhqlwyei.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxhybfqf.sHtML

[E07] 按分隔符拆分
来源：http://3g.fanxiaobao.xyz/Article/details/gllwjagat.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fanxiaobao.xyz/Article/details/gcxilsewt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gfppvvdcz.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grawcolae.sHtML

TS:   s.split(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnpjyfvd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmebdrdbv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoieyqom.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhivfqso.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.fanxiaobao.xyz/Article/details/garelaxsn.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fanxiaobao.xyz/Article/details/goqvzpkbx.sHtML

Py:   ",".join(items)
来源：http://mobile.fanxiaobao.xyz/Article/details/gucssgurr.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fanxiaobao.xyz/Article/details/guapgpvrw.sHtML

JS:   items.join(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcknqpqj.sHtML

TS:   items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/gcdmwqwqc.sHtML

Java: String.join(",", items)
来源：http://blog.fanxiaobao.xyz/Article/details/gzivcapbh.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjciqoij.sHtML

Ruby: items.join(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvtvztfp.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fanxiaobao.xyz/Article/details/gljsljsyz.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fanxiaobao.xyz/Article/details/guglowxzg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fanxiaobao.xyz/Article/details/gqdnvwaah.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggredqvyp.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxwctpxd.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdusbvbx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fanxiaobao.xyz/Article/details/gepiaffbv.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gypkxyiqx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gwjdkjbzf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fanxiaobao.xyz/Article/details/gliphceql.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.fanxiaobao.xyz/Article/details/gnbxgrrdu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpcwrtur.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.fanxiaobao.xyz/Article/details/gijlmrqro.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkvfldyw.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gyknaylox.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fanxiaobao.xyz/Article/details/gxqwxawgb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/grxujjbnc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fanxiaobao.xyz/Article/details/glhlyypcv.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzbshund.sHtML

[E11] 反转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjugftyf.sHtML

Py:   s[::-1]
来源：http://m.share.fanxiaobao.xyz/Article/details/gmohpxred.sHtML

PHP:  strrev($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gawutepgo.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwpsxdyg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnblgryb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fanxiaobao.xyz/Article/details/ghwdqljnj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gourbgflo.sHtML

Ruby: s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/grlqbvpph.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgpateuc.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdsqrvzpi.sHtML

Py:   s.count("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grhvqsmtg.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fanxiaobao.xyz/Article/details/gwgurvtnu.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/gwfmwzamv.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/gekaybvid.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.fanxiaobao.xyz/Article/details/gpdbfgxze.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gogizbegi.sHtML

Ruby: s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gkjcaadae.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fanxiaobao.xyz/Article/details/gqfmtjwtb.sHtML

[E13] 逐字符遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvnwcvjg.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fanxiaobao.xyz/Article/details/gchkfotqg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtoeszbgt.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhfcnolq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gguykgcqn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdxdnxwv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gymozixaw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlihjogm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdwmxvsf.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fanxiaobao.xyz/Article/details/gkmklbyfl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fanxiaobao.xyz/Article/details/gzusopwgr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gawbghtar.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fanxiaobao.xyz/Article/details/gawdemabz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gemgxrkat.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gagvgqjpl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmszxcly.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnupraxz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlzsjend.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.fanxiaobao.xyz/Article/details/glytanvqb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhrbeuak.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrfnanvb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.fanxiaobao.xyz/Article/details/ghwedaulg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fanxiaobao.xyz/Article/details/ghfzawfiv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fanxiaobao.xyz/Article/details/gilaaagxu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjamsukf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghefhbxfh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.fanxiaobao.xyz/Article/details/ggamzmhsr.sHtML

[E16] 数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gvbskwozk.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowqgguex.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpomjojji.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fanxiaobao.xyz/Article/details/giacbnrdc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fanxiaobao.xyz/Article/details/gysnxqpkq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnipimoes.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdmzxvgr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqygtjsy.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyyytrgd.sHtML

[E17] 首字母大写
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdnyashb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsstuauu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gtinozflf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxinzikzd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/golzeksjw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gujwkvtri.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.fanxiaobao.xyz/Article/details/gdscmtxre.sHtML

Ruby: s.capitalize
来源：http://mobile.fanxiaobao.xyz/Article/details/gsjgvitkb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fanxiaobao.xyz/Article/details/gryknylik.sHtML

[E18] 模板占位符替换
来源：http://3g.fanxiaobao.xyz/Article/details/ggftmkcmf.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fanxiaobao.xyz/Article/details/gwkqkwocq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fanxiaobao.xyz/Article/details/gcmofeixn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjwspxpt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzmtpezti.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/grufoshbl.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gxpmstlko.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fanxiaobao.xyz/Article/details/gwhkkwhna.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fanxiaobao.xyz/Article/details/gighkwjqi.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrdjbdgk.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlqecqih.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscaxwboo.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fanxiaobao.xyz/Article/details/gjschhjwo.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbjanden.sHtML

Java: s.lines().toList()
来源：http://www.share.fanxiaobao.xyz/Article/details/glqtcbvel.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fanxiaobao.xyz/Article/details/gqbilapjk.sHtML

Ruby: s.lines
来源：http://baike.fanxiaobao.xyz/Article/details/gcajjjkbf.sHtML

C#:   s.Split('\n')
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiljniox.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fanxiaobao.xyz/Article/details/gtbfngish.sHtML

Py:   if not s:
来源：http://wap.fanxiaobao.xyz/Article/details/gqekzhmah.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fanxiaobao.xyz/Article/details/gegrvnhpe.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gyariqwlq.sHtML

TS:   if (s === "") {}
来源：http://wap.fanxiaobao.xyz/Article/details/gcdmvglus.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufrtlmar.sHtML

Go:   if s == "" {}
来源：http://baike.fanxiaobao.xyz/Article/details/ggkrgenyh.sHtML

Ruby: if s.empty?
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghimqwmlp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpefaycop.sHtML

[E21] 超长截断加省略号
来源：http://baike.fanxiaobao.xyz/Article/details/gpoxhtybq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaaalgsy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gnddtbtxj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/grrchiibg.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gqubnojwf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfxntxxv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcamauto.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfcuyrya.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gksogwnjw.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gynpsdzti.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gjzzfbopp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/girkwcqst.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fanxiaobao.xyz/Article/details/grfvqsrww.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmyghszt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepdepcuh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfniunlyr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graxfeurk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfwzozwo.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvmatbnx.sHtML

F. 文件与目录
来源：http://blog.fanxiaobao.xyz/Article/details/gaemwbrlx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/guhymiznt.sHtML

[F01] 读取整个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcrtlkxjy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmlqrgeh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gffusrgmh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzczhnkt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtubujyrs.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/ggkehyaqh.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fanxiaobao.xyz/Article/details/gpompdatj.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/grinrppde.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gzwedqlnr.sHtML

[F02] 逐行读取文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gahoytwks.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fanxiaobao.xyz/Article/details/gbwucfqbo.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggwlqmtqx.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fanxiaobao.xyz/Article/details/grmtqzoqw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gffdxahfx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gjnloibkx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyhakcss.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fanxiaobao.xyz/Article/details/guhptijym.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fanxiaobao.xyz/Article/details/gsbryfcxl.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.fanxiaobao.xyz/Article/details/gtviowvly.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gptfpoaww.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdtxitczl.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnlardkve.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvatedrb.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gkpgekunu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdmzjiqh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/gswmjksst.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gmiwpvrsm.sHtML

[F04] 追加写入文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxmghjav.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gngrmunne.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fanxiaobao.xyz/Article/details/guehpabhh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gcwpsuook.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjqanpfz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fanxiaobao.xyz/Article/details/gwlilpdxs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giopyofva.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.fanxiaobao.xyz/Article/details/gvarkyxvq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbfjrrxe.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvwikpat.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fanxiaobao.xyz/Article/details/gyajvkpaj.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gbtonhrqa.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/glfoqynuc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjsetfom.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gjonmjoot.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntktidfc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrrziykj.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsotivpa.sHtML

[F06] 删除文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsheickic.sHtML

Py:   os.remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gynrwlgru.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjrbqxyz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvowchrk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gahuiwylv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gdnbxyjcb.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/glenxjwqq.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifcgubke.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gpiecxhqj.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkoyrljo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fanxiaobao.xyz/Article/details/geuqrbvrh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gormsrpjl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fanxiaobao.xyz/Article/details/gfvzlpsho.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gxtsfckqo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fanxiaobao.xyz/Article/details/guftczkom.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyfgjanqa.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fanxiaobao.xyz/Article/details/gyskfssxz.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fanxiaobao.xyz/Article/details/gjglzlwby.sHtML

[F08] 遍历目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gznkowqin.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsieejnvw.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqenrmet.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fanxiaobao.xyz/Article/details/genmivmzf.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfxzjrhs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fanxiaobao.xyz/Article/details/gzjfumgut.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gswczuaak.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomsbmjic.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvbhbdht.sHtML

[F09] 获取文件大小
来源：http://baike.fanxiaobao.xyz/Article/details/gwkcjloeb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/grsbxqlfq.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzwtqwtc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkvbysghg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fanxiaobao.xyz/Article/details/geflpbnjl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gdftwfaqv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmnudlti.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/glcyjqben.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gtakaixkw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fanxiaobao.xyz/Article/details/groabgaps.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gcrfsbybm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktpmprhy.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrrqppec.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbueiuex.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guunzgwgs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjqyridx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gyugqwiuk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grosdvkhi.sHtML

[F11] 复制与移动文件
来源：http://wap.fanxiaobao.xyz/Article/details/gcjewutkg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkpnfysf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gfyxufsxs.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gxeaeuygg.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbsuswnz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqukgvvvj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fanxiaobao.xyz/Article/details/gscibkabj.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqimvaco.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkfngswa.sHtML

[F12] CSV 读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyxxszrt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fanxiaobao.xyz/Article/details/gkfnpognz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fanxiaobao.xyz/Article/details/gehntxeaq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fanxiaobao.xyz/Article/details/gmolurwls.sHtML

TS:   // 同上
来源：http://mobile.fanxiaobao.xyz/Article/details/gicsouxti.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fanxiaobao.xyz/Article/details/gvgxciytu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fanxiaobao.xyz/Article/details/geomqjdji.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fanxiaobao.xyz/Article/details/goflndynm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvlytpym.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzpwjnpqw.sHtML

G. 面向对象
来源：http://blog.fanxiaobao.xyz/Article/details/gqzvinvfy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gmynlcbbu.sHtML

[G01] 定义类
来源：http://baike.fanxiaobao.xyz/Article/details/gcpskysxg.sHtML

Py:   class User: pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwflcbhs.sHtML

PHP:  class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnmdepdk.sHtML

JS:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/grxwhatbf.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fanxiaobao.xyz/Article/details/gffrwkqtz.sHtML

Java: class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuwtxjco.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjukaphkm.sHtML

Ruby: class User; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gakhqnpuz.sHtML

C#:   class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gcxgncmkq.sHtML

[G02] 构造函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqufctpqk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtspexgd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxolqsiz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfjmatdzh.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyjbrdak.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grwbrmiih.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fanxiaobao.xyz/Article/details/gwgtmjyje.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gbfrjodzz.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/geezqjigi.sHtML

[G03] 实例属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gozhzumvf.sHtML

Py:   self.name = "x"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvzfmrly.sHtML

PHP:  public string $name = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gpjfggcex.sHtML

JS:   this.name = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/glqhfqyya.sHtML

TS:   name: string = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gotnjgcuh.sHtML

Java: private String name;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfgfhega.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fanxiaobao.xyz/Article/details/gxbenoaww.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grlbvfheq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqpjkzdh.sHtML

[G04] 定义方法
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghssukqwy.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fanxiaobao.xyz/Article/details/gnoocypwv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gumzjkiai.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwhcedodn.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuwykibd.sHtML

Java: String greet() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gcmzatzlv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/gowdkagna.sHtML

Ruby: def greet; @name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gjjwmgyvv.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fanxiaobao.xyz/Article/details/guakapisq.sHtML

[G05] 继承
来源：http://mobile.fanxiaobao.xyz/Article/details/gcifevrrw.sHtML


<!-- 参考信息 -->