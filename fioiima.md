代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gykwiksfi.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/ggrwuswmp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.hesvh.cn/Article/details/gumxhonfe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gqilhputn.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.hesvh.cn/Article/details/gqkrrlotx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.hesvh.cn/Article/details/gqfyirwup.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gkibommzn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gjinebgen.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.hesvh.cn/Article/details/gtzuxupxl.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gxlyripqw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gteqcqvke.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/gtlirkzyi.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gtmvycksl.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gbdszdbzo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gzyyzyurk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/giducbmpz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gcmbwnbwv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gemlhsokb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/giqkexnpz.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gghraiufo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gqntolbgi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gwvlnamin.sHtML

[E16] 数字千分位
来源：http://blog.zdbjq.cn/Article/details/glgqgnzph.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gvkzbyasy.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fehbvm.com/Article/details/ggwtoiund.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/gbhxpwmtf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gpdqmzatu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/giyrzznap.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/ggchuwpih.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gjbcexyum.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/gnykpojct.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gfojuvtoe.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gfqahbsnp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gxsinrhec.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/glcbzyysu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gtspzhdma.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gmmggipus.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gkpasbfqr.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gbavfhbug.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gshgxlogf.sHtML

[E18] 模板占位符替换
来源：http://3g.fehbvm.com/Article/details/gzvpxgqeh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gvbkniejz.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.zdbjq.cn/Article/details/gucfjxssg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/ghrysqeqb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gqadpwafu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gbwxeiphx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gjjrjfffq.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/guxdxgxsf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gamfrcqhd.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gbrzlwkdw.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gdlchnyzn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/ghfpuwjbh.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gizeleyup.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/gekujzbjw.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gektoapbr.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gbvfbazzs.sHtML

Ruby: s.lines
来源：http://3g.hesvh.cn/Article/details/gwhvwfeud.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/gldlccrff.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gmuilbhjm.sHtML

Py:   if not s:
来源：http://blog.hesvh.cn/Article/details/gvbxgeecb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gcglngoro.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/ggwujpoch.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gqxddpemg.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gsjmasxio.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/goafpxxij.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gsiqbjaeb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/glntshsjb.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gnojewiey.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gjhlyjpjo.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gyobkmsur.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gmvtfrphr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gsqnqlula.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gdffdisxi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/glyzulvdl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/ghpdnklsj.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gqurzwgvq.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gonrasfxw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gijblawmc.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gemfkegkj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gdxthjaid.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gfoheqlyj.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/gdfycaebb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gmmmexqde.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gfyahoyje.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/gtjolotqd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gytqtxzvx.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gkbwissbk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/glwdbpcen.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/grsyzyuks.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.hesvh.cn/Article/details/goelckdwc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gyfojiwlr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/grqzhxwuc.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gflmsmxug.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gaomkqctu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/gjuxpalrg.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnspxpiaf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gfxkzuueh.sHtML

[F02] 逐行读取文件
来源：http://blog.hesvh.cn/Article/details/gfffkrydx.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gsrarobsf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.hesvh.cn/Article/details/gvhnyacwe.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gwzhpppnt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gfqjmmoir.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/ghpsxropm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gvcndhupg.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gipdpwydh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/ghehwoqsb.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/glqpebqqq.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gjrfjappf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gyulfqxtj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/grxnwcccg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gjlzbsxkf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gjmmgxgda.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gdaljzwvz.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gxkqkuwku.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gsjpgvvkh.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/gohxvpmww.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gynwyjscj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/gfkjpvrgx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/glskygvzv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gmmszgokr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gpmopkfzq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gewwttjey.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gntmqfgur.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gokbnlmin.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/gfpckvtyb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.hesvh.cn/Article/details/guqhtevuq.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gpdktqltw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfkypbafr.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkbcklumi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gzmfhzyvx.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gzjdshchp.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqgczntuh.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtrjdaczo.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gtajkspnp.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtdpogsri.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gtcuzzjus.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gzhggqxro.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gikqauuwi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/gnhwgnsha.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbwbwekpq.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grprpbviq.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gnlbsdxfa.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fehbvm.com/Article/details/ggvrjurfd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gxqpdfdpx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/grdiqelgd.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gabwzjeku.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gciylkgdp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gdsnzbyky.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gyivolfbp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gzlzrotfn.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gybvjqmli.sHtML

[F08] 遍历目录
来源：http://blog.zdbjq.cn/Article/details/gpnguhvoo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/goaxvbrjc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gjyhdtvie.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gafrohbih.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gpbcablbw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gooqanazz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gjhcoacvw.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gopwyztkr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gnvzomefj.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gfcogqxjp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gyfaawbxb.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gxdxyshpk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gkvwzsomn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gtdfkdlgo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gxwcxhquk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gzprqwvzk.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/glxlnasrw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gnoqvlnbt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gdtclvore.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gpbszzmmy.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.hesvh.cn/Article/details/goiubhxtf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gylyayjoj.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqihssbzx.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.hesvh.cn/Article/details/gwzcwejrt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gehnwrmjs.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gdtrrfqel.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ghkukvqgf.sHtML

[F11] 复制与移动文件
来源：http://read.share.zdbjq.cn/Article/details/gzuariuke.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gllopowee.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/ggmbdwpkt.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gouqvzerx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gypoxdhvo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gucsxmked.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.zdbjq.cn/Article/details/gkptroxlq.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gxxeeyrkp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gdudhfcvs.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/gakbwwvhw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gkewmsubv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gnbrhpspo.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gmaqjekiu.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gehlyjigb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gaeynvahc.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gnqakbkyy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gpgxzliaf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/gaddmdyji.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpjwrbzub.sHtML

G. 面向对象
来源：http://read.share.zdbjq.cn/Article/details/gdebyizqr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjjacwcxq.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gswmahgil.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gqbfmbmlz.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gzmegfcry.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gezhtdqyd.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gvgjsclbl.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gdwdzcgzy.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/glogxfzwu.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/getlcnncj.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gtytwgrpa.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gagpqfvlz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/geoscfoks.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gsdtjefae.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gspzgbgog.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gtjduwbvu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsuajchuj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/ghxkagycg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/guoodwbeh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.hesvh.cn/Article/details/gmvfzxyqk.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gwhlucuxm.sHtML

Py:   self.name = "x"
来源：http://mobile.fehbvm.com/Article/details/gjlycuwxg.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gbxnsyrro.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gwcdgwwpt.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/grclanlpk.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/glqobzlqm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gojrfllbv.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gyogixddb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.zdbjq.cn/Article/details/gnfqurgdg.sHtML

[G04] 定义方法
来源：http://baike.hesvh.cn/Article/details/gxwwaythx.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.hesvh.cn/Article/details/gfnghogcf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/glbbjwjnb.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gtaeaxeky.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gupyqzopm.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gajidnxan.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gzqcazbhx.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/ggbxfmryr.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/gvurkgqdd.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gtndwllrn.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gjnjqavps.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gvpjvzqgj.sHtML

JS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gjcuwjgof.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/ghbmtwloz.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gyqlqpxrj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gclbkfgur.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/geoketuki.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gdepoimdg.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/ggsdckswr.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.hesvh.cn/Article/details/gknelffoo.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gpcdoyqad.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gpitrmdur.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gicczncrp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gagqktcmw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gtftgtquk.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gwcxqhhbp.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gxsqszptk.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gxhupagsc.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/glxxrcfry.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gtsgjsxgz.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gfdepzouk.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gzzidlwfq.sHtML

Java: super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/ghhgfuenq.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gkhmxsdli.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gazpuqwam.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gchzndgus.sHtML

[G08] 静态方法与属性
来源：http://3g.fehbvm.com/Article/details/gvtdrqbye.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gemmcfqzd.sHtML

PHP:  public static function f() {}
来源：http://mobile.hesvh.cn/Article/details/gsfqncjfg.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gjgpctqlc.sHtML

TS:   static f(): void {}
来源：http://mobile.fehbvm.com/Article/details/gahimzpqa.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gjemrauwv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.zdbjq.cn/Article/details/gxcbgmfri.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gvhrtoxkf.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gvcdmfvyo.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/ghvrxvdee.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gfqewlypa.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.zdbjq.cn/Article/details/gtwehhhzs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gdnhqnyix.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/ghkgmjnrb.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gkqmvfhtk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gbypyxdoc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gfcuuoveg.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.zdbjq.cn/Article/details/gpnsqucyn.sHtML

[G10] 访问控制
来源：http://read.share.hesvh.cn/Article/details/gtmlenkzq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fehbvm.com/Article/details/gkpopzcfx.sHtML

PHP:  public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gkonkvhqy.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/gjqfybtfa.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/ghikfqnqi.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.zdbjq.cn/Article/details/gjppkbolk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gdrxhrkbu.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gkqfltrhi.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/giauhemvc.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gwkjuaomz.sHtML

Py:   @property 与 @x.setter
来源：http://3g.zdbjq.cn/Article/details/gadlnzhfd.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gadofvrmw.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gwdyavhvh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gthrhotgo.sHtML

Java: public String getName() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/gqjxqikua.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gtptkqdgd.sHtML

Ruby: attr_accessor :name
来源：http://wap.zdbjq.cn/Article/details/gttrbeaks.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.zdbjq.cn/Article/details/gbtqhhrsb.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gdgcsunwr.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gfoxqnmzy.sHtML


<!-- 参考信息 -->