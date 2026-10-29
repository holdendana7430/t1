代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/ghryfqtia.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.hesvh.cn/Article/details/gklaixmpu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.zdbjq.cn/Article/details/gvewjexdc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gnhbnnxhg.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gxwbmvwsf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gaicmkxeu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gtqquiggg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gzoibweht.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gynefffeg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/geiezaujz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gwcfhfdnv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fehbvm.com/Article/details/gyosbgkss.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gguulxwhn.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.zdbjq.cn/Article/details/gcdrnlcoc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gggadhofp.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fehbvm.com/Article/details/gnerbhjvi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gxjzbsaef.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.hesvh.cn/Article/details/glqapgich.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gnckdaoja.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gbkdvsvee.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gxkpzqiqx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gstszmdpn.sHtML

[E16] 数字千分位
来源：http://m.share.hesvh.cn/Article/details/gpbzngfwm.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/grvgzwdjm.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gruultxve.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gheqendds.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gibjkdfyb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fehbvm.com/Article/details/ghhktiicj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gihssdayl.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gyoxxbubs.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gbxahqkmf.sHtML

[E17] 首字母大写
来源：http://mobile.zdbjq.cn/Article/details/gjxwzfvfb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gdboqxgft.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gdpihcffy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gdkjjqibe.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gzdohkhlh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gyfjxbbdp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gutzoulqn.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/gorzmyhqv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.hesvh.cn/Article/details/ghmjpmcch.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gpdhjbhrt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.hesvh.cn/Article/details/gboppatfo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.hesvh.cn/Article/details/gvqgyrcdm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/grlxcowwv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gmxdnnxbg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gumtieuki.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gijzsofvd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gvfeyzylb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gmvaoflau.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/glooynsde.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gcvhhnbcr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/geweqjhio.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gaqobbrof.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gqdjllwcz.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/gbxadasls.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gyxcwehya.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gzlkzpvxk.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gmxipjqwc.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gccxnmxdv.sHtML

Py:   if not s:
来源：http://mobile.fehbvm.com/Article/details/gxhphlkkz.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gnqjfxdqa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/gwmeihqir.sHtML

TS:   if (s === "") {}
来源：http://www.share.fehbvm.com/Article/details/gzsklxdjf.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gjoharplt.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/gpcrjygwx.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gkuutlrea.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.hesvh.cn/Article/details/gwkrnndzs.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.zdbjq.cn/Article/details/gecbnpkbm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gitsqzzwn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gmcjwycyh.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gqgvoszyk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/goubrhudc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gblszacdg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.zdbjq.cn/Article/details/gmdeubled.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gjkyoarmw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/geqvpgmjk.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/gbcjnpwtv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fehbvm.com/Article/details/grnkjcmdi.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gkhkqzpye.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gdsogokng.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gjqlsdjyf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gewumkkwr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gryxnjznu.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gsasxfloa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gkdidmprz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gmqxszwnd.sHtML

F. 文件与目录
来源：http://m.share.hesvh.cn/Article/details/ghgzdhgxb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwybegnmo.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/giitddkov.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gdtgzwvtm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gzimcmmqu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gsecnjvwq.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gaainxvyu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/goovitutm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gnymrxqlb.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gvdrrjils.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gqnpiygyj.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gndmxeqlf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gpewmoiuc.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gjcctmjmt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gsstugwfp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gkzabrhax.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/geakhzsto.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fehbvm.com/Article/details/ghxszjmla.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.hesvh.cn/Article/details/ggvwhixpi.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gamdcldsg.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/grltyhhjo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/glwgsokxg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gmheftagg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gqfeiyubn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gcnndxved.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.fehbvm.com/Article/details/gklzdncsz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gkgnpnblh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gqmezrauq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gwvevdmzh.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/gibipbcbo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gauumqpgl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.zdbjq.cn/Article/details/gsnnmphch.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.fehbvm.com/Article/details/gaebxzmxi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gjxbcwyow.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/grfrgsrzz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/ggvnxgrlg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gkismodqc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gejlcpisy.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/gjqknjjim.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gixtqlvbn.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbwebkljs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqubqqpvp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ggdsazhti.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gygezoisj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/geuyfojra.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyeheyrqm.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/ggeupwble.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gsjguebgm.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gdpgpbxvu.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gphmscmxk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gkudlzwcz.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guforuvzl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gphzjazlw.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gaxvtwbjr.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gobasmmzm.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gkwdpvlbu.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gunotufpe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gposzyhps.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gzvqhbhhr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gknbxhzms.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gflbdoxyw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/guigyervh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gkfohppqv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/grlnlxaux.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fehbvm.com/Article/details/gbhwxvwtt.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gkzvajtaq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gqabgglkl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gzhyqtprp.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gmwzuzntd.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gfqkyttan.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gsgbyjsnt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.hesvh.cn/Article/details/ggofijael.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gwsmljsor.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.hesvh.cn/Article/details/ggpjvfppd.sHtML

[F09] 获取文件大小
来源：http://www.m.share.hesvh.cn/Article/details/gdlefkbji.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gykkcojhb.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gplojihlq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gdcumpcbr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gbssdjzrs.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/giazjsjqf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.fehbvm.com/Article/details/gyaeaustq.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/gkvgldwxa.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gbuhjdumm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gvegrwvnv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gkskcwbxu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggeggyfxt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gtqoheezb.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gvkkeqwgg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gnwnmqssy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gydfgvyng.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmjbvpevk.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/geojitsgx.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/glbtdxvjf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gsngqtole.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/gzpdmbany.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gagbsgofo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gxsdnxzol.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/grvvuisqu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gucxrtunn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghbyrzuti.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/guahunjbe.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/ghsxawbwr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gszpculup.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/ggjpjreoy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gepafoukl.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gljmiggpf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gehevbqch.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.zdbjq.cn/Article/details/gmeilipwj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gyztmlazr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/guejijubc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzhppmcni.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/ggrphzrbf.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gobfmzllp.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gqyklnipw.sHtML

Py:   class User: pass
来源：http://read.share.zdbjq.cn/Article/details/gktigogld.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gikldiawm.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gqvuqlrxn.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gfylwosai.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/gxpnhsczn.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/ggjcvkxcs.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/grrzmzfvi.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gyyulghfq.sHtML

[G02] 构造函数
来源：http://www.blog.hesvh.cn/Article/details/gclikoean.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/gnmzlopkg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gzqwzkczm.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzlgohpby.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.fehbvm.com/Article/details/gbxgpugku.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gfeekipbj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gmwgegmdg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.fehbvm.com/Article/details/gievcrvme.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gmfjpvxwa.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/gqmekvsvg.sHtML

Py:   self.name = "x"
来源：http://3g.zdbjq.cn/Article/details/gxzohuttw.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gkyghlvku.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/ggbecdzcb.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/glnqjfpma.sHtML

Java: private String name;
来源：http://baike.zdbjq.cn/Article/details/grizrtatg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gwfyirufc.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gtwieabct.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gakpjjybb.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gbgeodhgf.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gyjssfsdj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/grkujeuxq.sHtML

JS:   greet() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gtqbgvose.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gndvabsav.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/glaxyvhgl.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/ggbhdxvbc.sHtML

Ruby: def greet; @name; end
来源：http://baike.zdbjq.cn/Article/details/gghijwzqv.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fehbvm.com/Article/details/gtywvlcqu.sHtML

[G05] 继承
来源：http://www.blog.hesvh.cn/Article/details/ghjkeqwql.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gogfcfzrw.sHtML

PHP:  class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gpexkniev.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gpcquixsr.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gtsoygwnl.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gfshwrxey.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/gktrdelgh.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/glkkjhhfr.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gqbymqksb.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/gkezqsevg.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/ggbsfvqvi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/giopdqchr.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gqnpeawes.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gbekzjaxi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gvfkysito.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gsxcarvha.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gqhppocxe.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gdbcumhxa.sHtML

[G07] 调用父类方法
来源：http://wap.zdbjq.cn/Article/details/gtohnudkh.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gckxsqnyu.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gkfrielzt.sHtML

JS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gnpmrzzul.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gbpaehwak.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/gbxceepsf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gwiyqnfit.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gpbdyoddh.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gnrgywkje.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gflxrfhzc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.fehbvm.com/Article/details/gbjsezglf.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gfmhrgqxa.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gjqttjlna.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gjxtdsekv.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/gnepixkof.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/ghonigpqa.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gpgqlzokh.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gltlklsdj.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gizdxhzxe.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gwppbmgbj.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.hesvh.cn/Article/details/ggxglbxit.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/gjgmsumbl.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gqjztndmp.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gydilmydl.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gpehvfzds.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/ghbyevkmw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gqtepvpif.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/glyksnpdm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gbwhdlfgp.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/grlvanwto.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gyoprutdl.sHtML

TS:   public / protected / private
来源：http://3g.hesvh.cn/Article/details/gyspjjjuq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.zdbjq.cn/Article/details/gqowiadzz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/glzhmxtii.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gvitseuny.sHtML

C#:   public / protected / private / internal
来源：http://m.share.hesvh.cn/Article/details/gftwfemvm.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/gtkdwimij.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gguzgnfmc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.hesvh.cn/Article/details/gxxyqtcfu.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/grssijenz.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gewggrney.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkrjtucmv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/gkxfkmszt.sHtML

Ruby: attr_accessor :name
来源：http://www.share.fehbvm.com/Article/details/gilabolmv.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.fehbvm.com/Article/details/gkmqwbizp.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gnkrgsifh.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gxwxxrzpw.sHtML


<!-- 参考信息 -->