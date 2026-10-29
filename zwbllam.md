代发 wailian999

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/grqkbbbax.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gifmjblne.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gnyutpitb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.zdbjq.cn/Article/details/govluadue.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gveahxeup.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gsnmqypos.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/geqkfxcpz.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gtwjhtnkk.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.zdbjq.cn/Article/details/gxvznuepw.sHtML

JS:   s.split("a").length - 1
来源：http://baike.hesvh.cn/Article/details/graxbtvyr.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gqixmcbxb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gnyqevzwk.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gewaqjcrl.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gfhoyiqtw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gxaysysup.sHtML

[E13] 逐字符遍历
来源：http://www.blog.zdbjq.cn/Article/details/gnvmgfsap.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gboikyoig.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/ggrgmrauk.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/ghtbwgajh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gwekoztvw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/guqvwgcym.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gevlqewoo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gczlzcqug.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gqwiymnvs.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gegsoqzxr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gdkmklepq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gilbnlrzg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fehbvm.com/Article/details/gdzgjbfjs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gckzgrojw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gxnogohmd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/gpckwkjjg.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/gwlrqxzcy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gbsdijojs.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gimrwlqew.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gvramfckw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gxwndqzcj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/ggfxgdrfv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gthuqrsxd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.hesvh.cn/Article/details/gnxoaqanb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.hesvh.cn/Article/details/gmqrejajq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gftsnteom.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gxhjxdtup.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gulhgqzfu.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gnfgbxzqn.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gtodbvlcq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/glbcosiiq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/ghlcynmkj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gwdetlthj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gghewgmwf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fehbvm.com/Article/details/gwqgqfkjt.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.fehbvm.com/Article/details/grcsmnyfo.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/guiyiaisr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/grfdyztip.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gmlcsxafe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gvnhdqvkt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gjtsgnkiv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/guddypljo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gscllzifj.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gpnparwed.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/ghdzbwqqt.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gjvsejics.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gcxygqoxm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gsvhfgpjy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/glulrgtbd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gmikfgvpg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gufacekil.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gncxxxtku.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gjmqpqxos.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.hesvh.cn/Article/details/gckrxxmsy.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/gwqawljks.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gzhusijya.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gikjbrtbu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gjvihsxkh.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gzbshcumu.sHtML

Java: s.lines().toList()
来源：http://read.share.fehbvm.com/Article/details/gvkenbovj.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gdkhxmfqu.sHtML

Ruby: s.lines
来源：http://blog.hesvh.cn/Article/details/gezphwagp.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/gpooujujw.sHtML

[E20] 判断字符串是否为空
来源：http://3g.zdbjq.cn/Article/details/gjlmvrfui.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gvpofibff.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gpxowafre.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/gkswhfvsq.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gkkaqmlka.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gdyhbkura.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gdedmpixu.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gvswawhif.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gqnpkzjuc.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gfqlthimn.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gvekhmlav.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/ggcezpvvd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gmiexpglf.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gidwnxurj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/grzyjrsol.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/ghdrnuvcp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gjlmpijsk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gjgoxrqdx.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/ggidpcleu.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gopenrabj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gkuaguzfr.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/guvwxmywh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gfectqtzi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.share.hesvh.cn/Article/details/gukebciwb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gefzwikph.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/grabahlir.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.fehbvm.com/Article/details/ghypjltnk.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gblxmwnke.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gofvgddhj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpwllkhcm.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gosattmok.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/ggpdqiarp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/ghlgopagf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gzttjlfgk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gdwlvgphx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/glsyxiykv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/glabmetmm.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gprtkpryb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gvsjqqyip.sHtML

[F02] 逐行读取文件
来源：http://wap.zdbjq.cn/Article/details/gejknacjr.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.fehbvm.com/Article/details/gfdfklvra.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gjkuvihom.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqfszbzun.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gkvoywjik.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gnafbskbb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gnfkftpxf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.fehbvm.com/Article/details/gtjrfidql.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gbfcsomfl.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gsvbqnixr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.zdbjq.cn/Article/details/gbhbdqxvr.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/ginxyhjbq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gnsclkjps.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/geijwcone.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/geyegwzdk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/gyypcilpz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/ghicbrwqb.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gtrpdzzok.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/glplxzcoq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gyfffwphk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/glsvethcc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gqhpcbayy.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gzjhnjgvv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/glrgoxfpv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gqlketjpv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.zdbjq.cn/Article/details/ggikkuxhz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.zdbjq.cn/Article/details/gcrrdqsgg.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gesdpzvnf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/grjjafjxq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gynudppve.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gnzvrqeji.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtnvklxlw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gafuvuzyx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gcidlsdfw.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtdrvvoak.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gkarfewnk.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/glugwfabv.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwekpgayi.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gcqdbxhrf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggpjoktdk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gxfslhcmc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gaiuflznv.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbnhnpgak.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gaunxxils.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/goziecsjx.sHtML

[F07] 创建目录（含多级）
来源：http://wap.fehbvm.com/Article/details/gcpcyhdsc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/gxtwqqljl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/ghxhsuzrc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gnqijdzwi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gcwbgzszp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/grvxomvkk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gbgymkhxv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gyhqkkgaj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gbcbqhkoc.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gzcvbiwpt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gedqufyxz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gtmfonype.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gzzjyojbq.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gqdkpqauz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gkdvgrnyp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gzephqzte.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.fehbvm.com/Article/details/ghfclvpna.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gmasbzptp.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gbdugqjhd.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/grbfoqkjl.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gybiafwxi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gqvsgtryy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/glhmsexjt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/geosoawdy.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gbnvnljyx.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gqnzsrovd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.zdbjq.cn/Article/details/gzajosqzp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gypwzclhx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gorylzqxj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.hesvh.cn/Article/details/gjbmmifyc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gqplpmect.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtsezvzez.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gggokpgox.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxoanotys.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcqrdeiwk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnykrqtee.sHtML

[F11] 复制与移动文件
来源：http://www.blog.hesvh.cn/Article/details/gyofmsxiw.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gbmgrnyhh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gwujikopl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gttdlkrai.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gmenmrpit.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/gkjhusgal.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/guhjlpsfy.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzznygndb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gyxumzyjo.sHtML

[F12] CSV 读写
来源：http://baike.fehbvm.com/Article/details/gsepjdfuf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gbuzdhhbx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gwmxiqdbi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gkwyjulfk.sHtML

TS:   // 同上
来源：http://m.share.hesvh.cn/Article/details/ghisqotya.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gehscniky.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gnmhzjrxs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gezxenfyf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gpoquhdor.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkhpmojht.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/glzweibtp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcblxnqcc.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gctgtljtr.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gozoeobdh.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gmwdobwmf.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gbxfkufll.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/grohkvloc.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gjvjpqwfi.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/glaskdqbu.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/ghnfbvovl.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gvgkowqfg.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/ggtmfveis.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/giasumqdc.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fehbvm.com/Article/details/gyiyxgbln.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbrudikyq.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.hesvh.cn/Article/details/ghwvgmrsm.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gyppmodbi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/gitwiayxa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/ghidmvcyk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gdwuojtwn.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/glebdxebn.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/ggepojxuf.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gugqltyqd.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gnhbvbjkd.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gmgvwgqoq.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gfgsonzsk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.hesvh.cn/Article/details/gkxaeuibq.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gwveikapx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/guymvouwl.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gcucxesqw.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/giupxmkhu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/gwsynvhrx.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/grxqcblvb.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/glxgzxsqm.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gmkayswjj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/ggrhscnzz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gguquwmli.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/geugdmqvo.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gofzknkwa.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gsiykurqv.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gnvsuisgf.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gqfnfpllg.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gfuparywr.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/grqxvjfrb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gjpnpkblg.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gbheiyllx.sHtML

C#:   class Admin : User {}
来源：http://blog.hesvh.cn/Article/details/gudusawev.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gyzwrpqjf.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.fehbvm.com/Article/details/gxcdnqdsf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/ghjgyqkiv.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gxsmijhpa.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gctktniyr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gbsyobtwx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gppmowjpr.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gikchivdi.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gccnrpfay.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gjgrlhqxi.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gnzrtuwdb.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gueixqvqh.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/geasvacyr.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gcorpjjum.sHtML

Java: super.greet();
来源：http://mobile.hesvh.cn/Article/details/gvijfmsfx.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gibncbdon.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gvzawcxdn.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/glckrjpns.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gzzcbkkel.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/giikieycv.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/grlohrxbz.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gkuoxagan.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gsunztvom.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gikurnome.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.hesvh.cn/Article/details/gorurqgly.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/goneiflyn.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/grsmewgam.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gbzvraebu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gqcqwvgjk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.hesvh.cn/Article/details/gkgwcrtim.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.fehbvm.com/Article/details/gpxdnzkqx.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/ggqzznkqe.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gyvwbedxy.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/gqpxvvezo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.fehbvm.com/Article/details/gsggmjbni.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gcxsjgxsq.sHtML


<!-- 参考信息 -->