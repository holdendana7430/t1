代发 wailian999

C#:   s.Replace("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gdjbyxpwk.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fehbvm.com/Article/details/ghtnaqkaq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gncbdktmj.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.zdbjq.cn/Article/details/gjvctzonm.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.fehbvm.com/Article/details/gnfeyycjd.sHtML

TS:   s.split(",")
来源：http://www.share.zdbjq.cn/Article/details/gtpdlbxkl.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gzpcxrdxk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://mobile.hesvh.cn/Article/details/goeryimvv.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fehbvm.com/Article/details/gggtyekzc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.zdbjq.cn/Article/details/gqejarvsk.sHtML

[E08] 数组按分隔符合并
来源：http://blog.fehbvm.com/Article/details/gdncqjvtc.sHtML

Py:   ",".join(items)
来源：http://blog.zdbjq.cn/Article/details/gmzvcdrkz.sHtML

PHP:  implode(",", $items);
来源：http://read.share.zdbjq.cn/Article/details/gbmacfmfp.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gqokcvfjf.sHtML

TS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gowwwcwmy.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gfjwdrzxz.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gpkvbbhte.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/ggcyfoner.sHtML

C#:   string.Join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gmijkbhqx.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gxdyaocez.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fehbvm.com/Article/details/gkhkcvtup.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/gdqmzvllo.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gdrfnwsgp.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gnhxopvtb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gdoqyfdpw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.fehbvm.com/Article/details/gztetlzfd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.fehbvm.com/Article/details/gialkavpb.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gcctxccnn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.fehbvm.com/Article/details/gkfoflgfv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gcrsnaypt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gmxdvguwp.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gzpmrodkc.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gvjafwgvt.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gyzpzapbl.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gsaifeaaf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gscmrorzj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/ggrlbmbjb.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/gmhsbzdta.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gxmtqqymm.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gqirpzqlg.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gmfjqlfag.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gmfpteiez.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.hesvh.cn/Article/details/gtxwhrjzj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.zdbjq.cn/Article/details/gxrnibbva.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gsybgqmuv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gcoxhyngk.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/gonipnqzj.sHtML

Py:   s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/gmxgonbon.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gvftacvtb.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/guyuysqao.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gxmnconiq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gpnzlkyws.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gtphmfpcz.sHtML

Ruby: s.count("a")
来源：http://blog.fehbvm.com/Article/details/gibqzkbxy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.fehbvm.com/Article/details/gjrpgzjgt.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gxnmaezha.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gpsnqsmjl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.hesvh.cn/Article/details/glytegnrg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gajzfqgey.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gaihzmvva.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gnlzzkenx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/geuwtkutt.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/giwzeqcqt.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gswdmtpav.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/gwmumlfnq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gapyzrbms.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.fehbvm.com/Article/details/gowaernke.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.fehbvm.com/Article/details/gykhdjxfy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gcphimqsi.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/ghxpqjqau.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.fehbvm.com/Article/details/glxnwulad.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gzhzqfaao.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gvumweebm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.fehbvm.com/Article/details/gwoofjyao.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gpzmueoxt.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/ggleimlqb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.fehbvm.com/Article/details/gsenlabcp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/ghynrvlpw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/ghelvqbuk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gyeoiprxp.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gjnbtfyje.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gnondsruu.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gcabtoktn.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gecweykaa.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gvfscwvlz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gecxivjlp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gbupksmhk.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gtubajwyh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.hesvh.cn/Article/details/gfiybydhw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gnobdqfgv.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gnwsmlvvv.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gatppwfxu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gnduakjjo.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gdsyuznpg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gkenclyhj.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gqjmbhgdo.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gumlbkixn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gkfohzdnv.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/giyiolnib.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/ggcaiyixn.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/gzgeezfqg.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gsmfzdkkq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gbyxvptkh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gviieiapm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gwtvtmghp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gfnxsvwis.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gvrcwdgbu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/galkgeaul.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gdtsirfvm.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/glchcyllt.sHtML

Py:   s.splitlines()
来源：http://m.share.hesvh.cn/Article/details/gqsglwift.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.fehbvm.com/Article/details/gcjkomatk.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fehbvm.com/Article/details/glzrrlqtl.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gwovsgaar.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/glnvyffnl.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gnjtfnnxe.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gawkfxumk.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gdaiumgjw.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.zdbjq.cn/Article/details/gnqjwtohj.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gkzauveaq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gcjezffwv.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gdvxiurfo.sHtML

TS:   if (s === "") {}
来源：http://read.share.fehbvm.com/Article/details/giavgxquo.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/geyajxrhv.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gaatftygx.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gbaazunpq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/gikgcexwv.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gqrzswjzv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gxyodoink.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gipmenchh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gwawcxoaw.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gkelzjcam.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/giaibvire.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gfvmvxvex.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gfoocgghe.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/grvmppuih.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gpchcocay.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gdlgiznvr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/ghkmiozcc.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gnornhtgo.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/ghxnbrdgy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gpblamgfg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.zdbjq.cn/Article/details/galzltkmr.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fehbvm.com/Article/details/gyjkgglkr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.hesvh.cn/Article/details/gsfujwiil.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdkwqzods.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gqtopgswx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glnogmnhc.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/gcymogxya.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.hesvh.cn/Article/details/ghlcmjfdd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gsbffpyoi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/golzoecwo.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gloqaeklr.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/ghuwdzjll.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.zdbjq.cn/Article/details/ghlfbzwex.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gwhavqfnp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gjcqanrra.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gjnijgwgh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/gedlxzldn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gpecorvgp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gfphqvysy.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gsddxluoh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/glakjgold.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/ggwcdpbxn.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gcznfiagn.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gevsiopnp.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gwuwjlgjw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gfqzlyhaq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/guazynkmd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gqckaekej.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gembyhqrl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gelqcxzqr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gqdcmfdwm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/grnlsihsa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/ggiogyfwd.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gsgxbqgqg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/ggcxrjokf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gkraxdbtt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gtgqqsxae.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/glzjzecdh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gegeunfgm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gbjdhkiwq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gjtacumfz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gvcraopio.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/ghnjtrkpp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gyvwsqrnw.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/groonvtge.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfjwwpufw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gldtmvngh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gllemgjbh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gwqzgpgri.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gptahfmev.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcxjakqxm.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/gotrbeomq.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gbdijylwe.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gphnusaws.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gljhgqpwk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gneisjaih.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gaoreepsi.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfkvygiej.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsymubsig.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gkewzswvx.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/ghbsjargm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/golcukoze.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.zdbjq.cn/Article/details/gzsmqriic.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gotgsthhh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gburfyeck.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/grkeegvlx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/gekhhcfbf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/ggrlcgfvu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.hesvh.cn/Article/details/gulogxbam.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/ghrvzqyzd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.zdbjq.cn/Article/details/gbcnpkxnu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/ghrlwagho.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gzwminpcw.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/goztsxzdx.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gdrmnbntd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gjbyorxpp.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/gapyeldsp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gieenepuz.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gipmjfvlv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbqvvhine.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gubyvhmum.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gdiqweuva.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gxztgsmsx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gclnmrlcs.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gsfphufoh.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfdcuyphg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gidyjydbk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fehbvm.com/Article/details/gyxlnazlz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkgxkprub.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gdonbmnwr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqeyuesoj.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjjmoyyge.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fehbvm.com/Article/details/grelfaltb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/guqprwymb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/geadpqldb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gypllebrh.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gjmqvbqpn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gmtrcmgqe.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gpvggbovr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gfbqgaknn.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gxywuworv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gumkjkevg.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gsonoxxvp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gqcshqfoy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gmggududz.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gheawmwao.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gpqdbqptb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gwncayjxj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/glptqyywr.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/grpuuyyoe.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gqjxrnoih.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gyavtzzwc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gioacxdbz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gnrwyssza.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gvvynjozl.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gbqpgkgwa.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxxsoeejb.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gwkdrzbya.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gjesqrrtt.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gglxmhjup.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gsjdnidkt.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gsuplflxl.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/guswfebbh.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gzhzhdiol.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gqrxtczjs.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/gdwivmatb.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gcrwdiezy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gyrnppkal.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/geewmtzhi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gebyylnqb.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gwlqindkp.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gdpoirhfo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gmrzluehl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gjvnhkwku.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/giqisljeh.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/ganqwutxx.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/guohgwlap.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gwuscrguj.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gzkobvwnb.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gikaczymp.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/geaotrqup.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.hesvh.cn/Article/details/gnusejwch.sHtML

Ruby: @name = "x"
来源：http://baike.hesvh.cn/Article/details/gbpmzvpaq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/ghzuvpsyf.sHtML

[G04] 定义方法
来源：http://mobile.fehbvm.com/Article/details/guuglqvcp.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gxmjhzgxw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gxkqnissh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gecpxssqs.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gybsppnmx.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gcargzfdk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gdmkujkoo.sHtML

Ruby: def greet; @name; end
来源：http://mobile.hesvh.cn/Article/details/gpusaaizy.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gbnmkqyvi.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gwsnqrtpa.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gfighluqy.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gbyzosyrg.sHtML

JS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gmccyipye.sHtML

TS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/grxhvthea.sHtML


<!-- 参考信息 -->