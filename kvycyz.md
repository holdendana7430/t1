代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2pftrfsbc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tjskwood.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qognqydm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sqnmarrc.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2idtyawky.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jayzpwgf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2yjkjmsvx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nmaycvum.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tpdisibe.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xeowmjas.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2eaafkgnl.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lozfldjz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2fencgndt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2feibwrae.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pabakatk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2usepnhip.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2pmamiczu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2asqfzkyk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2dcexvqil.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2lirpmuzh.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fndnhron.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2osauilcg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2almmtnti.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tsttarud.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fzftdzln.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2iuulhtsy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2mhvoqesw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qpxnpfuy.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2vpnzhkzd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wlwspohk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zuvbxuxk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2wazyqfpu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kdlbqdaz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2kezdpegc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jboybbvv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ogucaadm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2esnrbsjm.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xzavsdvz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oczyoips.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2dkzlvrpb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iwmzlkhb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2aqyswdfw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2sejbtlgf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ipwqdupd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ifxfimuo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2oszdndna.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2degsppyj.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qkhgjmdh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2xhvgbttr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gikcposi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hpojbjpw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hzkipxda.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wejjnmla.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2jerxwmmf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2apxerkmg.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ppsbhruk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2kkksjemo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2thiyjojm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2iuegncwa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uxexwfvl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2tcjbeqxp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2uuhtlsyz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2pjddgsgh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2qtlewlox.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hoeuppmw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2jscpxyhg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2hpbmkxbv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dxuxracq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dwuvewkg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sobpdbfx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lgzzdnai.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2xyruhlkf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2gbmvtzka.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ufnegmpg.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2mmlvqnhj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cdultbqx.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uiryllqw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2glaogytx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2uqcerlxi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ljnkjfdp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2uwyjuwav.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2wnuizini.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ejnfkcgn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2otyvgvsc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2nmazusig.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2redtfuvg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ohfyiryv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vcxcxxln.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2uadgebgt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ecobwwjf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrrktvjl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ghzrwgbv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qxntmcqz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yitrbzhk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wdxmpndh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ypxwzjvr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gdvyvbdb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2srgxhzoi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2btholtvw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jabrsadx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ivykvvtx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2kxcecfmm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wpcvpvci.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eavxqpes.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kilhwmzg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fnauzhix.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2tbgpnqwj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iksxkgvy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2upaexzpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nplyrzxk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wqgcejlt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbgsktkc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zcogzqlw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2gebtfezm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2awpjksou.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2afvumdgc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gewsnuge.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xvkaokfy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tfbhtldr.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2plxxugzk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pyfsgdnv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jopxaksb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zycnbued.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2srlmslkc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2tmxvupqx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qibbflbs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2aowkweml.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2mwurcidn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ddhbdeuq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2dezqhnfb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2xtzvbvbg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jnnaoblf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2szvfriog.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vwrtkafy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bxdlgvbt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mmtpqlxg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2xviukwkp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qrdyppft.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qrglrsmq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2whddwwcm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hprkmvuo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2qsihatpc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2looyqshg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yitxcmsp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2enhmqrfs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gbllsevw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2eozvoxgn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2czpfndsy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nelomohm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ehpojoeq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uctvdjni.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2brulhpga.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qqfsdqqv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pmejwldi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2pykkozqg.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gqsdqsiq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdouwdii.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dqiywcuc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2krlhgsmr.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ahaevemr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xszawfjy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gqhwwxpb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2csckydmk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zqjsnuhk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pajnhbmq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oyifpsnx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qbkevrxi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hgvntzzo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vllbawpf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2whxjzwnk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vkooihjk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2crtosklf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2znpattkt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2zyidpkgx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2jpirnioq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2pmdpfskd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2asrahcwo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2fcstrsnh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zaoeyrtg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mhaibtmr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xmvonjml.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vbsiityf.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2enedwogk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fjmilreg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2kefueugv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2znjrrnsu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pusfeven.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ufqyqrpm.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2oaqntqyd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2binkkrhv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2fmabhelo.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gccbovfx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2nesqtmoh.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2oznxacue.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ffrnlyqf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xisrlveh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wjfrtypm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xdxnhddp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2lesohxsk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vocxclrh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqasmyhz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lufsqdxc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2fjvpicdn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kfglaaho.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rfvnxjmq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2poaczcjo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tllkdpja.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rtmuljja.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2zcqbkdal.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ryhxcdza.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2bqzoxfwd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2chmxubum.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2vqlojvxr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2cyylriir.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2zmgshxgs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qhridstz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2yfwzjhrw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2odedjzos.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2azfyhund.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hwqbewmb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzhbnpfp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2cqqmmsmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ppvpsjbr.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2iqdfaocw.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2gpdngioq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfhkhexh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ukhekvaa.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2qddswciq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkgypdev.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2klmxhwyl.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2qxjiwkff.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cabgkefq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xjlfjadg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2jyxcwxrn.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2empsmbjg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnjrbwix.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cyfrqyyx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bdelrbfe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2cbwxzmsi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2shqtabsz.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ciuzbbqu.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2fgbmohug.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2oqhvdhxz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jcxgrenr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vbftzebl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vksrnjnq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2lzfjqmwk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2kqjdpitt.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cskcvlmy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gzyakjin.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qlhwefap.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2uqsnppsz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxrlorlq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2brtzjtmu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qwvcywjv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uixsxytk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mjoiydnn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xmqhzomt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fhfcphwb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2eiuefwuz.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dwnnseye.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxcnpxxb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ipkrodza.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfsxafmt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cxpgkuqz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hjulzred.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dpahynao.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuttwkfz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2mkeoxxqb.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2yiixycyk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rslwrccc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kjsxfcyu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyguuigk.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2amnewrqx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2vjplhnpd.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2gtivqkqz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2uqbxjvur.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2pxzuzwjo.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2bhihzcxi.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2djtgwwvy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ywrookvz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2miwlqvvr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2umdopzzh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2hvtsdxds.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ntpxsogi.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2afmfnvak.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2ebgdsqge.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2ynkpidqk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2efwhvvfl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2kwfoirer.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtegcwok.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2tdfrfeaa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2fushgpga.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2tdwklsth.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vnspyupg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2habosapo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2sdzikdam.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnynzpjl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2iqwvwjgv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ssarrhtg.html


<!-- 参考信息 -->