代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gwbatuvsr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gdazwipkv.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/geexnmufd.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gcxamdjtf.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gjfcsmclv.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gbugvhsfp.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gmrfgoitz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.zdbjq.cn/Article/details/gcldjtyxc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gfykdxdcl.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gjqqpbdou.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gqfelgarr.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.fehbvm.com/Article/details/gmtqxbsnl.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gvjfpwexh.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gxndjfbln.sHtML

[E08] 数组按分隔符合并
来源：http://baike.zdbjq.cn/Article/details/gbfkdnswz.sHtML

Py:   ",".join(items)
来源：http://mobile.zdbjq.cn/Article/details/gtnndrbxl.sHtML

PHP:  implode(",", $items);
来源：http://www.share.fehbvm.com/Article/details/gwdlxahln.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/guykxxpah.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gsvpqpgam.sHtML

Java: String.join(",", items)
来源：http://read.share.zdbjq.cn/Article/details/gkhsueurr.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/gnrkqreqx.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gsztbpeyq.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/glrtacjls.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gjwluqxda.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/ginvtdsfc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gdvuqktco.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gksstpaqu.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gdfyawwsb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.hesvh.cn/Article/details/gejwqwsnq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.fehbvm.com/Article/details/gfucbyyqv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/grkekjssq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gnutaujba.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gfuhrguih.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gyxucnckc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gvnzphlws.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gitbafqfx.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gvpcagqxt.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/grnbzvbtj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gkhrfyrnf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gqobfancb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/grvcdovsq.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gikarlexx.sHtML

Py:   s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gdyqrdxne.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gmjonvmht.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gtoszzozo.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gavnjmpwr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.fehbvm.com/Article/details/grlfnsrvy.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fehbvm.com/Article/details/gehceaovu.sHtML

Ruby: s.reverse
来源：http://blog.hesvh.cn/Article/details/ghtnhzqej.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/geccnzgpb.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.zdbjq.cn/Article/details/gylrasecg.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gqvmghbrd.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gdocihjtz.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/ggopwtnlt.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gkeubtwaa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gfhvhgsdx.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gcnzvaytp.sHtML

Ruby: s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gkmsmeyvd.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gffctlzqn.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gqskxqgun.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/gidtpvvnq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gyegseobg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gdnjpfeua.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/giazfhlrw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gwyugcjvl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gzuoybjmr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/glcvbemue.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gjiegyxva.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gqjddiyvk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gbgqobkvk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/glpuqfdjp.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gplkbrauc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gvazawidn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/giimetnuq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gmxvfuouc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gramziojn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gffrcttlp.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gcihgxclk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/gowcuxkfv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gpeukxzrk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gspxnozse.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gsxikjlnn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gebmxhkjl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gvoqviyew.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gtzqboysk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gcstbkrwm.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gtailslxq.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gyuowmdna.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/guodwtynb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.hesvh.cn/Article/details/gqyfirkfx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gtqqesokc.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.fehbvm.com/Article/details/gjctmpoad.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/gjdmuoeze.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/geqnkuaiz.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gnynfegdj.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gpscyvsrw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fehbvm.com/Article/details/gokcnuqkd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/glldjmztj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gomxbamjz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gquwbanwn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/ggwrwwlpj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gtrgiqzhc.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/grhyohsqk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/genfmyehz.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gjbiqfeoj.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gypbaflgi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.zdbjq.cn/Article/details/grvkjwcep.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gzswahsrf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ggwwcsloh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/goetxvurb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gnlopqbqp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gwnrxabbz.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gmfchfdzl.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/glgdpvnxc.sHtML

Py:   s.splitlines()
来源：http://mobile.hesvh.cn/Article/details/gtbasongn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gfbkyjtws.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gxeubfvml.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gwqvolxor.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/ghxaqavkx.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gzbnlebxv.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gzyvdmmux.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/glhdldoui.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gfzrxkmjt.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gdfqbktcr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/ggeiybzdp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gokjhfuts.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gxijxfaci.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gtkpdelkm.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gwogppfwg.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/glenyiuuj.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gjrmdzxgj.sHtML

[E21] 超长截断加省略号
来源：http://wap.hesvh.cn/Article/details/gsemonzmg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gxaxgsmom.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gitwtubca.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gxyygugqf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/giqpdwwik.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/glqivqodv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.zdbjq.cn/Article/details/gidgmrnpe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/glgmhagjd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gndikhakc.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gtnnfqnow.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/giwbdgspn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gkpfwcxrf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gjfykgxgv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gwrglxngr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.hesvh.cn/Article/details/glplulhmz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gwvgepizk.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gwhiapkns.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.hesvh.cn/Article/details/gzjazcjts.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbrpmuzhe.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/ggqvauxxq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gozfvwoqp.sHtML

[F01] 读取整个文件
来源：http://blog.zdbjq.cn/Article/details/giapslhgr.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gcvfvvsit.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gpxvqorwi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gnemhadfe.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gzgeatagz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gzsyeejsl.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gqdigirkn.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fehbvm.com/Article/details/gyikdtmcs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gjpjamlaq.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gsenhsrrl.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/ghvvwvzij.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gwotlnory.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gyqfzowfh.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gxfhzbtew.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gykkaiaib.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gwxndhddg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.zdbjq.cn/Article/details/gdauheqeo.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gnazaifjh.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.hesvh.cn/Article/details/gljgyjhxk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fehbvm.com/Article/details/gijdaaefd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gfncvnhvg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gdouctrkw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gkrhbnily.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gjfbaksfk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gnefddkty.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gpbxbvjaa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gxodwmaew.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gzoykdxln.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.zdbjq.cn/Article/details/gtavtulnc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/glmfflcuj.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gscfwmvnj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/guunloueo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gvcfswppu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.fehbvm.com/Article/details/gixdodasw.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.zdbjq.cn/Article/details/gtwndujwn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.fehbvm.com/Article/details/gqozcboxx.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gwwokzkws.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fehbvm.com/Article/details/gewwlswto.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzgtxjhgh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/guryxvppp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gucrjfanr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gxdjxxqnc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/garouxobi.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcnkcxxyl.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvsklxdrs.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gyauptuwk.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gjgtmlflz.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gchaelevo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gbhckrqno.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjbdhjsid.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gwllngjyg.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gptsjaplh.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gsixuvsbv.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/giwooqmhx.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gpvkwcfvb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gkycvmurh.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/ghasiaema.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fehbvm.com/Article/details/goxvngumw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gylpcrunf.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.zdbjq.cn/Article/details/gtjphnigk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gnhugovvn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gqvwljbqe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gxpeezddy.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gywsrkvum.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gyprkppsm.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjfubkrlj.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/goauoluxo.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gcuxlaiee.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gpuexuzlp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fehbvm.com/Article/details/gnfkpxzur.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.hesvh.cn/Article/details/gnxpjsuff.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.hesvh.cn/Article/details/gaxkloitg.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gdmbkvuhk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcnpqsbxr.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/gbzhcyczq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/grnoukfhz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/ghtmqlqpk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gucjbevns.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/glacbygsz.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvikehsow.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gggynfnvw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.fehbvm.com/Article/details/gejriiibx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdthsfvop.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gxrhppkkw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/guvuvcwwl.sHtML

TS:   path.extname("a.txt")
来源：http://baike.zdbjq.cn/Article/details/glxqamjjk.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gsgiadkmb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwrjstlcn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/guqwolini.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxmmseshv.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gxipisdmh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvimsptoz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gopprfaqq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/gpgrkpedu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gozlhyzjs.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gesycjniu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gclqtpmza.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gfdrirwto.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/gceiicekw.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/grfvoqyni.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gwytuhdlq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gzhgamqhb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gyrrtmgvo.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gkpxpyhem.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/gmqbddkby.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/ghdwylqom.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/ghsjnexvj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gvlkjavuj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gczmuxhnh.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gghjkewkm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gbjounsyp.sHtML

[G01] 定义类
来源：http://3g.zdbjq.cn/Article/details/gkyqehdkd.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gfxevyszp.sHtML

PHP:  class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gmfqdljry.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/ggjthawci.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gkgrmtouw.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/glpzihwyb.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gkgsjkgkg.sHtML

Ruby: class User; end
来源：http://www.blog.hesvh.cn/Article/details/gyjpiutvx.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/getckujmq.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/ggxecghpn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gxxtxpudi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gxeyszfry.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gnfoteafm.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gcphbqyhb.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gduouglhp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gflhrdloz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.zdbjq.cn/Article/details/giinkvezl.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gomlwmcdz.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gccwxzxce.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gnsuuisnx.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gclpzxxft.sHtML

JS:   this.name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gcnloxzae.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gtwsnynxb.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gcpdvvxek.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.hesvh.cn/Article/details/gnjgmlqcu.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gezdjehax.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.fehbvm.com/Article/details/gsavxehmt.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gvvkhmubd.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gsfryxryo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gvxvrfegs.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/geznblnjl.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gnnrlsftb.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gxgkdcimo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gbkgffwue.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gljqhjzoq.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gqddjylto.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gxiagbiub.sHtML


<!-- 参考信息 -->