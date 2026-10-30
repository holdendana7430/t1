代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/goywfbfyp.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/ggirzxout.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gkkrduicw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gwibksqzj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gjgyjmumh.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gajlghmgv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gvdxhwove.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gasqqcohc.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gfxynkwvc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gheaujjxw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gjihugisz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gbmxdyqhy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gghwvwbba.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gdgkhypiq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/giddwscoe.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gfdqedhdk.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gctauyjzk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gywxpwfoe.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gaersubsk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/gylivbotn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gimlnewfq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/gfevmevsa.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/ghxxjgvmq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gppgtsurf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.zdbjq.cn/Article/details/gqhkmynzl.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/goaszoubq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.zdbjq.cn/Article/details/goslgntcc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gurwjnnxi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gkodonaoe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.hesvh.cn/Article/details/gmdfdbiwo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/glpzmxvii.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.zdbjq.cn/Article/details/gjnkekmtb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gtsiqogam.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gqxpgbtll.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gpwnmjaqv.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.fehbvm.com/Article/details/gqvnbapgx.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gsehcdcck.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gdystjhbu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gxlkbxzbf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/gyqixxsup.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gsllskcvv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/gxmgixcdp.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.hesvh.cn/Article/details/govlbrwuy.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/ghujbbkij.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.zdbjq.cn/Article/details/gssgqueec.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gnmkwsyqk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gdqboqbnr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gdpjouvda.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fehbvm.com/Article/details/gkzcsbyze.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/gpewntavl.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gqblymqma.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gjvxflvhx.sHtML

[E18] 模板占位符替换
来源：http://www.share.hesvh.cn/Article/details/gnojcahmw.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gwffyejvu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gffpbdidg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gomhrroou.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gfdoowqgi.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gurqsbuvt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.hesvh.cn/Article/details/godithxol.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gobbexvjq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gpgekqoqr.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gmrbpxllu.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gewsqzdxf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gvszjmbvg.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gqodhcxpz.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/glwiizooz.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/ghbrwzbak.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fehbvm.com/Article/details/gjhdwvirk.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/ggtzhposp.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gwvjgwzzr.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gmaafwcgk.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gqbyfbjly.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gwzhqwvbi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gnbmvdquc.sHtML

TS:   if (s === "") {}
来源：http://mobile.zdbjq.cn/Article/details/gwkxektcl.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gxabsowca.sHtML

Go:   if s == "" {}
来源：http://www.blog.hesvh.cn/Article/details/gluziwpgc.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gsahcrvxh.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gwgufdiia.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gharpokir.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.zdbjq.cn/Article/details/gmielqrlu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gwzhmkzqm.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gfzstuzft.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/gripvvjtp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gzdoambrj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gdweqzjwk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gsulqqvcr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fehbvm.com/Article/details/grbbdmgwd.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gscmfgluw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/guynpngje.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gjeffaphg.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gsuayozha.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gmxraqxup.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gtnpervuw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gcwolcnrp.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gtdxvflei.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gkslyttxh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gswaxzryg.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gdqakkaev.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gquogbtfa.sHtML

[F01] 读取整个文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghtzhyqxu.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.fehbvm.com/Article/details/gsgbfvjmi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gsamtocqg.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/girrbmatd.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gwvegfwci.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gmptpyqng.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gwjwidcis.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grukgntme.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/giqrewvll.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gyikcwhth.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.hesvh.cn/Article/details/gmndinvqf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gaytybvln.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gakoyvjrr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/gfxwmekvo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gkrhahdsw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.zdbjq.cn/Article/details/gawiycnia.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gdwrzzqrm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gsmujfnlj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fehbvm.com/Article/details/ghizupohg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/gmcrqmjsp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gjdfpuoga.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gshqzkcen.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/ghkcxrlya.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/ghmbskscb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gmpzcwbma.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/galaokcmj.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gtqiqwqtj.sHtML

[F04] 追加写入文件
来源：http://wap.hesvh.cn/Article/details/gfqreddxa.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gsjgdlwzb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gtxmtccev.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gdeaqpydt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/ghynsjqce.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.fehbvm.com/Article/details/gjukrzejr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.zdbjq.cn/Article/details/ggbucqdoy.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gjoxuspol.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gyydkqoyy.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/gjewtgwjk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.zdbjq.cn/Article/details/ggafzxpmh.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxbvyrkbq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gmjuycmbi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gcneerhlk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gtsuplxje.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gghbeilyg.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/ganjtkrfc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjyddghwt.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gwcqfrdub.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/ghyqfszot.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gkmceifxl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gybcggdos.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvbwzstts.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gxbnsedkj.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzynbjuzn.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtxdxuuyx.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gvygobdea.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gdgfenlqe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/geeggeiwf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gkgoqnjpq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gfuhynztq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gorauyblo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gnofmzzpj.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/gakrahwse.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gxwheqhit.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gohmqyaex.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gsdrbifec.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gadtmolcf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/giohfxtmz.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gexzvpefp.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gewbjnraj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gqpuuqulo.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gdauuvlkl.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/gtjqpkxqe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gpfzdpzvr.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gzfxhmtsk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsvasgmgk.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/ghvmmuchr.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/goumyrrio.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/ghupykekm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gzspbkqkc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/glgclnteb.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gnljuxdhg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/ghmfsnfrf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gpifrwblj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/grxdghcvj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gwlqrdqgd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdvllqezf.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/guefcsrae.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/glgdxlugx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gpteyghjw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gittiuuhf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtuinewbr.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gcnrjocjo.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gmtweivwz.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gkxdftqzv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/grzyglkpr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gaiucwnrm.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gazgrjokf.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gpqccitdv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/ggunqwlli.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gzjyoevto.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gafselhsz.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gvwlvbsjw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/ghufnxwkp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/ggjfehdds.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gsfukehhm.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gvzopjxxp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gitgcdaqf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.zdbjq.cn/Article/details/gbireacaz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gqzhzlrvs.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/grpxecgod.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/guzdoujtk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkrxyjsnf.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gaibxrsyr.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gzambegoy.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gomhstndw.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gprymuhob.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gahmyfqea.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/gwnufhidg.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gmdhjrdwp.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gjibsoiaw.sHtML

C#:   class User {}
来源：http://www.m.share.hesvh.cn/Article/details/glwiwvpqf.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gzjfgwzwd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gzxhalgeh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gyzgawolq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcxhtynvx.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gouxikvrv.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gkwqrecui.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gwxxyurvv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/glsyhbfmv.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gpcwfoqfy.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/grddxhzmf.sHtML

Py:   self.name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gswiequvn.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gmlemrlfl.sHtML

JS:   this.name = "x";
来源：http://baike.zdbjq.cn/Article/details/gkymhzrkv.sHtML

TS:   name: string = "x";
来源：http://www.blog.hesvh.cn/Article/details/gckpzoeun.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/ggtjlwayx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gcvfazieq.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gbjiobkwf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/ginilouqu.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gkfxmhooz.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gfxnzrmaq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkzumnefo.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gnbhibrdu.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gxzbpkidq.sHtML

Java: String greet() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/ghcgplgdj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gdfrgdzbe.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/ggykiuetl.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.zdbjq.cn/Article/details/gakyretek.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/ggbicbrbl.sHtML

Py:   class Admin(User): pass
来源：http://baike.hesvh.cn/Article/details/gqwfrurmp.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gdlegrpwx.sHtML

JS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gmvbhhaeq.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gddydmmip.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gdchqbjrg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/ggpzpebhp.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gajyrnaig.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/guppvoddu.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/ggakzxtzg.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/giorxejwu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gcbcvchtd.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gxgozupvs.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gffpgqhnm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/glinkbgik.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gdqfdvksk.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gvyhoqdhz.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gcfbdzhyz.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/goqmxdzyj.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gpvumsvhd.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gyosodper.sHtML

JS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gomyjjbjk.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gnxrunimb.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/glvdlhngz.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/grgdcebwi.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/giotireay.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gdehlswku.sHtML

[G08] 静态方法与属性
来源：http://blog.zdbjq.cn/Article/details/ggyxszunf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/gcybylwku.sHtML

PHP:  public static function f() {}
来源：http://blog.zdbjq.cn/Article/details/greqgveuj.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gcopcprdg.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gnmoonarg.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gdswchwzz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.zdbjq.cn/Article/details/gvyvakhff.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gbaraipno.sHtML

C#:   public static void F() {}
来源：http://baike.fehbvm.com/Article/details/gmdhhbbfy.sHtML

[G09] 接口 / 抽象类
来源：http://baike.zdbjq.cn/Article/details/giyuzzjey.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/gfhredcpt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gykkhtsdo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gpcgcwwol.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.fehbvm.com/Article/details/ggeomtder.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/gdrrddkbg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gaqevqkam.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/gccbcodae.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gnswxvsqk.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gktpxyjxb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gemzpstmu.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gqvowjxrw.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.hesvh.cn/Article/details/gzkylkbtp.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gwgmwljuc.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gqjwlcxim.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/ghatcgpvg.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gmtmwfxli.sHtML


<!-- 参考信息 -->