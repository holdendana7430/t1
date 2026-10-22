代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2aiwjhugb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nkgvaqbp.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cmvzlzsc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2itbmbdai.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wcussnuj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zjtgfyoy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ehxdcooc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ledocuqy.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jmekpdrj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2eusdmbew.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2oeentmuh.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mfpneibe.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2tjfgrkck.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2sftrjvaq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2uaesvfgi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qtlmgtyt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2spkzobjb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2demwvyfw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2dfkaprtq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2pmtceufc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2yykzoivr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2kaxvwspz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhyqstbq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2alnjhtmc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2unrcohrz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2srdbuzzv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2cspvnpwp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rtiygraf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ovavqsej.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2wbswhcdr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2rbwqzyoa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2xjvgcqga.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2imundpxy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ruhdntzq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2yrznxneh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2lqhqukdh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qijbtuhu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zcmvatkw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jricwzmb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2picylawr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2egnirbxz.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zpnosvaz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2hbzytetx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oetalmcu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2cmlupcik.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2uxjtrnfg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xxzpnkkh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dpefazao.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2dodnfuak.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dgmljwae.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2howpnorc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wninibti.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2evecveba.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dhgilmnb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2gwiliwir.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2fzlyovcx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mrshjilv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2pvvfefex.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2uynmxonv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vkyviopp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2kqtytyev.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2kmusiwfu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qxuknksw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2drjqyscn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2dugjaezg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2akkqajjp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2fiqjomke.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rgxqfcxp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qsvpqivq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2egptxmkl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2buwmfasp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2epfafibo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bvlywkwn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lddqbekl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2bcvfkzzl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2nepfpqkd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vllvgwfl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bcbuwuwr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2lctcnqdt.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qpucgvrk.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yglcuobe.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tqcezmif.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2mgxhddod.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2oincugza.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2bndohete.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2bejyvata.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2gseejwmm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fckhlhey.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqowjbag.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2rgulifve.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ivmbnels.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2piraeefe.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2vanbqhph.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gvulihkb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ehabpexg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bvzfgggs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2umimuflm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2bsaqpnfx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2grdnlsxc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iyhuuvao.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2kpcqslto.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oaicfejt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hbkepvzp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cssbwpob.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tmuzzpkg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yhogttfu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2lsjujmtt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tjjhexuw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2usnaiafq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tcptoevy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2kxmklxlw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgrsqvax.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lffhwkmu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2vdvvempf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yvcthpib.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ivdpvzna.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rqicnrnl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ahwsmwao.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2jcidmbtj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jwzqhzeo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pmuakhkh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2uxqdprrt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2wmxkoelg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2htgawgzp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzhyvayz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azveeyqi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zfmxyxrg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2squhsujy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2yyjpsuly.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2byipsvur.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2rrwmfbhj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tswwtypa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vdyrliyp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lydcxhzd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mnsjncue.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zvydwpzk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2egbgxvts.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jbuhpsmc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ufdfokdc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2osohpxvz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kmthamvz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2gaqevosd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2slitxmqy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ibbubwoo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wwzqweqe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gjcouwwi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2duuubizk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gyywnqlh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2esengeuk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qmxdbukc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kclpiane.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2skoygnqk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cydyrcpl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lzxwcdyv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2onpebdju.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gpitiyqx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xiicakmw.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2kgfcrjpf.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iszhafyp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yncfeqzy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2varnhvwk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nodqjlfc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xdzinwbn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hbegsmvx.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wygbntsq.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aigrtrfu.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vgvnvmlh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tffssdfz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tujiqdav.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nqyxtgez.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dnnkzvgf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ldokudyr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ezvbufbx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mkaubyfn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2kwbcwwvr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ppvizqkh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ncgguevb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2uzlyhofe.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lqglzzwm.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ludpmhhd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qysdrbgw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bxrsggjp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2fawueoqt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2hprmmdla.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jdhrdhiw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2frdzofqk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yadduzhb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2aibsnzrg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2yvnelfwa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2druikuvq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ahokeiys.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xdprjhjo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2rpguiqhd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2roqryosz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cwuhjewn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jpweipks.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mbbqltph.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aluvaehr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2kwxqebqv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pagooiog.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2traqodag.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nddvhgxg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dqbqathr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2niinjvue.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2jxtedgyz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nxblokco.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tkuswkfh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rlgbxnkd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ywrbhckq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2iccarqiz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2kqntmioc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2phhximmn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2naxzvhpy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dtmyqczu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ztcsylzd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2mqxgshjx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2gzjduwvk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ntjgtzyv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2liwdgjnd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ubstyohy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yfbqzfbv.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2vqbyywiu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmjrygmq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2fuvrptnl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2najeztzy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ofvjixwf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qouqzjln.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2esinzvwg.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2fyuemkmw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ghqdnqqx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bcfklvhh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tgsoiufs.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2cvtkxllf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qgozouhu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwveemvl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2chtxfyvl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xlbesury.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2biiwyisi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2habwdeuy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2avlfsvlb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkblnttg.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lymezocv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rhdxuaop.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2koladvia.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nydondwk.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ooihsktv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2tzvpjorz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2tmnqaonr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jhzixtea.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2utivxrnz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2oroeequu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ffthotkp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kgckjjbn.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2aihivuls.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsqtugrr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tsdqcrgd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xyyzhagq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ngyfhiub.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yrnnaynh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2jxkgotvm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2fjviofeo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvmgruck.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qzzzafol.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffmzqnuu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2saqccoiz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2dcoegonq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vhtmjjyo.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2myuewnou.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2zxdedliu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2qantikxi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tyxulizq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2erbdzwme.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2urcattjf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjmxmhyd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ubplocis.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2yuaajwzk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2egalbxny.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2vomwpjiy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2pxexmksn.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lupagamn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zeogswsm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qaibzlhb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2owgpxgdf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2clbgwubh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2orwbkmxs.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fuvwmrna.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2rnfbofgs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ntcqbqcd.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2yuayhghc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2vmgfabjd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2kmnomgcp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gstvflrn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2hbnfgjnj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ghzldewo.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2azeehnmr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2rvqsyqkw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2mjdjflck.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2nycxulwf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gcpcfdbb.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2adkollse.html


<!-- 参考信息 -->