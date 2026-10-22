代发 wailian999

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ourjwcxz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2safuewcs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2mbnxcuez.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2yqipyccg.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2obakxyxn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2owuhvjdd.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pwpoybzn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2boqasxvc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2czaxcmrl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2smupliix.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2vanfclht.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2hfviwskl.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ublindlm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkencuii.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yuqgbpzx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pecjefuf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rbldolrx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lzkcomvb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2aiiclpsl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xvzwypdl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2osvbqsgm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qnyqruqf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qxxzslrv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qyzqngcc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sddiqkca.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2adsgdeaa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2myiqodzn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2igmrhxbf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uevuknmo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2coeejwvb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2kklnjbdf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wnwwptto.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sdfkaxrv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2jhabrlbf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2wauwbpij.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmqbopqj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2spdcwpoh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2avmfrnqq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2cwkofuet.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jwcabukj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jasdvxbh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2oikmcprg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ardsejlh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2esljtaxc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2eckpnqzx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2drltnrlg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hgrgaqac.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2viqmmnur.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2lhhacluo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bzkllkwm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qpkzhtow.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vnjdpapt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ljrnnqou.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jjnftlen.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zmhzmjua.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2nowyzbgl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lridqoit.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2snushhae.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2wpulnweg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fmdvmboj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kxrxgubi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gfxgmzdw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hhungkws.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xcehllnf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2wtuxkfgl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lnhpqxri.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2shasyrll.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2svivmray.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jzdjvpgf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2oaoftmkj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mvwlsixm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2kdtfhzqj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2heobdqeq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2wwrzndqd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ajeordqg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2hogpolne.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2wrjizcky.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2nxyarbvg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2buubmphb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxfwevps.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2znnrdsfm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2exhsyqtf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqjlrqxh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2rmiwmdux.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2yybqrbrf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tfkmfbvg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ewxzbmgq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yxdasaeo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2avzfabny.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ujskujla.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pyjxvrby.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fqosiypb.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2zlqblrvx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hpezhuyg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ccfjwkey.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ihnxagzt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dwclwmof.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gzoqgqpt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2vyivtelv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lmvcorxx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2oqilflri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aetoeyql.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2vyeggmdr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ofuaexzu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2syacwich.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2zryvefmn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pwyosrkk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2nguqulzz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vuykaaqo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kipsullt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2lmpswtwp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xwscorok.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kpjpufsz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2wovlvgwt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vkvxyazk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pigtzzqv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aturcguh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cycyfkcn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uviwcjae.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2hpikyeow.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2jsiwtlej.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2wocgzegc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2rntmvggx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yxkovmoj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cjyowakm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hqpqpjek.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qldetovy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qqtvzzuc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2qzlomzjz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wijphcyl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ztnlqfyt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2oplbhaon.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sysnyfwm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2oxpcomeb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cvjtdzdk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nqteoaka.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2slpkmeym.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wpxgacnr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2vtptezzr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2iptgcrof.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2sdwdetzn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2oionfkkn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2egvvdudt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2plovqcps.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsuurlza.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nxrmyfys.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2cospaqht.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jntwlrrn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rvamjadt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bjbtvkfu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fuxxihsz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kjzlqzir.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dmoxlavu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2axpsobgf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sefvxquw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ejcbsucv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2itsiodiw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rqlbbqxc.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2efxqbtrb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lxbeixor.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ggzrlgpl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2invgwiwg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fxjsqbdc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2yfumjhzt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ofkpvhpr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2vqznsjbz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2skzwcpda.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2gdixekxn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2jgxikall.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2apvkxpzm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2usumbqra.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rvxczdnf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2mazxdaau.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2exzmjucd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jlbtsauk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2goowrhbn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2bbzczagm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sogtbhtw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2imshruqv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2xzgyuioj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2tpflfbox.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fottxygg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2slevxegs.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vddspqzt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2pjtkbzxk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2xiwvpbwr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2brfjyqeu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xhskwhdl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lrohmkff.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aczbimpq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2kfgtnkwk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wnlbkbeh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2twrpbuwb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kzemlmke.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2eacabadh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jbbbtsfa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pguovezv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2slsecalk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2caygrsiz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yyftuijg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2zaibqpgq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uimajiju.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fjgjdprf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tjserenj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rricovps.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zmfuavoz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qetqdclz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ttrwwjjb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2kwobzwps.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2tfzocrqi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2dhompcqy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2owtlutza.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edpenjet.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2oqvzafgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cerxkghp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2iwolpwmk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2xismyktz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2qovyyuhd.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hkbccibi.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2tklgobzr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtfoudkl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2omwdltnu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hskbyvnp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rhjgxdqi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2bxzxghcm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2vdclpvdp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hhfkwwbg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rcmexotf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gwatgjgf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwenphpe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2osnronzg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cbhhmbec.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wavrfcfd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2boltljsv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2wolaxjyu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rsrbkwbk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ffdxiyhp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2yzjwydtf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2epwsocut.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2fgymuuhu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2eozqzsvt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dnixojyp.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ulqfrlea.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2qzfeyeuw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wgbnvbpz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2jeqejmfy.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2trwlpssc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wfnqbery.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yiwghtln.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qxadsqka.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2aiqbunqp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2cwvmjjqu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2dqxwgkpb.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fainvctm.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uxanxewj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuarkmyt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnxioopo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2ripnbhch.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2nsnmkjhx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwssifor.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ouobdsrw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2bwfxclvn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ztthokre.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hdbsqgyo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2kbsfmmtc.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pqnvqajv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jaudagyh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2jdwsxbty.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2dcyoaflh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mcqcxulb.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ydgvpmkq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2meljqbja.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lngeghzl.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rrcupkvw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ecbwwdha.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2urmstscn.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2wkskjpza.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2puumzxju.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2atzpzoil.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2prdwplsu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2viqsnbuv.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2jhbzodoh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2enzezcqb.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2phiwgpes.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2lpubcfox.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jiuecthm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmdinbfk.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2wnmbprta.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zzwdsacx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2kfrkmalt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2nvrepryj.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qevobmya.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2hzkdshwt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hfoeymhd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2pwffgduz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhgwdncj.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2fjrqarrd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gfrcoeso.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2irlpnzks.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2qchrhqfx.html


<!-- 参考信息 -->