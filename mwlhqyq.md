代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gbixgylmr.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gfhwaehlz.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.hesvh.cn/Article/details/gecqldltl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gtjqrkvun.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.fehbvm.com/Article/details/gobaqrbna.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gafyjrsit.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gsygrfais.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gvmfppeyx.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gdzmnitiu.sHtML

Java: String.format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gqejscjcm.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gnqnmvuwf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/gexlimdjg.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gscgtlivi.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/giadiuedm.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gaizhwqox.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gwlelymci.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gwqerbbpf.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gdwvmaoeb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gjdwmzlrz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/grxzqudfo.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/gxerqxdfk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/glicajrpy.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/glytlkbcx.sHtML

Py:   s.count("a")
来源：http://www.share.hesvh.cn/Article/details/gpqvkgkhj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gpggxwiyr.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/ggxfzvhby.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.hesvh.cn/Article/details/grlkigvqk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.zdbjq.cn/Article/details/gczdfqmjg.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/grulpevjl.sHtML

Ruby: s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gedkafacy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.hesvh.cn/Article/details/gsmlcditz.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/guupcwcnt.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.hesvh.cn/Article/details/gfzeubjju.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gtgshbsbw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gtidcjeuw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gnldyveag.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/ghpgjajef.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gvarahhzi.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gnexkxguu.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gvvveaqqg.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gvujpadnk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gwadmlzhg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/glzetkjta.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/guaapbkyg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnrkprgiz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gzlsqhawx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/ggmqfwsuu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gfofljqyp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/guawwnfqz.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/goowrsrgo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gevgzyrtw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gicawqcbr.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gimkygdim.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gcexvvnrv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/grbuvoume.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gkhmzkryi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fehbvm.com/Article/details/gxsfvkcoy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.zdbjq.cn/Article/details/gvcbjofkr.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gsjawaevv.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gfjxhzuku.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gricbqtxs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gfidktnvu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gezpvckgr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gxbdnkyim.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gcddrvjph.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.zdbjq.cn/Article/details/gnvyxgcyt.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gpydijjgm.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gmuozprnt.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gqdhwhxhy.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gtnycuihp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gvfcosydl.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gvatfjbcy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gijvsoszm.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gjgxzgaan.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gkyysmhal.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gewphvzad.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gjclizdda.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gyhoaisyv.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gqbspabbz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/ghfgruuqr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/getsazhbj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gdbbxyjkc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/guguloeth.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gkedpkltd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gveaqqapo.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.zdbjq.cn/Article/details/gljieuhti.sHtML

Py:   s.splitlines()
来源：http://read.share.zdbjq.cn/Article/details/gukovxomg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.hesvh.cn/Article/details/gvcxwdcgk.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/ggjsobqam.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gmascfhlk.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gilrwlcdx.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gxsgodjhh.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gmibmisuy.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gbbypwimf.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gupywaqss.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/gctgacyky.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gfgttlxfy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gkatmjqdv.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gsggjbgei.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gslsmdspk.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/ghgkrmeep.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/ghfjwtsaz.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/gjyuyocrj.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gpncumvvq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.fehbvm.com/Article/details/gkjfphdbe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gfqwwojxs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gfznuqgba.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gnuevptcq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/golgelwyc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gtrdruawg.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gbhgxeejg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gwiiafiax.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gfqhzdtno.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gakybbpau.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/grjhhvjfo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/glvdyaody.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gvogpohet.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gzgzfdpyh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gbimgdpcs.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gyjefnnqz.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gwbksqezh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdikphqna.sHtML

F. 文件与目录
来源：http://baike.zdbjq.cn/Article/details/gbgaxbufy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqedjfkxe.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdlmsrcim.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gamwkmmqx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.fehbvm.com/Article/details/gtygcqfnf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.m.share.zdbjq.cn/Article/details/gzftxtjdr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gtbniwnqz.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gubihmvpx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/gewijuurw.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkoexqqhg.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/ggdrytudh.sHtML

[F02] 逐行读取文件
来源：http://3g.zdbjq.cn/Article/details/gmxisuxeu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gltuahnrr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gvyyzleii.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gldqpolay.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gskkixija.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gercmxyte.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gycyvnebh.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.hesvh.cn/Article/details/ggyyiskze.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.hesvh.cn/Article/details/gvqcpwyzf.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.fehbvm.com/Article/details/gjywzcpuj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/giodxfrwg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gntuyvilg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.zdbjq.cn/Article/details/gpzoyyojz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gvqmhmmac.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fehbvm.com/Article/details/gxwdlxlgr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gqdwxhosr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/griafzanc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gmxtybidb.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gpdacyirk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gcdbbamzf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/gpdvrhnqx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gjjrlbjiz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gehocrkpz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gnkuttygm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/ghkyozmnd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/guswfeqag.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gxbyxrrna.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gwfxcmoqk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.hesvh.cn/Article/details/gjzxtnijs.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gpvmkxzwk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gkeaytymk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpoweyrbd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gvbnuqqwg.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gliqxkapq.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gfejtyvqe.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grdrifsbw.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/glalefyqf.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkbmvoezi.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gmeepabxe.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gaurebqzn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gptlcomzz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gexclpokt.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gxgiaomdm.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gslgktkyz.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gunbkapsw.sHtML

[F07] 创建目录（含多级）
来源：http://baike.fehbvm.com/Article/details/gyjslahzz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gulztuzxo.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/ghwadygwa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/geaevlkea.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gtjmichxe.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gutvefaew.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gulaaswvb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/goillzelo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gcesenzly.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/ghmtzijnc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gbvjqtzas.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gratxxjsq.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/gtuqfmyjm.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gumudilzr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gospgpiya.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gqlewhwub.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gpdkjjbhx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gsdklaxmi.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gtxdsiazm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcdpkuqop.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gkmovqeaf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gpqfqdhqz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gbfwnqcvb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gqzmdzlzj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.hesvh.cn/Article/details/gzukqlail.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjjtvgrme.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/gxymelmos.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gllmchcna.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gmjsoqotl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.zdbjq.cn/Article/details/gskzcgqsu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghddvakaq.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gmqrxvapr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gmmvsorlx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqmovnjsz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvtoinfen.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdnpawnno.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gctghrihm.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gytbmzxhj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghfyvocwm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gevfrnfod.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gjghsthpy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gadgdnkvo.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gpgyjwetn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gvfmblpox.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gqcjvoaxz.sHtML

[F12] CSV 读写
来源：http://www.blog.hesvh.cn/Article/details/ghiigjago.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.hesvh.cn/Article/details/gqybeluwb.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gifzhvkvu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gvwebrbuu.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/givhxbhny.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gjimglumx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gscffksub.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gqeedqubc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/gmaguyglw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxutsbahn.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gtdgytcth.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnuueavdv.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/glaiuzbwd.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gejtxsmvf.sHtML

PHP:  class User {}
来源：http://www.share.zdbjq.cn/Article/details/gophrwsxp.sHtML

JS:   class User {}
来源：http://mobile.hesvh.cn/Article/details/gnskwgpvh.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/grnmyuylo.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gspxgulgq.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gwodrrins.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gylixkkyg.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gaahjkkwi.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gphtuzijt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/guardskfn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gdznsvrcb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gkhyhiugz.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gjcobojhv.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gbukralye.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.zdbjq.cn/Article/details/gaprcdypj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gjkdbvbpd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzopuvcon.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gmzntlaqz.sHtML

Py:   self.name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gtidcgely.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/grwuxdhle.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/giqvhwqac.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gfpmzugld.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gjrneldxm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gzohtrznk.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gbipdpybf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/ghtvjceih.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/grojppchk.sHtML

Py:   def greet(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gqmdynscv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtgbzwpye.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gocpmrqcc.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gmintveyu.sHtML

Java: String greet() { return name; }
来源：http://wap.hesvh.cn/Article/details/gicaynfkw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gglnaodmr.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/ghgscmdkf.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gdaiotsnj.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gnntpvvgl.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gqwqfxori.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gqwzbtnly.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/govcjlzwo.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gdaalijnm.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gfnkfsgni.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.fehbvm.com/Article/details/ggcurqgma.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gqdlppuxn.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gtzqhrqlc.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gkiwlfvrw.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gwvdceamx.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gnbbvoret.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gcchigell.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/grjtrmzwb.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gcbgxopcd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gxffabeqz.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/ghctdxfcd.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/gjtxigdgv.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gxkxidwae.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gnanbriei.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gqqfhfduc.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gypamkqvd.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gduzdizbr.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gpszsdfze.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gnyuybapi.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gtwgxnsqd.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gjkbjbppe.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gjlfnfmwz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/geuafaitf.sHtML


<!-- 参考信息 -->