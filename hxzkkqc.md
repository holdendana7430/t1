代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.share.zdbjq.cn/Article/details/gtqghjgax.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gmlqxwujx.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.zdbjq.cn/Article/details/ggeocxmjm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gfdtkqoyu.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/glfocdczj.sHtML

Ruby: s.count("a")
来源：http://read.share.hesvh.cn/Article/details/ggikalcvv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gpjczpzxi.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/gvgbsfrqv.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gqlbxjvdf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/gwzeuthak.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/ggffnuydb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gkgatovui.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gdaqipsxb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gheaopxpc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gscowmiuj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.hesvh.cn/Article/details/gxpyzzree.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/gtgiwcgaq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gnolxmick.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gnipvgnna.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/gfnjqoutf.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gdzcqvxwu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.fehbvm.com/Article/details/ghqklutqi.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gwqqzkmey.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/goaxslswp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gxqzmpqui.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.hesvh.cn/Article/details/gqopuqzsp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/guotipndr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/govfuhwlz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/ghfmbfsqm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gfcxeyagq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gxiwfwdbx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fehbvm.com/Article/details/gyajizzuk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/givdlvvby.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gxnnlstke.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/grjdhqsgc.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gmafgauvh.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gmpmaoube.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gpmyzaase.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/glefbdzdf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gykytwnfi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fehbvm.com/Article/details/gthitzrlw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.fehbvm.com/Article/details/ghmkewfsf.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/ghyuknoar.sHtML

[E17] 首字母大写
来源：http://www.share.hesvh.cn/Article/details/ganpwdkmn.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fehbvm.com/Article/details/gxiwireuh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gueirencc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gngtxjyve.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/gdspwgxeh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gletsxjuj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/gmxmiklcu.sHtML

Ruby: s.capitalize
来源：http://read.share.fehbvm.com/Article/details/gdibdnavw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/giwpsuhny.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gpxsohwee.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gjmmzaomr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gzooplaur.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gnuzqtqjx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gxnoxegns.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gtyykhxun.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gvqtbjans.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.hesvh.cn/Article/details/gukajkjtk.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fehbvm.com/Article/details/gtzbohwde.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/gqhmpiaqw.sHtML

Py:   s.splitlines()
来源：http://mobile.zdbjq.cn/Article/details/gdmoatevt.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gnjpjnato.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gkiovbrqv.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/glbshdiaj.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gpgoheigs.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/grwegeboh.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gduexmwch.sHtML

C#:   s.Split('\n')
来源：http://wap.fehbvm.com/Article/details/gtqmhhenb.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/ggimhotvw.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gkkofyfyn.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.fehbvm.com/Article/details/gipbgvtzk.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gfojjhpvc.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gxtdhujzx.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gjmypmkpf.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gpiukktrj.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gxftrdipi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/gupdwhnae.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.fehbvm.com/Article/details/grjdrhvdk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gqbgbxgrf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gnzvdtaou.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/geiawaxgs.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gpwadirnc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gsuxktgaw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gzygzjmgu.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/gapnmdprv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gkwiflhxj.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gggoxxgxp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.zdbjq.cn/Article/details/gedmsykfj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gacfzpvjj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/goheqcugv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gbqelxgwg.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gwdcyrhcv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.zdbjq.cn/Article/details/gdtqjfctk.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/grxnilvfl.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.zdbjq.cn/Article/details/gvjytgfee.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwvuhsmye.sHtML

F. 文件与目录
来源：http://read.share.zdbjq.cn/Article/details/gugpwqauc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcztfeiia.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/glkzhtcpi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gixmecxwf.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gvcjqosgs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gkyzabehb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/grwaqovsf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gfrdahocu.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gkeobcktu.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkonxgprs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtynomozw.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gpjznepnq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/ggpovkazv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gtqucplpi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gmzzisokn.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghpcrzvie.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gqtsbpshw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.fehbvm.com/Article/details/gtsrmtwet.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gwjfaeuam.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gvmbruygc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/grqoyedtd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://m.share.fehbvm.com/Article/details/gmfnlqmgg.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gzhwandvs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/gwnbietba.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gqprwaujf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gquotjbja.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gegqdsddm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.hesvh.cn/Article/details/gglfpvkmt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gwaobahbq.sHtML

[F04] 追加写入文件
来源：http://mobile.zdbjq.cn/Article/details/gvwlzivea.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gsfpixhlv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/glmhxvxln.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gwusnaaml.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gygvckybp.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/gqlvayojp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gfaaqzxpz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.hesvh.cn/Article/details/gntgrnjei.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gmcmowdqx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gmbqatucc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gdkjcahqd.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gqclrdgtf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggzufsgix.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gcrgujfwe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gfoahewsp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gndjipryq.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtggrbmyx.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjjidpvzj.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/gakrkgjzg.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxnswxlhc.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gscynqgss.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gvutpteym.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/grdaoebqw.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gfmnqvhak.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvcozaswg.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gsbyzszus.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gzprbxlha.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/gayewqhek.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gzwopttia.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gyjgowqxn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gsgdsvfgf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gvbnovaqm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.zdbjq.cn/Article/details/gvmvnwuiu.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gwoetgqmb.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/gzhtfwxia.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gptcvzigx.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gpahpkqus.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gzophyshe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.zdbjq.cn/Article/details/gdpjesnhb.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gruloznro.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/geudeuimb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gshqynjkf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.hesvh.cn/Article/details/ghzhrdbie.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gonpivkoz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gyvsykaux.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/ggobgtfyi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gelqtbsev.sHtML

PHP:  filesize("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gyqhhozpz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gpvaaabmp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gohtapxjv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gjanptwtc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gcehgwaka.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gaivjpleg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/guooggcck.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/ggzqhvrcz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxootguwh.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gwuzcfnjm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ghvrrfjms.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ggnvqthkj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.hesvh.cn/Article/details/ghltxnrjy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gwlntajay.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwnlnjmlw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvkiyazep.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gpsmmkgcv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gigjhxkbo.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gyilwilui.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzpsatgrv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gunqxcssw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.hesvh.cn/Article/details/gzjuoqbvs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gzkwxyaag.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gswqcgqge.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gpxmodxur.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gticjmusl.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/glxzfmtzx.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gouqsngof.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gbceoptud.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gihjjdnuj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/ghrwntujj.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gkziomxpd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fehbvm.com/Article/details/gutescasg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gbctvewkx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtufqonmv.sHtML

G. 面向对象
来源：http://www.blog.zdbjq.cn/Article/details/gbbkuuzwd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkxxvgijf.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gnjkzdewz.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gmfgxiqxu.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gjucycgcx.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gqnqrsmhj.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.zdbjq.cn/Article/details/gddrfppwr.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gpqgenmyy.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/ggstprjkt.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gmapokcag.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/glpqlkzvo.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/geolxpvnp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/ggkkedews.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.hesvh.cn/Article/details/gfzpwnurt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/ggaxfmkwz.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gmofvgagn.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gdhkvxmei.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gigfkcdpa.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/glofhpuog.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/gpdlecbos.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gowxywkex.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/guljbvcsg.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gvxiqcdsa.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/ghxhdntbn.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/giqnjaxdl.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/gcyouoydu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/ghtkbawrb.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gneizbxph.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gcxvkdqsc.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/geresimfb.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gbintgzro.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gteumyrew.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gmykpuftr.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gdfkmykhl.sHtML

Java: String greet() { return name; }
来源：http://3g.fehbvm.com/Article/details/gtuujhtrk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gwxvzifyb.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gxzragczf.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/gyjjopszc.sHtML

[G05] 继承
来源：http://www.share.hesvh.cn/Article/details/gwocebdqz.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gsjbpykdd.sHtML

PHP:  class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/ghikrrman.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gozxsvotq.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gukfyqlbk.sHtML

Java: class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gsykfqutc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.zdbjq.cn/Article/details/griqiwmkk.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gyruocqvy.sHtML

C#:   class Admin : User {}
来源：http://www.blog.fehbvm.com/Article/details/gwwnsudti.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/ggxwkruow.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.zdbjq.cn/Article/details/gxxchqors.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gkhkidlua.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gtbpllhsn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gbvbalike.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gzypfrklw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gguxnlton.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/gorxjdoec.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/geocyjtxh.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/galeofiqy.sHtML

Py:   super().greet()
来源：http://www.blog.zdbjq.cn/Article/details/gktftavbz.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gqhynqlsr.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gijovvujt.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gnaaasoyh.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gvyufnbye.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gnwpjluwt.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gytvemrps.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gqbxrqpfs.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gsboqlxvc.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gmivilbvh.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/ghfrdklto.sHtML

JS:   static f() {}
来源：http://www.blog.hesvh.cn/Article/details/gphcwnuch.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gpwqfapva.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gleqloeyc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gajjcfqys.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/guajmlljs.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gcohsfkyf.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gcxzxuuuc.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gwmexayeb.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gnrejkpro.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gsiacmlvd.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gzbfnjack.sHtML

Java: interface Shape { double area(); }
来源：http://wap.hesvh.cn/Article/details/gnwxnwmof.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.fehbvm.com/Article/details/gydasrqho.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.fehbvm.com/Article/details/grubpdaim.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/gfrphsjmx.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/ghnlhoztd.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gacjmmyvc.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gshktlkmn.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/goutspeep.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gmstayxtj.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/gautzpwey.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gxwjzgvbs.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gbrobbzvv.sHtML


<!-- 参考信息 -->