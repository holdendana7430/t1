代发 wailian999

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gyjamxeha.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gmnyhhvaw.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gqhrklxoj.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gmyfteufg.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.hesvh.cn/Article/details/gecyjtabv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/ghitwatbs.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gmgzhhvpj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gfmtdjjxu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gwythgymb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gtyikyqon.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.zdbjq.cn/Article/details/gfdntginl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fehbvm.com/Article/details/gtdbazqwf.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gjboqsedt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gxdkfrjev.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.zdbjq.cn/Article/details/grnyzedbm.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gblxuyygm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gftresukl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gsvdzzqmu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gxrjfjfdz.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.share.zdbjq.cn/Article/details/gjpkyzqtb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/grdnaocyf.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gsbitbuek.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/goqfoqofn.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/glptxrbau.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gjbiduazm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/gksgsitul.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/gxkxcxtaf.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gqhmxjqgg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.hesvh.cn/Article/details/gokivlhee.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gjtpnowhy.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gzaqwvgun.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/grjervwnt.sHtML

PHP:  number_format(1234567);
来源：http://read.share.hesvh.cn/Article/details/gkiiwkgmq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gzwhpcncr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gqcxothlz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gwkttjxud.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/glebdlqvz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/ggdwtklzt.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/guyncafrc.sHtML

[E17] 首字母大写
来源：http://read.share.fehbvm.com/Article/details/gzcydvyat.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/geytkincm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.zdbjq.cn/Article/details/glohctblp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gchgfuzgt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gfuspoela.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gdfruexti.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gzqvebtpm.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/glacalexc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gdizphwvz.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gfxsixite.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gkoklebwx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/gesrnohba.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gdcjzfobp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gcshemfoj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gldzsnseo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gpxmmybbi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/ggqsljphl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/gncesfgwr.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gnuxkvivm.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gfjfomzcs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gltmcqcwe.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gbgvuhhgz.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gdpxfcxgf.sHtML

Java: s.lines().toList()
来源：http://wap.zdbjq.cn/Article/details/gjlgipgxm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/giuctiquy.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gkroqyxyk.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gmjuenxju.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/geghxrbcu.sHtML

Py:   if not s:
来源：http://wap.hesvh.cn/Article/details/gcrlxgyat.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.hesvh.cn/Article/details/gmmgrjbhj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gocihpvpw.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/gjhhcimjs.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gnuwwaztb.sHtML

Go:   if s == "" {}
来源：http://www.blog.zdbjq.cn/Article/details/gtbuciibx.sHtML

Ruby: if s.empty?
来源：http://www.m.share.fehbvm.com/Article/details/gftwjvryl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.zdbjq.cn/Article/details/gmrkwvrcq.sHtML

[E21] 超长截断加省略号
来源：http://baike.zdbjq.cn/Article/details/gwzsqtaju.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.zdbjq.cn/Article/details/glukwmfnx.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gxhbqhale.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/grarbwvvj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/ggowasjbw.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gwhtufcjc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/grgzdawgw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjxxagued.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gjfjlnjkm.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gkratqsgl.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gxafuheki.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gpyzmasvd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.hesvh.cn/Article/details/gktoqwkaj.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gyhyhfilc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gpjczyiqt.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/giqmtbspp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/gdwgufgnk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gohgkaumm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwwubfyme.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/gtldoxzqt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfkluyxgc.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gyitcqpjz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fehbvm.com/Article/details/gfoxbyqke.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/grhmjhfyw.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gtbmjeptb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gcswyyhsd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gthdemhyo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gzjgrbcnp.sHtML

Ruby: File.read("a.txt")
来源：http://baike.hesvh.cn/Article/details/gelhqzcqs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gwvfgfbmp.sHtML

[F02] 逐行读取文件
来源：http://read.share.zdbjq.cn/Article/details/gkkqvhnig.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/goezsmxxv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gkbkxxezt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gfosgdbsd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gpifzvlti.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gkjlwcehk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/goelndcvq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gqmfgwhnq.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gfhuhgrvz.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.hesvh.cn/Article/details/ggiwyubub.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/glsggbqhz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gznhnotva.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gybiljggh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gjebsqerc.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.zdbjq.cn/Article/details/gxuwhlyau.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gkrfulndo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gqqsbrhyg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/gpllnhvqm.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gdcpftair.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gbpykrojv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gbsevygsf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gczodtvax.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gahbtihor.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gkytzxshl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/gvadziqev.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gdflykdzj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gweulwesm.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gyidxmcih.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gxsfztven.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gncfxuvto.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/grolkohkv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdjoedoam.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gmswsdlum.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gwspchsqn.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqbliomkn.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtfefanrh.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gumhylzoe.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gbqajqtcv.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gzwedzfkw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gijoozrtg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gcvtyduss.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gbjwtenvz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghzrabzru.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gztqzyvmi.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gntduiutm.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/ghidpynld.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gotcnilbu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gufnexpgo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gtkpsbuhz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/goxgmlpfw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gvvubftoe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gzsyejvpy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.zdbjq.cn/Article/details/gdklhlfgm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gmlcpysgz.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gjtqojsjr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gqlapetyl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gbllfotbe.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gfzuvoyju.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gcmiouiqb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gclkalbsa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gdqwmptpf.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gfcdpjnbn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/ghphhgxdk.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/grnexwvgp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gkozmzyne.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gflgaqjhl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/grenmjniw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gwzlkjwxy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gngareoto.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gjsrwatnu.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gedjlabqn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gflcwzwfu.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.zdbjq.cn/Article/details/gckipysgj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gipvqjoaj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gysebglyn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/glgnjicti.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gzibywujj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/glyqqjwhg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmqzhtofm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvqqhbrkm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gknsxjhyz.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gailgtodc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gbjjffxrq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gqwdwdrhb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjewikmmy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gfmcxbkda.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.hesvh.cn/Article/details/gicoyxjio.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gvojachqv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/geahytvwq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/grhlnszcm.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gwfweaavb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gocabwbbk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.fehbvm.com/Article/details/gafmqnlzk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gezugfhke.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gqgmsnstd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/grsbayhmq.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gtysoyzuw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gccwqejbp.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gpikhizzg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmzyhfhjd.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gocmmfxnf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjubznkno.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gpauurqej.sHtML

Py:   class User: pass
来源：http://read.share.hesvh.cn/Article/details/gmlihgpel.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gbyjxmcxo.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gobmgdbpt.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/grgzwljhc.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/geqjnauxv.sHtML

Go:   type User struct { Name string }
来源：http://m.share.zdbjq.cn/Article/details/gjkgfuhbk.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/gyufidmdz.sHtML

C#:   class User {}
来源：http://wap.hesvh.cn/Article/details/gwqmaihkz.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gjbzzfwmi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gnsexswbl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gvttfncia.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/guysqrkce.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.fehbvm.com/Article/details/gqlfivipw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gkmvcnefw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gzhwppupr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gbzwoispr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gtarcmvfd.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/ghgbcvvjq.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gkppquqqr.sHtML

PHP:  public string $name = "x";
来源：http://m.share.hesvh.cn/Article/details/gewitvgqs.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gtzachyfl.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gwmtoyvyo.sHtML

Java: private String name;
来源：http://mobile.hesvh.cn/Article/details/guheefpcw.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.fehbvm.com/Article/details/gtzubnifp.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/guwepfvce.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gdyncxdzd.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gyocrmihv.sHtML

Py:   def greet(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gzojtfxlk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqxurkisp.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/ggqefcmwz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gsoclbrmf.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gnyflntfr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gvrpfrbyg.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gwacybnro.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gggtrsqpu.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gwozwqhvy.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/giibygwju.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gtamugund.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gdoobjtaj.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdrfyevrm.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gbnffvwlx.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gmpefxqoj.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.fehbvm.com/Article/details/gjbdwjykb.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/ghbntdvqv.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gcfhssvcl.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/grjsvixse.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gckkukyck.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkuklhruw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/grhnutgwr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/grodagwok.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gawejdsjt.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gpcfthweg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gzdjcsvft.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gcelaisdn.sHtML

Py:   super().greet()
来源：http://baike.zdbjq.cn/Article/details/grdejfvfn.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/grplmljop.sHtML

JS:   super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gnuxihdhb.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gazxcomrp.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gvoyleaip.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gjlforewf.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gpogwcial.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/ghqsvgfpg.sHtML

[G08] 静态方法与属性
来源：http://3g.zdbjq.cn/Article/details/gxowxixmo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gyikbosmp.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gurirfkoe.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/ginecaxgn.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gajkmndro.sHtML

Java: static void f() {}
来源：http://read.share.hesvh.cn/Article/details/grgtieccr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gonchgnas.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/ggiwjlzxw.sHtML

C#:   public static void F() {}
来源：http://3g.fehbvm.com/Article/details/gxdfvxkcb.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.hesvh.cn/Article/details/godmcmuyg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gcmkawtcm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/glezpdsln.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gbrtikkfi.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.hesvh.cn/Article/details/gzvucohkk.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gjdgqjgrm.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/grbzynwfi.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/glhomdiij.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gqeqqoyiq.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/guzgfvcer.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.fehbvm.com/Article/details/gyttoyken.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gqnfgfkdb.sHtML

JS:   #private 字段；其余公开
来源：http://wap.fehbvm.com/Article/details/gbsdxnicg.sHtML

TS:   public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gruvznguc.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.zdbjq.cn/Article/details/ghakccbnw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gikbcbpif.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gvzooqesk.sHtML

C#:   public / protected / private / internal
来源：http://www.blog.zdbjq.cn/Article/details/gzzhefisk.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gsbratcng.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.fehbvm.com/Article/details/giyrpgoon.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gdrelnmxv.sHtML


<!-- 参考信息 -->