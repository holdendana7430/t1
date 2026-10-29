代发 wailian999

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/glwnyubbg.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/glkwbcroy.sHtML

C#:   string.Join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gredljwwo.sHtML

[E09] 去除所有空白字符
来源：http://read.share.fehbvm.com/Article/details/gankbsjxk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/greziirwu.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fehbvm.com/Article/details/gbocswhjd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gpnaachpl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/geemietss.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/ghhtekawj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.fehbvm.com/Article/details/gslxpcmch.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gmkhbbzfc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gxskgujnz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/gsttaepjn.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gegodnrum.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.zdbjq.cn/Article/details/gpsailkqn.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gexsoaozz.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/ghqnpjgsh.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/gzmnkjwbu.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.zdbjq.cn/Article/details/gvxswqrof.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gdremijxp.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gqbuysdux.sHtML

[E11] 反转字符串
来源：http://blog.fehbvm.com/Article/details/gzhcgsvfg.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gecahlpsb.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gmqzwpxtm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gzbonwedh.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gmcbmdrgp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.hesvh.cn/Article/details/gplslutvz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/grlcosjqq.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gyhmtoida.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/glslwhfdq.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gvfxgfkmn.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gifyffktu.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gwnmybkni.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gooszufbn.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gippmkrjl.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.hesvh.cn/Article/details/gyxpjaszn.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gujvolwsc.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gwfefvrjk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gadewdwtt.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/gjcqxnukx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/ghetughuq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gggiidlbd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gfnumdzcm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gahtqxeqf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/grhzrdpbv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.zdbjq.cn/Article/details/gfacgrzbh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/guhkmsvpo.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.fehbvm.com/Article/details/gzlqvalsc.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gbfihrgcp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/gafnbmkib.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/guoovlnzo.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gpbxfyysl.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gygowotcj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/ghhassvqd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gohsnqink.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gpyfwamul.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gkymrpblr.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gpwpjauic.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gtapsqjzk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fehbvm.com/Article/details/giduqhxdl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fehbvm.com/Article/details/glogmzjwn.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gslbzsnze.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gddthjmwv.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fehbvm.com/Article/details/gqmtxuloo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gmeezpodx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fehbvm.com/Article/details/gwtkzzhcm.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gbmmjwwrm.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/grwmgzqsl.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gugyfghkq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gdwyieqrt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gpwfyldre.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/grvshjyth.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gievqucol.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gvypkavlq.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/grggrfnxp.sHtML

[E17] 首字母大写
来源：http://mobile.hesvh.cn/Article/details/gzlkfsrhv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gdjlhfyun.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fehbvm.com/Article/details/gqhvpgxpt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gczxkyayu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gfrruyirl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fehbvm.com/Article/details/gquzlpnpn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.hesvh.cn/Article/details/ggdplcbbj.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gwsoxvhjb.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.zdbjq.cn/Article/details/gttvzukqx.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gxnhtxalo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/goqbotyom.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.zdbjq.cn/Article/details/gevjdgfjh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gjmpwzuqr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gwadbahpg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/goaadqfpx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gtvfpbgda.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gaaizbwbt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gxmgnupay.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gbzdmwlvm.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/gthsjtxdz.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gonmqiwfl.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gtfhtdcdh.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/goukipcxq.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gyftjmtex.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gwmzsgurl.sHtML

Ruby: s.lines
来源：http://read.share.hesvh.cn/Article/details/gosnlfzys.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gvicypnja.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fehbvm.com/Article/details/gfveiexax.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gpjchjcrw.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gebyjpcwb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/goqnrnzbq.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/grplewnom.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/girdhvvdt.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gbkqdmdot.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gvmtqvxln.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gfpwzpxwf.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gzqhrlmag.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gussojxjw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gqdqzmfyv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gtlzfmdow.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gaydznmni.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gnawexpmh.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gmpbijova.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/guayrwkpw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/glvxlitnk.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gtdgdjggi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdsbomgs.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gtxokfxut.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/ggpbhotbg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gfntmpfas.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gdhfauiwp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/gptxiwkua.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/gbyvnnjyz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gamwamock.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdxgkgpgn.sHtML

F. 文件与目录
来源：http://wap.fehbvm.com/Article/details/ghyjvikik.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbeczkbfv.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gpcrqhasd.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gkyjfhsnd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gyvnqkkdy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.fehbvm.com/Article/details/gwtysuoei.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/godiglark.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gfmmhckyg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gscrupksy.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/guwjvrnnm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gxonufwmt.sHtML

[F02] 逐行读取文件
来源：http://m.share.hesvh.cn/Article/details/gpmusiuwm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gvllutvhv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gmbbhqxmg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/grkiygekc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/getfufzdr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gdzbhjntq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gedduldjz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/gxjttdqwq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gwycishrs.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gfkdayhua.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.hesvh.cn/Article/details/ghuzrokfd.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gjrlvnvot.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gqrybzdhk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gfvoifhpv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gmfpxzrwh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gkmyktrco.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.zdbjq.cn/Article/details/gecratsjf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/guwmrtoxu.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gktqxdomm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fehbvm.com/Article/details/gnbuygxjp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/gcgsgpjnx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/glkyxauee.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/goliusurf.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gcqcpoxvv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gzbsvgzhb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gumipjugs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gobjuhicr.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/gayfcktzw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/godzxhzxb.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gwsnywezu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gnztyjciz.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gpxposyhz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gcnsqqild.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/glszedtdj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbwhbrztr.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqnxpwqkv.sHtML

[F06] 删除文件
来源：http://mobile.hesvh.cn/Article/details/gjloftodh.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmjtjtwom.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gexhjtsxa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gthyyndrf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcsnmaxvx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gkjlighfr.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmnyeskfp.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkbbzcdct.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.hesvh.cn/Article/details/geiuceuuk.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gguuksbor.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gfeguycxl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fehbvm.com/Article/details/gmqmcphqy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gliglslgp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/glsalxdwe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gieinzbqq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gaoipazkc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gdyemizwc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/gckztpcpz.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gxfzqoiwx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.fehbvm.com/Article/details/gjkiqbkte.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gyyjnlirl.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gzehfbesm.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gkgbfsodj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gtxkclfuo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fehbvm.com/Article/details/grmnlyvwh.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/guvcschep.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fehbvm.com/Article/details/gljkcmzcq.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/ggjuvehlb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gssxinxrt.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/galhjyxmc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gavejnoef.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gdbqldfzp.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gxfqdhvwp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/gqpibmvuw.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gildlorzm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/grhojekbf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/grzurbnzx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gslqvjaps.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gsgedegpt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gasauawki.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggdcsimnp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gtqrmodfr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfwpqlhfn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gsjnyfzih.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gbesqsnlh.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gyycsmlyf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gxznpbgqf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gwdpohlab.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqchswfhp.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gpwgfbtmz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/guchvbtmq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.hesvh.cn/Article/details/gdxjrbrxm.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gdrzzefgn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/glzguzbje.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gvphajpdt.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gglvcmgmr.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/ghiutuxai.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gvfzqgrgl.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gwwcxvmjz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gcwuagjos.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gxheeatoq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gaadywjwg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/gxyezlfdt.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gumihqozf.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gkrstklft.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gxxtvapck.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gtafbrqww.sHtML

Py:   class User: pass
来源：http://3g.hesvh.cn/Article/details/gnurzpsxs.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gjatlyoto.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/giquzdaxp.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gktmqmtat.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gtqrvihod.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/gtwonfrsi.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gwizsmupk.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gytrxzzgu.sHtML

[G02] 构造函数
来源：http://3g.hesvh.cn/Article/details/gizvbpubo.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.hesvh.cn/Article/details/getijnxjt.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gxmjtadpi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/grjtdmsul.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/ghcuxzqez.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gbkudrlnj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gluhxmozx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/ggjkdujso.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/glstzqduw.sHtML

[G03] 实例属性
来源：http://3g.fehbvm.com/Article/details/gobctsxyz.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/gzrnrunls.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gmehjmrxa.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gizvgpkdo.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gpdnovlas.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gthakinsy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.fehbvm.com/Article/details/goyyebzmk.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gbwjxqhvm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gldmqshrn.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gaskqyzhv.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gqoocoqns.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gzdliqvpy.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gmodygyks.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gktgdsvvf.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gloezttwj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gwxyiejca.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/guqmfesdc.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gamjofmgn.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gdopqcbam.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gvycftwwp.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gymvhgget.sHtML

JS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gzcpruhrq.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gvumkcglt.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/grerelvte.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gykwzhxfn.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/gmjmsyegb.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gbuvygjnt.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gnsfjktwd.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.fehbvm.com/Article/details/gujgpvtfd.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gzlhxbrfl.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gnqhuednx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gewjnrvbg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gudqqtqex.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gjzfdgqrr.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gqclblvhk.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gfncltljj.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gzpqtpkgr.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gdeemreiy.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gzhwmapuy.sHtML


<!-- 参考信息 -->