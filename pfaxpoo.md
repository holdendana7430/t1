代发 wailian999

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gepokgnsr.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gpspknmpn.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fehbvm.com/Article/details/gpnyxvlep.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gvefswdyx.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gkrfkstom.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gnjopztua.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gqeocbvkq.sHtML

[E13] 逐字符遍历
来源：http://m.share.fehbvm.com/Article/details/gbpccuwjk.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gctulrnvs.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gqsgbxaff.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/guokvvkcd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gnsvlfebm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gsthyzifd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gcevyvnfu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/glpqrchvm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gxxtosbbe.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gjwvcoczb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gsizaixvh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gbejfqbxr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gjesjmtvu.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/grfeespbk.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gdkwihgvp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gyfceimwt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gupxnziwh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/glkyhmcwj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gtlhqgpbt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gqjvpgubx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.zdbjq.cn/Article/details/ghqrkagdi.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gokejnytd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gckyqkbos.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gzsssldiw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/goypghckb.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.zdbjq.cn/Article/details/geuktzkgs.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/grhluxgwd.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gcyxpcamo.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.zdbjq.cn/Article/details/gtftempbz.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.hesvh.cn/Article/details/gainegwha.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gqgvmfpyt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/gcvsrwdqi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/grbuloveq.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gyvbweppq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gpgfbylzl.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.zdbjq.cn/Article/details/ghiplxnen.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gqowwzqri.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gwjehwxgv.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.hesvh.cn/Article/details/gmtmpcknm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gsggxggwb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/gbmoxjfuz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/glepqdjwn.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gsqacilas.sHtML

Ruby: s.capitalize
来源：http://3g.zdbjq.cn/Article/details/gqnxcmenf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gmpxkarbq.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gqjmnewma.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gfoielabg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gnqlfslpx.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gdzcbnyot.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fehbvm.com/Article/details/ggdluvsvp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fehbvm.com/Article/details/gkupbeeof.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gzstnhpni.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/ghfwwjalp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gxnvkpijf.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gtoevcgtn.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/grrgnabsg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gkketblgf.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gcfezwkut.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gzpbihgzp.sHtML

Java: s.lines().toList()
来源：http://www.share.zdbjq.cn/Article/details/gsfftqvug.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gyjmeyszx.sHtML

Ruby: s.lines
来源：http://www.share.zdbjq.cn/Article/details/gzhdyiwgc.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/ggvmoxiej.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/grhtfmzja.sHtML

Py:   if not s:
来源：http://3g.hesvh.cn/Article/details/gzbdiaekf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gwfwbvukx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/grsjxtwuk.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gsrjbsijb.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gznfuzwdf.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gpzitflww.sHtML

Ruby: if s.empty?
来源：http://www.blog.zdbjq.cn/Article/details/gmavmdtci.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.hesvh.cn/Article/details/guwrsbtum.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/gliafusgj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/grvroenys.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/gzkgunyth.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gccsgysqq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gwqvcfkmy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/grydqrmxo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gzmbwfxnn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gzmaylcsw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gdwmyyqyi.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fehbvm.com/Article/details/gxdutfiqb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/guscwlajo.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gfofluypu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gincgsyep.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gmqqgrdcf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gqxslmwdw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gzzvwpqiq.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gvzzoqzqt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gjvupxjvz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gumrzgoov.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gsdkzleqh.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gurojrule.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gwjdxjefn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/ghszcdtfi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gepzjljtm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.hesvh.cn/Article/details/gkkavdzdx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gewtbfdlu.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gfgfktmaq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://wap.zdbjq.cn/Article/details/gkthrgqaw.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gkmxlulqm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gshcdovhn.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gzujqthfk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.zdbjq.cn/Article/details/geikinofd.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://m.share.fehbvm.com/Article/details/gnpvykyuj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gjywgedtr.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gewesapmo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gdpnxsieb.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/ghqkgbsvm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gwghjzjin.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/gzshrtiyl.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.hesvh.cn/Article/details/ggouegvrr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/geuqxgulb.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/gimatexle.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gawxkifkw.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gvzeifnmj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://baike.hesvh.cn/Article/details/gttadffmy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/ghmlhsals.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gsdnvlzsx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gmapexlyk.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gsobizlqm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gwuykgngd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gtgfvpltv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/geoqlzwnd.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gymhkugng.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gvcllnwyo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gllfxzfes.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.fehbvm.com/Article/details/gsuatzozf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gavoyccua.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gxdtpbmkh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gakvorenz.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdiddynkc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkfbdrwnm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqkoejzjl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gdnkzoleu.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gyqxikpze.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtxgmbefi.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gvmceqbsn.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/gsdbtqeao.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gkgcbpdua.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gerqcmukm.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gityxbeay.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfzrzrioj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/ggvuzuztb.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gihmepjga.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gmotnodka.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gyjzlxjsi.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gbtzdljij.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gwlmjupjy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gkwpfumqf.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/geyedgapc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gjnjcxwgh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/grpprxint.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gcmuupinv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gwfvtpryi.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.hesvh.cn/Article/details/gjdbnghoe.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gelmblqsu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/ghsklurdc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/gfwuvepry.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/galpqcvua.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gzyizyssm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/ghfatlixn.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/ghgmqguey.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/gpkxbxfgd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.zdbjq.cn/Article/details/gukrdfrlm.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gdfnghdxr.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gobtnfyvi.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gznldufoc.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gooyyzsic.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gurevatsk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/goiwdxryd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/gurgixcay.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmsdorhgk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/ghqcighjr.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gwqvtnsod.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gtddbpbgl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.hesvh.cn/Article/details/gfsulswnf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmunhoclj.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/gnljhqgil.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/gmmuaoghb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gxdlibrbx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gjehswpgp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbomxijmj.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/ghyvqhqss.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gcqqtogfg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.zdbjq.cn/Article/details/ghdsfrgpn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gkarqsrbs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/grsrasrfj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/geeigcdyw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/ghlfkhglv.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gdcckokwt.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gxktdmutc.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gcztwlahi.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gnboavvqa.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fehbvm.com/Article/details/goqfbhply.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gyjkduoju.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/gztsdopnv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fehbvm.com/Article/details/gaqrbngvl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.hesvh.cn/Article/details/gfzictpjw.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gdsnmvzsn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fehbvm.com/Article/details/guhoqvzbp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grquhyqgc.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gfreuinhh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gozjnviyh.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gmrfwvjcv.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gpvzywfss.sHtML

PHP:  class User {}
来源：http://blog.fehbvm.com/Article/details/ggpfnsbfc.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/giojcjelg.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/glfaanciw.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gegvplbgw.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/geplzpgyc.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gdkmzdcky.sHtML

C#:   class User {}
来源：http://baike.fehbvm.com/Article/details/gwdbxgpzg.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/gaacarhxs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gjstovqlw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gwvxvuqmg.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gmtgekuui.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.hesvh.cn/Article/details/gvvofwciv.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gmusptvsp.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gwaqakjji.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gopclenam.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gkwmdfaxg.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/giocoqtcx.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gvkhzqhet.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gdzpqqgvt.sHtML

JS:   this.name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gquxsjnii.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gjafqhgud.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gaovoszix.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gmaffwgng.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gcyytnsxi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gbxqtuztx.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gkworvzpa.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gyhwtotde.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/guxpgcyez.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gjiiuoanv.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/guiyzozbo.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/glnmjcwrg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gfpjarxef.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/ghrviozhb.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gliqtlpso.sHtML

[G05] 继承
来源：http://3g.hesvh.cn/Article/details/gunoibdxm.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gzsuxqdqv.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gyphjwwgn.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gbyecfzfs.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gbjztlmnc.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gxrhwjwip.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/gwdooubcp.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gqxipvayc.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/googhjmgg.sHtML

[G06] 重写方法
来源：http://wap.fehbvm.com/Article/details/grxzbhozc.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/grjwldfij.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gzzidmdor.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gkahftzvn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gavrnqvty.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/ghndulowp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.zdbjq.cn/Article/details/gnforwsvl.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.hesvh.cn/Article/details/gdcuvvcqi.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.fehbvm.com/Article/details/gjijezlau.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gjbspxpxm.sHtML

Py:   super().greet()
来源：http://m.share.zdbjq.cn/Article/details/grdfszlwk.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/ghzaaqaql.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gumnwculm.sHtML

TS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/guqztoizx.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gdteucsfh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gzpbzijsc.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gqalfcdyr.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gymlyrlbd.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gctgzqeer.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gdcqpdadh.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gskdxqsfe.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/goquezrpn.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/ggppudiuk.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gmhgqwvji.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.fehbvm.com/Article/details/gusvgxkza.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/ghdvttpcw.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/geusglohh.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/glojzxuty.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gejrigtgi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gxtdtrmwi.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gacxozgsw.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.zdbjq.cn/Article/details/gknqbkrtw.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.zdbjq.cn/Article/details/gizdyesip.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/gaqgnyxar.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.hesvh.cn/Article/details/gyjojiyjv.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.zdbjq.cn/Article/details/goyyuertn.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/ghrxtaepx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gfdlhjbtm.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gojzexivs.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gutxnuhkq.sHtML

TS:   public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gjkgulfie.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.hesvh.cn/Article/details/grrszdaxf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.blog.fehbvm.com/Article/details/gztxardwn.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/glakinrgs.sHtML


<!-- 参考信息 -->