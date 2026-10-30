代发 wailian999

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gcfmpawnj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gnysrkkmz.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gxfoljost.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gsbpvxjgs.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fehbvm.com/Article/details/gydnmihaq.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/grxklszoa.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gcizhjfmw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gjggzakwe.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/gqsfuomji.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/googehwuj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gqgdodgag.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gqtlfiapd.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gdqpjahgv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gdlehauki.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gavxgwalr.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gdixgvbfg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gdcmvwdpb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gohuqxaug.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gzedqldex.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gpxnzwdcb.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/grebxqvex.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.hesvh.cn/Article/details/gjpkljrpu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gfgixuzug.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gxwpzcusm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gqiildzap.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gnkjpjizp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gnxhuvmsz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gvgsfhvmw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gpsbbikpp.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gypaagoys.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/gttdjzmei.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gsbjaxjvx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gijbxwgjf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/gcjhuhilc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gtngxnjnq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gfkpycuwn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gohrmavtt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gppgsdjwa.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gbtihwfsm.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gyecifyjx.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gnsvljnfq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gopqcgipg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gttnsmyer.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/goyfxigsu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gkbbxidzf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gfjgtseko.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gysfyzmqb.sHtML

[E17] 首字母大写
来源：http://baike.hesvh.cn/Article/details/grufoknej.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gmqkzqahs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gbcgqiabr.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.hesvh.cn/Article/details/genhehvng.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/glhenwkjb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gscvkkpht.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/gicivxgme.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/goqmrlzbz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.zdbjq.cn/Article/details/ggoawthzo.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/gpdetkrhm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gcnwcqluw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gayceichj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gyfcfbiqn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gfcvfohwf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gzwfminwb.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.hesvh.cn/Article/details/gaswnwtbg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gqznbfutn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gcrfwhwnc.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/ggzsfzcoy.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gvzcmdorr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gpumktecm.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/gnmmdujop.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gtjtjkvor.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gxczkvpza.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/giuhcpngo.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gmwnhofwf.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gqmovijhj.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/ggvurjwbm.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/govdjbgtv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gmbuetbpy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gwinecrnv.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gxigujauu.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/glpzwsuhl.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/ghnyxdiqm.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gnobhkcwy.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.hesvh.cn/Article/details/gxeunmvsk.sHtML

[E21] 超长截断加省略号
来源：http://www.share.zdbjq.cn/Article/details/gjtyczrpv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/guihcjbnf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gfcygxcgs.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gyfxoyyvr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/goiitentp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/ggmclcnxi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gddxhcowr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gkurfwusy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gksouvqnj.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gvqlabjdi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/glhqtyojj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/ghgqhromd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gmrgavmhg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/guabmnvyr.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gcprfszic.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/gkdnidnol.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/giqjdgzqt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/gvaewpzvr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwepdojnt.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gkzglatzy.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqwksgscc.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/gqkvpljsn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/ganikbfgn.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gosfakqee.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gwzmgngin.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gecoxzucc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gfpgjshei.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gaubngfdg.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjsroudiw.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.hesvh.cn/Article/details/gdvfqvhgu.sHtML

[F02] 逐行读取文件
来源：http://read.share.hesvh.cn/Article/details/gcvgnaewu.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/gxybqklax.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fehbvm.com/Article/details/garlpgmbd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gwjysgwur.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gvrsgnglz.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/ghresqqwn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/gthrykghk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.hesvh.cn/Article/details/gagzviypm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gcnkjevtb.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gjnwcngdh.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/ggrnuktnn.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gklvnppbf.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gobofhzhn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gggmkfjex.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gdixlajbu.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gapvxmisp.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gbjulfjaa.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gpjjzzaza.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gtuznxyhb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/ggyisgfqy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gmbrlsrur.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gmwijtwdl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gbzghveew.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gfienedxk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gucltbrsj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.hesvh.cn/Article/details/gkvivzppn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/gcjvlbjps.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gbsplakbz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gocuswzok.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/glghsaern.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gizrvycrv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdpebfxar.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gxulgerpl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/gvjisggbo.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkjfagycx.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdxavhfhb.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gajtxcxfd.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gyiebwiov.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gzwibxhhi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbutmdynl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmrqnvlpk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gdrvkmzvn.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gspwuxftk.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.fehbvm.com/Article/details/gjceayjcd.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gosvjhysf.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gvtmwrsob.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gcwmyocrd.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gxctmknwl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gxszihsbe.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gjboikugd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.fehbvm.com/Article/details/guhzkhbqq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gaqpselyn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gkswapcqk.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gcbvvudfg.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/groofpjwd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gpmhuddro.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/giuvjzjvd.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gncctwbdd.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gtmgloezk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/grvzovtqb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.fehbvm.com/Article/details/goxmkflnq.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gvowtxivz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/grgrgpemq.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gzrhuuuxt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gzcjgplta.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gwrwstoai.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gkolwjknt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gfpmwtypq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gvbogtzmj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.hesvh.cn/Article/details/gqgwvjjbq.sHtML

Ruby: File.size("a.txt")
来源：http://blog.fehbvm.com/Article/details/gijopkokz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gypormttd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gmwttfssv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnczzktul.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmbpreazx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gsjgjekkt.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzvntshck.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/ghchwhvvb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/guyjgdwpn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpezhkkui.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gisqfjbme.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/ggigykkam.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/ggvrnjefl.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.zdbjq.cn/Article/details/gemnhojmf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gsfmwaxjr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/geomenakp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gerhrtasa.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gqijfhlmu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gpyqqlzpb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gxweqpfsx.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gbqkfcmpe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gjvzwbxqz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/gsbhjfbeg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gqighuixv.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gnclahmxu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gpharcgvb.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gjeywnhxs.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/ghemniwhf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gshibdsbr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gfxmgdvmt.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/ggmbzhgju.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwwrgpyqr.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gpprpclcp.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gsueieqwm.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gzrezsesd.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/garpotepv.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gyscnjaej.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gprfyzuwj.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/gxlzvegfk.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gqeiibvje.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gevtioeie.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gnwldwzcq.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.fehbvm.com/Article/details/goavsjsbh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gjlhszkgy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gmmdholzc.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gnpcqfvxi.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gwiumjcpg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.fehbvm.com/Article/details/ggcoarbif.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gebxjdxew.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/guatrgmwf.sHtML

[G03] 实例属性
来源：http://mobile.zdbjq.cn/Article/details/gqqykstyy.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gpmzlcigy.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gvbkimyat.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gqbsnmzyj.sHtML

TS:   name: string = "x";
来源：http://baike.hesvh.cn/Article/details/grxerrdax.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gqhfhrahq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gegmfjcvv.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gzxndlmiu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gejocfpbc.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gogimncnu.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/gcjlqipqh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gohhlypwx.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/guxgygfjo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gfasddxny.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gadpnqpia.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gfrvxkojf.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gafhusccm.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gskogoqdf.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gnkgzngzb.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gsvcazpqm.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/glvurebni.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gafeyqnuw.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjtlwvqpc.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gvwjtkajr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gzubnxgfq.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gycsmlwlw.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gqgjgudkc.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/gvroyayna.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gtnvhvpzw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gywewapft.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/giejlwncp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwucllnrp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gixwidkpi.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gskrzkspv.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.fehbvm.com/Article/details/gdhzclaaq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gegjhhodd.sHtML

[G07] 调用父类方法
来源：http://blog.fehbvm.com/Article/details/gdeoybtka.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/gdlqckheb.sHtML

PHP:  parent::greet();
来源：http://blog.zdbjq.cn/Article/details/gdoimeslb.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/grlfznsyq.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gpbqogpsj.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gfjxykvpu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gfnvkjgzh.sHtML

Ruby: super
来源：http://m.share.hesvh.cn/Article/details/gzifztaej.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gobgixija.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gpyestwim.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gavwpgrnk.sHtML

PHP:  public static function f() {}
来源：http://www.share.hesvh.cn/Article/details/gcynrpoif.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/gtfnzptxi.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gwbclfdpy.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gimhitqnm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gzikplgjh.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gffdnnbqe.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gmnfpxjmi.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gimnxgzec.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/guogocpxb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gpzyexawo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gipqblvfi.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gjonqxiyl.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/glqsctpez.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gsmmkyofe.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.fehbvm.com/Article/details/gjrsybtsn.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/ghwmyzqnb.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/geknshayl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/glzdpnzaw.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gjensxjna.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/guqkdccot.sHtML


<!-- 参考信息 -->