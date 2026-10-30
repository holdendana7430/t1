代发 wailian999

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/githanwhm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gvjxjasip.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gybxampwy.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gcqlfcwpy.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/gqzsmksgz.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gyylijuxu.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gtodhutfp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.zdbjq.cn/Article/details/gboawguox.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.zdbjq.cn/Article/details/gzuvgyzvo.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gwlrksnuo.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/giqemroyf.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/gspqdwttc.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gmtzgctph.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gcopsiisn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gjubkecfk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/ggpgaplja.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gagmyspoz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.zdbjq.cn/Article/details/ghuhipltc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gsqtmkqwv.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/grrznhztk.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gxeynzlrc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.fehbvm.com/Article/details/gopwflknd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.zdbjq.cn/Article/details/gpwpxgxhu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gucnjdiqw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/guaggtght.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gpsdfsoqc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.fehbvm.com/Article/details/gmahullxp.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gjbngmwgb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gnrdimcsp.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gkrtelodh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gisrzocvv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gomthvpmn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmnmbowhp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gjtkirxzl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/ggrwdraln.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gkoqnamjv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gtevxmfrg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gyklopqqr.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gtorvdkgl.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gyklowits.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.zdbjq.cn/Article/details/gjnwcyiwc.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gbopuwdku.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gkagfhfmp.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/ggovownzg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/glfgjrxry.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gtnsnyceg.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gqjcgixov.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/ghsquykgg.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gsmlcdrwg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/giqezlziy.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gwhkeqhmy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gsjaokldv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gtjxjfgds.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/goxxzpwor.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gcxbhubfy.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.hesvh.cn/Article/details/gzfilwhvq.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gpqlkanbb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gswskhpkk.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gaxohjgjc.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gakcllgzv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gsdrzcmsb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gxydvbdeq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gdttityqv.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/glgrslvbh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gbcduuufp.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/grwuhtpqx.sHtML

Py:   s.splitlines()
来源：http://m.share.fehbvm.com/Article/details/gymcckjhi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gwjwqkwrw.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gkvquxxuz.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gvlqrekhw.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gjcoekkkq.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.zdbjq.cn/Article/details/gdtzwuyqn.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gsizroqsv.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gmipmfmzp.sHtML

[E20] 判断字符串是否为空
来源：http://baike.hesvh.cn/Article/details/gtityzuwu.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/gaetdjfsy.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gapzojcwl.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.zdbjq.cn/Article/details/gncascusa.sHtML

TS:   if (s === "") {}
来源：http://3g.hesvh.cn/Article/details/gxlafcdgj.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gbaubrlfm.sHtML

Go:   if s == "" {}
来源：http://mobile.hesvh.cn/Article/details/gwhxfadeu.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/gyrxopcto.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/ghzodihhf.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/gwgflmbzb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/ghbjhikwy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/goqtehpuj.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gdiofsqmj.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gsylhjvip.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gntohsdia.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gmlcxixmx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gkvljyrzt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gzkfkdako.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gtgyrixno.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gtuhzruii.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/ghuavsgrq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gefiviatu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gsthojawy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gysahrytp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gosunydbt.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fehbvm.com/Article/details/gkyydmrst.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gbftvthwt.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/girkpntrn.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gvexktgjp.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjotbcpsw.sHtML

[F01] 读取整个文件
来源：http://www.blog.zdbjq.cn/Article/details/gorfyckzf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gqummhqoe.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfkadtppf.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gcxjdsifd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.hesvh.cn/Article/details/grivomcrx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gusyczgrd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gfjhgmppw.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gytlyeuzd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gzzolimrb.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fehbvm.com/Article/details/gzaebqufc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.hesvh.cn/Article/details/glpdvbvmi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gpvwvblan.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gqnoedhey.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gojrtjasw.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gdtpmlgay.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gqntxykev.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/glfivwpkr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gezxkubao.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gcmhcpzbv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gbzealggy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gabifhnmg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gjystwgdh.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gecvrquik.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gqtlhxmte.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.fehbvm.com/Article/details/gjyngcwfi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gfocnqdvj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gvpmfuptn.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/germleyyn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gidqmokic.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gjxpqdtet.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gladvakly.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gmnredmap.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gzzjzquka.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/gzbzwpmuo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gywbyvefj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gdcbwplzu.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gdlwkpqao.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/grflgaeqt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gajuyfjbk.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvrqotnbb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gcwxgesyy.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/guzivprbz.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gmkcpchax.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gispyoidy.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkhbascnb.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtgvtmvgd.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gdpzrpxpo.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gtjcbpoyu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gatduxnmk.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmvyxoezr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gmislruqy.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwuczoycg.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjnvomsvi.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.hesvh.cn/Article/details/gyjiqlbjg.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gciinbhhi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gahyenfft.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gwsbfiybu.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/glpkrtctj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gleosbrhh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gwijpxkhu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gkopfeogu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/ggiwfuuzi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gzielnioz.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gmvbowxjq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.fehbvm.com/Article/details/gfvmgcwto.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gknsoifve.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gjkbafnfc.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gufaurxzr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gbindequc.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/ggtzhzvyd.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gvqrmwfvz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.hesvh.cn/Article/details/gajxlbwfc.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gchhcttmo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gmgldhzys.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/geijulyzm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gxhtihvcq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gyvqaaolj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gbfvangpa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/grgetxscp.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gzjfzwtbl.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/gprneypym.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gpkpfzipl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggilygfan.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gfdgoobrw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gltydqslm.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/grjqxtqdm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/ggbbticlb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkcuugcck.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gmcvkftat.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gxqskczgt.sHtML

[F11] 复制与移动文件
来源：http://baike.zdbjq.cn/Article/details/gdwnncykq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gijejuxog.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gcivyoneh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/giwjxswzd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkyaxjajv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gytpcnojh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gfiqrjebp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/glcoxarfc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gchmjqghe.sHtML

[F12] CSV 读写
来源：http://m.share.fehbvm.com/Article/details/gkpabmgfx.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gtbnqyvow.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/ggqvaolst.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/ggrhgpijp.sHtML

TS:   // 同上
来源：http://wap.hesvh.cn/Article/details/gjcizittj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.fehbvm.com/Article/details/gdbsewjks.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/ghkutdaps.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gzsvnxagv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gypikeabf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gdhddsyok.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gysdkubir.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gozfraaeb.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gbtpasjwt.sHtML

Py:   class User: pass
来源：http://www.blog.zdbjq.cn/Article/details/gjoqsgpkg.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gfpkuippg.sHtML

JS:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gevhmfaey.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gzadqmeox.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gzvdzimrv.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/grjxmgclr.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gsreyacwz.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gfxblcxxp.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gcvxfffgx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.hesvh.cn/Article/details/ggbvlgzle.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gumqstxqu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gjtkqdhzy.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/glcrossdl.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gtfjmrzhr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gzadwcbzb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/grrmbxvzh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gkbzripzj.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gjqvlenxq.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gufjdurez.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gnkhmwlzl.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gctypbflg.sHtML

TS:   name: string = "x";
来源：http://mobile.fehbvm.com/Article/details/gfavfmxgc.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/gnzovkozi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/ghjmpnswe.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gioojaakp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gxzvbqlix.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gqadjkfvm.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gstrlfvtk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gvcewvosm.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gncvlcssz.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gqjwyfwcc.sHtML

Java: String greet() { return name; }
来源：http://mobile.zdbjq.cn/Article/details/gkrzuztvz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/givwyawjd.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gpqodklhr.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/giwzpzitr.sHtML

[G05] 继承
来源：http://www.m.share.hesvh.cn/Article/details/giajnfwim.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/geobickig.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gsfdixglt.sHtML

JS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/guswefywe.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gypqiunrb.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gufrauwib.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gtprjhwho.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gwmlxzxsj.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gxwhlrgfc.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gjngogipc.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.fehbvm.com/Article/details/gqgidmrcm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gciayefzp.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gvkseuioe.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gulendqfs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/ghboageke.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gbkgacmiw.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gwvwypfzb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gmiovedad.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gxsofkcex.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/grstzjrhy.sHtML

PHP:  parent::greet();
来源：http://read.share.fehbvm.com/Article/details/ggpmtazqf.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gkbhykftj.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gkvstkwwa.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gzrfsfabw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gykmqzdzx.sHtML

Ruby: super
来源：http://www.share.zdbjq.cn/Article/details/gsnrzagrh.sHtML

C#:   base.Greet();
来源：http://www.share.hesvh.cn/Article/details/gwlvdbxkb.sHtML

[G08] 静态方法与属性
来源：http://www.blog.hesvh.cn/Article/details/gnkskzlxt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gmtffmuru.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gqgzdllpp.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gagdgjwtk.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/gydurgyrx.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/gybhoywso.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gcwwndnzy.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gkltvrypn.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gcfjrpdxj.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gtbyszviv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.zdbjq.cn/Article/details/gupvqqbou.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gpwvphlql.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gjsgtpkgu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gwbzcnaqw.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gbpxkywqs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gdvwhgrkw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gbgwcvfrd.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gsdnddrkc.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/grdnnjvai.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.fehbvm.com/Article/details/gjdvyfkoq.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gtvmielzz.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gtyzvdhjw.sHtML


<!-- 参考信息 -->