代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2xpofdhht.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gouglrlo.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2krlzgnak.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hczemlgp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ytxenfjl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wrrymzlt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2zuaiujih.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2yphkrfpv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2iwziuvig.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fhmaxltx.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2dprzcgzq.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rusdpwuy.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2lwlzvmku.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pipydund.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qtyfdkvd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2pngejzuh.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zgdstnag.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2usrnthnb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2yofjhbng.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qlypitcs.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2xrpevjre.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmasyutd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qzolmsgp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kqhnkybo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rwfyknio.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2mrmthncm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2tpgxsplq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gjjggcrr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2kvdgawpx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2glkuivdh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pyipoakj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2yahvefts.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2epgbjizv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nkxcufrv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2lowfkltg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2cssdsweq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pzyqepkd.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2trkygrfn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uofuzldr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2oqjsadfx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2flgcrojz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xpcyeygd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2lzhuvvmu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2bxoonvel.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qfatenme.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tmijogpd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2kymwtwqw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2exwhifsz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2uawbtkow.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2sponiqjv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ushibtmr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2muqdgahm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2xcatkiyb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2btxoxgyr.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ymtysqjy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2nkhcqnsf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mcdjvfkw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ooqrbzts.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xttdzmrw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qefvoadx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2fhcldniv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2apkxunif.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qjalsgbz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2odiiryjq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2aoohdmic.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2prbustqh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2zwlhnloo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sxbkrrzi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xcvbwhip.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mdblbtbo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bwbwgwpd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mcllcniq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2offozgfi.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2xqhhwqao.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2gcxbelvp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qzawjolc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nbplxbgl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2faeznzrz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yfuezizl.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2fevnvkgs.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2jskdtubg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2axdhhhmq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2oqpftzug.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2vxdhavpg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2tvpgzqxx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivxmzzdt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ariteatu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxtsgtds.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2kaaiysba.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2vuvzjgji.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2nwpvkggj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2oovglpnq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2xjzctnbr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dppezdic.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kkvohkpq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tmlnyzlg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cythmuqs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2dinjuagu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2leilxmpu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lwgvvlzw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2chmzctyv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ywqfjcft.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nwpevaqa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bbrmehzj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2buulqfqo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2zpzehkid.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cxolrern.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lzyodxsp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jwyzsxbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bxckncto.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mzmfooxu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wtogateo.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2tahuirsp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2sayrcnya.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nfcisiey.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2eokothvt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tatohzjb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nuhopjqy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2yfcqhyyb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tqtznamb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bhdliivi.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2tslpengl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2rxzwwgeb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2lythlrpw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxkzzvjs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2omsemuho.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xwcpvxyy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ipskglvp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2bzaajrbu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vkssrley.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2mueaxlzf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jtxywuxw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zgemuoic.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kawpxssx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qurtanes.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xkocpcfk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2fywcubbj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xxnkrpgp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jwxgfanr.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2jdmzlnrk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2eokoavgw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2uopvnhbd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2crgxgwye.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kxlnuuvs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2lbnnasky.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2lzaylmog.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2qbjxpnys.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2iuodkont.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2svpfvsru.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2iqqrfwua.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ivtpljkw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jjjwytph.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lqywndhd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wxfohfng.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rmettjve.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bgbypequ.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwqtjzon.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ehhvoggu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qcdbmymd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cruuwtcx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hplsxatq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wpbscciu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xvcstxip.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lqiditeu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hgtnqtiq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lvgycswh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2qscltqzx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2aulntaqv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jtgkhfhq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ycsxsgec.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jblcddfw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2cmiphgrq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nsustykb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2kyrocoqp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xmuhgjwc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2janpvpcp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2tjmhzcoo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2rloalsll.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wgphwhso.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ugbsolhr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cixhtvlp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vmrwyyww.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ofiigmow.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2yjuxalau.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2xxheudai.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ozueifrx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zrpjzmpp.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zssaixxf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ffjrnfwx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dlygooel.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2btozbgae.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hqnejgjo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ogsfalgm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2wmpwymrw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qnfmlkqg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uawkqozj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhtwpsqi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vheirapm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2kiehbiya.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2llgtcgtq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lfsmkpaz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbliqulu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2kcvcgwpb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2emkhsnyh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2czidgpve.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ewyqwwhb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2typbossa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2puvjdula.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2dkrjhqsa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cjfxyslz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2fzcqgdkq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fqtvbjna.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2nsepnhpy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2ixddqkwm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2myxdfjra.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2xgygmxpv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2rzaqjjlz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2uuhqcqvu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2nuugsemu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2sfqwndel.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ngyimtiw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2bkbczxsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntmehfrx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2mybdvpxg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xdauxarv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kqrnazyq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gyaozpot.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2hvmrxkiv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ygpqehss.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2cplxlenl.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2slglhczc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jhtdtsay.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qggrnyng.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2stfrozxe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ljtawpmy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zdrkvoct.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fikvrtoz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2frouenio.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2swyhlyuj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2wjdzgbdm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2abmilhhi.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rkdjzuee.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gybnozqy.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fbdkvkdz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wtcpxiyo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ydkvlcbq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2kyhjigey.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2uqadfbyp.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pvqhpfgd.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pvgojnbw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2rjanqfux.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2fbsvzwvn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxbkjhkg.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuirvafs.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yfetesdg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2guclkthf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yhcfibse.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zqadhuhf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2viuiftye.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2yezvsjaz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2cosexagc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mopzmslw.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bphdisbg.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vvdexazq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bjkcbqzh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2oevhcwce.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gvgzntlo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2mvrhypgn.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2hftqvnvt.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ziuxoinn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2exbjeusf.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sbeijwod.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttjhpcsb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkcaarlg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2xqkuxhym.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2litcbgse.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2racxqomz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2rbblddqj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ubvbynkj.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ezokppit.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kfhtuttn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kwpkxsuj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bzwzsmmm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2oiqmvgwl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2rfentlyj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2zjopabxj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2zbunduno.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ydwlqynl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ctnxpzpk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nithzsie.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2niwqtyph.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2reowolyx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ybwhfkrg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2vjhmvaib.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2deescjdp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2dznqfyjs.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2pzbvsfef.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivhzyhxe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2cfiaihwe.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2cqhsvjwh.html


<!-- 参考信息 -->