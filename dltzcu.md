代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2qmlzlbqi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wzqqixgx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kdlmvkiy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gujldyem.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wnqfvqxp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2veugcldn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfwgpgxf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ohfupkic.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqfmzeif.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xnowyadj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2rowzyauu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2beebmkar.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vcyjegbe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ntglwyzc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2mrcgbkgn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2lnkrtyys.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2xynlnjss.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dciuxyjk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ipnyyqpk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2hxibsmdm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fxnrcguc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rbfivpqb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2hcscjhet.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ktyubnwq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2vzybepon.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2krniolgj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2cfclulfl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ubwetutm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2jyeznwgw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tfgjufzn.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lokevtoy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2bebfgmri.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2tkhezkhl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nnffjjrn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wgmhqhsl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xbiingel.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2stkkkqol.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2igmcotsh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xwlrungy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2fxnbydss.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2isdmdxjq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vjoxlgqf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vlqweavk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ielvbcyg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2heqlbjvr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2hlluqnim.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dcfernya.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2spakixvm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2tpznpmkp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2dhuiwuzp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kunzostr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ummdbaki.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tmxbyiuj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2otyqbkth.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xbccstoh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qadnwryu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ruybbrtj.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2zkjylcvm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hftgbbbq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fyvizstb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kvboolqw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2iovqfrpc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ggllkced.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2kpsjfenr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2xrzllgsx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2feyaxyud.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ltvyoaao.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ainxbzvc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2fzxpjvne.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2rskuejgv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2euonvuuv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dyyssmra.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2bdnyayyj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2gfesdsyl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2mtecmcie.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2cauxvhya.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qowsaery.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mglxqaga.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2suxcqkgc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ngqtferf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eyohujhq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2terlipzc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nojbjrma.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2atuyxprk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2qfeyosdk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2yaxufkno.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qjftjylv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kiooeopp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gxrxysqb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2urdebxng.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2haclawhv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yogcvkpm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2tddmldgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzisojdx.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2awvjuyhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vznjypqq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kyubqffu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2yecbfxyr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zcooljhx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ehbmwodw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2urvopjdf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ywmlywpn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2bclckvpv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lxadudjh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gxirppqb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ubmqegcx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2nfjlndyq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ellknvav.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qpaflyxe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ehjstyfo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pvhoxppa.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2jrweukod.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2dsjkkcmk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2lgfbgcpn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2brloijsu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2shqhtlyn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nsavkucy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2snxmazcj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hdpihtsc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fuhepjif.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2crtsqszp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sdsgjxbd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2yqcoucpq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2oqobdmke.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dnodnvtk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jduzhftb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2sfdpkton.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jwzbideh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2gpwxwcfv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zwjxgbvy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2eahtrzfn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2inzxxeki.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ozxqvmju.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2tgnafsdb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hhfhvzva.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bwktblni.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lbqscfef.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vocaqlqm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2sndisakc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bysqmmdt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gijviivp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jnwhikba.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cxolmzfh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bepviasy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bqetiqhs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fkylhuai.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sahayzps.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewjmfein.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xzbsleij.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wvfbzezq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2dujtfyvq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xvrcqtgl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ftjjrjlf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hwcusrma.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kjsdxqku.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2okmdbgez.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2oazytqba.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2gvelduwz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2uzkvczqr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2lqomhwop.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2sktksphf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2owtmimho.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nxrtzewm.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2prpktkvn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2fzsxyqyf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qtexmtyd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jdoiegbj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vkadxmxl.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2bufodnwh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2npkxoqau.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gafkmoso.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mhdgsnbq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2nkhpuxfy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kxikptfv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2scaaxfjk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eygkfqvd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2mnjpelgp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2axcltfmb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqisznhc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qylhwhgw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pkjogybj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tyodxogc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cddnabdu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmxidttb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2csyflqkx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yuuczrnp.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2zgfvmfpu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2amdfmjxs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ppzvuvdw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asjvtpgq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rmpfifhu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kaigjrjt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jnnhasvk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kjqskfcn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2hkvpnjma.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2zxcykqfl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2nwevydpd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2tvvrfztx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qxkafdje.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2zqgzxivs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2pxognygv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2sjjbwfea.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2uyqswtkr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rorxsugi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahoctzqz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qesyqryz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xrmxgaua.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2rzyzrhoa.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2cbxgcilb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2jjfynlgw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2akpbghrv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2tfqqqtmr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovxpysoa.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2pxpvnwsw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2uwxunduh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2issprfiq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2caymcfzh.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2jwffwymp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2klitisai.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdgehrik.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkannnsu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eclutite.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2wibagzir.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pudlvjnv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2emtstjjm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2lfwluayh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fzmopvab.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sqdhxckv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jikpanov.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ldyddaus.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2foomilas.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2dgypmjcr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mbphtjbs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2mocimahc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2cjhafehl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2dmngwygp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cdvezzas.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2oflrdcgj.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2adkorehu.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vfixzygq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wnsrrmxm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hmnarfox.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xvnbebjp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2nsnzaxhz.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2acfobiad.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjbqtqos.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwpuiqao.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gphtnmqm.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbzniwwm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qoajuvds.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2azbrtico.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkhrctvy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2dytisboh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ggspkfdf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2oiiilycb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljlohvin.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cliadegr.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pxmwbzcr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2hvoqvsoz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2lopztypz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2lofepjoc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2xhmpybiy.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2kckxqeqw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pucwvesx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dbtgjlpe.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bunhzfjk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ghwbatyw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ahtqnsiw.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2oenxwkfy.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2gucdigtp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2zgexpzox.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2rfmeqhju.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2xcwkidue.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2kqtxkqcd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2tayjbwic.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ecsyiqcs.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2qopehnhm.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ktgaejel.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjdgapuk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2pbsyrssa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2vnpjxezv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvysngvs.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2kvwyaarm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hhtjbfbx.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wdvdescl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2akdalcdt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2jvqoxvhn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2dteyrrdp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vzgkmiir.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2rxipjxpz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lfkgkueg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2wxkkrvce.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jpehmcpr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2boakjavq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2crjhvfje.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ssevqtyr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ofshfxzt.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2cfyzutfs.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2kfzujpwp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ydriwkjy.html


<!-- 参考信息 -->