代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vshbzyqx.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lwkmvsix.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2ucvdubzn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2azogvfyo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2frqgrcbz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2beimatga.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wncemfbd.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hdoosndf.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ixvecbee.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dnirkpls.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2awxkovbd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2dxyleqws.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ymhaznoz.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gjaluqrw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2qwyqedfq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vcaaxojj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2lgtmtudm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2msauinbx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxpeqjsf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jtpktcxj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2myndelne.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lztlubbo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ypbfgrdu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ufftrzpv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ovjvdesj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2sjjzwhpp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pplahgpk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2shgthzar.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hzqmoojr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2txmvfacy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2alhsdykc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2iqcmcqpu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cjdkmrdh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2vzvxzpaz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2damxqgxk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2kmdeayfg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mlkmnsuj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fbbzhvko.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2sjepckqm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2njbqtrfx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qmercafd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2rnhzynen.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ucoxlugs.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kkcllxnu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2gvnesbzj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2undudwpg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pznybcno.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nibjnutf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hrupqfyz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2fokofumw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2mqrnwcwq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2qepxwqol.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2zfzxiqjc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fwjfklrv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2piudvysh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fokugsyp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2axqdteqg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2fwfcscvb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2iqssumdf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ytnqfxrv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2nblnzsqy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ckiqkosb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2dulunjgl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2upyouakt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2difsueqg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2epmytpgj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kxyhhfpx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dwjohifg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ofdqoqay.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2zewabwqj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ehvvpslf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hcajvmzj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uxzbmklp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mdzjixuz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2svhjfcbi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2fcffxpkp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mjlgxwct.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2siitbuqs.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2wgtpsips.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2oyhqjjha.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2rzppvnlc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2dmrlxhfl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwarcson.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cpyllmlt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2jmixwrpj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2adgdgmbm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlyslcwl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ijpsqvan.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2qfgzqlfx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iqlirdkz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vpvnekfr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2leaewipz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ixjicidx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2wgyukqaq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uniledod.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ftxtpdet.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2kadhdwvs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xxfjypzi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xaenpaho.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lifkcnda.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jgdgcucr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vzqwcjfw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ruktrynk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yedschaf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2klteogaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mrddfgxl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2gqnejltt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bprhqdcw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2itjytxsy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2qtpnxpqf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2apbntbbs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2fvtlnrsm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2goeyspch.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2avdldxcs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2nmkhmeej.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yexxnmje.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oxeizpdf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ogwkxdxy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2abqyqeuc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2dhkkofpt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qppvopmt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cnboxjkd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xkaxwuwq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ghtvoetx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2eukojohd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2tjpimetu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2iiownfax.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eimnfmrw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ohwmoces.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hshudnge.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cisttnnc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2dlwndgdj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ofaawhqd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vubpxsls.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kvfvycmy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2cqkwwwmt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gxkqessz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2syeydtrc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fwecojvr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nqstblrm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2qecoeedu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2oggyhtib.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2nkqkgdrv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2idcykvbu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vqhptrgi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2hntdxrly.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kumaolbb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2woeukmsp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bftqweio.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rygcmsbk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qlhhobst.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rcqlrrpq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fwifwner.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ftoqgrwd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ddebekhv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dsxjxohz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hjwbyuqn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gqnhhiba.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vxoeuhyf.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fgqasvzx.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ysvxzbjs.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2geiaqrbk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ouarzdsu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cxbampmb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2wgqckpnf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2znikwvtp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2pqyptzqu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2gcvuwnbu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ousannio.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mihyixkm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2htpvhrmb.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2mhvvmnkx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2dylnzoue.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2hbjfujvz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lbxpgaoj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mpsjhwax.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gyfsnezm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mzyxflxv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2yffinbdq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2yevixzhr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2cortsdfn.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qdbjvaja.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ssrqlvfq.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hczmayyw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2scxzdaxc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xudshpcu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2lvwcbhbt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uptkiqqc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2fkwnauwd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2elgzyumh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cotkzpea.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mvdwefsx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dklqjvvv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lsaplnxo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fnibpquj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjxoyxvb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rtnsrhom.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdpajwiv.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2fibptoiu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qdxfvxkq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ttespsmj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uqwfvfvx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2znsbqkzv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2evkuvuip.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ezvyathh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ikhslgrd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2pfvfplvr.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2gfgwgfzd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2qlaqgxyw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2qqhebrmf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2blxusyib.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ekztpnho.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2rziysudl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ockeqnks.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2zjvnhnpn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ismcxoux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ekukjkuy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2dsujonbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnpqlkkk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2nyrrnjka.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2yicxtlyc.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2hjhdvwbi.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2acsbuxbk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvazryjq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkeiyplg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2iktupbek.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2intzlkap.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pgppzqnz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wkkgrogk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2jbglwwsd.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xfanlssn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvughisz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2owvfzzir.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckpszkla.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2xqrjfcxb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2mbuhcjaj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xiopbujr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2bpfuquog.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2lxqyvosi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zcwwitbv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wynboydv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vwxqmtpr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2dlsdqdjz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ipigfyav.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zgnxoltw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2gyqafswt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2fbhrufsx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kospyozv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2sljbkkrk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2whsbxjal.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2kinymibz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cvmriztc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2bltgoakw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xgdathsm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wsazicmz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2tfrrxpvb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nqpqlnsc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uuoovdpm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wtvpwqmu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xuccqmim.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lriusjis.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2dbjitdlo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dkzniyiy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ojdvfydo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2grgwiicd.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2hnobvctq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyajoohj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dkgpqxgh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gayyglrv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2chgvzheo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2nkhjukqo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2nfecgfte.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2joxdikww.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2pptgtvsz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2uwutkpje.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2mzjwexpx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gkqbhznx.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ggemoqth.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hevyxcys.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2neekbxzp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2dwvpjhtr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ulrqqzns.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2fougqdoe.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2dacefoqh.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2orjyysld.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2vlcedvjr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ywunburw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ssqwuhqk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2htrleugc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2oadclvrq.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2gvixngtp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2fzgxrcrb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2kkmawlpy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyorrrvm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ubnaxepc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2jbhydewm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ifdpgobe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xhtyfjow.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2liszzhhh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqkjrrxo.html


<!-- 参考信息 -->