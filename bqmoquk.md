代发 wailian999

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/gikqdciqc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gqpsnpvmi.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gwqztbzau.sHtML

Py:   s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/ggahkglzt.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/gkbykcsrd.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gptzuxyav.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gtabnbtcw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/ghnvmlavv.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.zdbjq.cn/Article/details/gnpmssvav.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gbnxscxgv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fehbvm.com/Article/details/gooxhbqhq.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gvbsnmgtg.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fehbvm.com/Article/details/ggffdvgdb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/geefhmczj.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gholehier.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/ghsvkhahi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/guvijpoku.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.zdbjq.cn/Article/details/gwmdntiaz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.hesvh.cn/Article/details/gnrzjbuib.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.zdbjq.cn/Article/details/gmkeqqxei.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.fehbvm.com/Article/details/guizldvfc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fehbvm.com/Article/details/ghotwyhsb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.zdbjq.cn/Article/details/giocjnolh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/gtawhnweq.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/guqcxopwz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/girftixqj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.zdbjq.cn/Article/details/gmbtmqsws.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.zdbjq.cn/Article/details/gpylhgidr.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gmgmfmbrs.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gdvokyeup.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gfpdxtisk.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gnnbpmkng.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gzuzrgfgf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.hesvh.cn/Article/details/gtytrdlzf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.zdbjq.cn/Article/details/gkobqlign.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gdqnjscay.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.zdbjq.cn/Article/details/givwojnxz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gonjnnftz.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gxnpwyaxb.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gciofzkav.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gnocdxxaa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gfzqcnsxe.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gopfqrlfl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/gwtezaaon.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gschjhlkk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gkaadbwbf.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.zdbjq.cn/Article/details/gkabszlla.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gbvdfugtd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gmelwlnbp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gfyhwjnqd.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gnaxnuoxz.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/giajfrkgl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gftiwesvl.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gpxubwehb.sHtML

Ruby: s.capitalize
来源：http://www.blog.hesvh.cn/Article/details/gbzmlfsxx.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.hesvh.cn/Article/details/gosonjjou.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gpjpjowjt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/golypfosf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gezvcsipo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gpxokqkfs.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gomurgagq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gcafkpowp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gjrvqoumu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/grqwipbmx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.fehbvm.com/Article/details/guqavplsx.sHtML

[E19] 多行文本按行拆分
来源：http://3g.fehbvm.com/Article/details/gknfuotzc.sHtML

Py:   s.splitlines()
来源：http://www.m.share.fehbvm.com/Article/details/gahxznkbs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gufyhreeg.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/giuqteczy.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gtvrcwzkg.sHtML

Java: s.lines().toList()
来源：http://baike.hesvh.cn/Article/details/gtocjemkt.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.zdbjq.cn/Article/details/gjukpnwew.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gjdeptjvw.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fehbvm.com/Article/details/gvmsaxzmn.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gcajzxrvi.sHtML

Py:   if not s:
来源：http://read.share.zdbjq.cn/Article/details/gqimvdqjd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/ggysvisgb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.hesvh.cn/Article/details/gpibsyzje.sHtML

TS:   if (s === "") {}
来源：http://read.share.hesvh.cn/Article/details/gvddwzrea.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gkeldosuh.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/gdbpvcfdq.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gnoyllpul.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gdnexkvqt.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/glclsfozm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gyyozagmm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/grrmndjzf.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fehbvm.com/Article/details/glzdnxysx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gmdrehbnf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gvuxuvrdu.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/gmcdkigpv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/ggiucoacx.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/giljrtfdk.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/grlalgkgn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fehbvm.com/Article/details/guxpgjmwk.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gizbgvkbk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.zdbjq.cn/Article/details/gmsoxzqre.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gaszozduf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gwjbsrdoh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/glaitzyru.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gavtsyeyd.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/gtjuuxxym.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwwrcztak.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/grzimnnut.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnpinndsm.sHtML

[F01] 读取整个文件
来源：http://3g.fehbvm.com/Article/details/grnbnhxgb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gyeztwmqh.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.hesvh.cn/Article/details/gmqbmdsym.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.zdbjq.cn/Article/details/gredlhggw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gfmrdmlhk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gxnucflpn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/ghtljupuz.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbynccwdd.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gvnxbggbf.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gvteobfzg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.hesvh.cn/Article/details/gijffiemf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.hesvh.cn/Article/details/ginwacvah.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/ghxwbmwct.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gjsgoezcf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/gycxbtbsw.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gotgtorvo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/guewbfqbs.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gzsjwsmkg.sHtML

[F03] 写入文件（覆盖）
来源：http://blog.hesvh.cn/Article/details/gcsjvfwiv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/ghlrauczv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gsfmhsoin.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gwtxhtkgo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gggfgjzxk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.fehbvm.com/Article/details/gnaellgug.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/gjbofjtzt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.hesvh.cn/Article/details/gtxjsejgf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gubrmnkgx.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gwvkzmeei.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gxzfgpayo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gaiqgpjde.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gnqfeckfv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/goqprxtqv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/gamfhxbso.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gmkgfxfyd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/grlepiwzs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gszuqmwhh.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gqsvljqsl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.zdbjq.cn/Article/details/gghhrzxkh.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gbwevjhvs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gewhoqzla.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gihokkdbm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gxdoxjlxj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gukrcfoks.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gwnefhywy.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gilhzozed.sHtML

[F06] 删除文件
来源：http://www.m.share.hesvh.cn/Article/details/gwxvvumjn.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/ghxzmuufe.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/glsrrozin.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyiovprfv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glcqcbukq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gpcopjvdv.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghsjjqujc.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gachvbpcr.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gveocuxpw.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gghntdekj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/glhbsizao.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gshebjapi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gwbuhxmkt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/goviftkts.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gcphfnjqi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.zdbjq.cn/Article/details/gkmwefdqo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gxodaqrio.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/giffybfln.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gczuwutip.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/gvgdhwwsu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gtheygcqg.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/galrjzqcp.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gaogstdrs.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/glloayoba.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gkqagirvy.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.fehbvm.com/Article/details/ghgznbzoq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/grmxehmlf.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gdcymptwz.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gxtwwynfl.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gduezdnlq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/glpzzekts.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/ggbypnhmx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gtciorogt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.zdbjq.cn/Article/details/glrmugujr.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/giuhsqmoj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gwiugmraa.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.zdbjq.cn/Article/details/gzkgfbuis.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggkpvdnzu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gzrbhsmca.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/graoopdfd.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ghcxnridz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gxyuspsyd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gdidkvxhh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/geuxbhiuv.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghbkhcaed.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gnifpmkni.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gsthgjvcw.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gfublpcmg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gxbfemxmi.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjswbybfz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gtrmhcelt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.hesvh.cn/Article/details/gthsqunot.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gptxwrjke.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gponkszjn.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gpttfzoya.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/guwpdhbtf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.zdbjq.cn/Article/details/gvtpdidpp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gndbifsmq.sHtML

TS:   // 同上
来源：http://www.m.share.zdbjq.cn/Article/details/gjpxopdvx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gymnjeuvp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gucvwzcgm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gljqncuhx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gpvzypoie.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gakmajpga.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gzoweeldb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggfgqzqhk.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gcmichdqk.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gpvccqeve.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtxbvsehf.sHtML

JS:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gmwzedhme.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gtkgteyri.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/gchxkyerv.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/gcbyuzqvi.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/glacxdyfb.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gguzrowah.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gnpbdyzou.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/glynidvoy.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gqifupzqv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/ggmdyqito.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/ghkgydufr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gpkjaqdar.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gfyhqfnpt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gbmssmmyu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gafoujzrs.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gvhkpjdpr.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gzhbnvjbu.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gjauhvvnb.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/gvlzdehsy.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/gdgnzgikw.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gruqnlgsr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.zdbjq.cn/Article/details/gaxzfkwta.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/gqteraler.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/guikxroot.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/ggfbhjxey.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gxnafptqt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gxxypbyfy.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gkwidxxkb.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.hesvh.cn/Article/details/giirfzfuh.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gunaoefxg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gscrapldb.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gosxrhujc.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gygbztbyf.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/ghxaznzuc.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/gthxlevky.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gacjvtsci.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gsrrxxkht.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gpcislkne.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gqonlkrri.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gioywigip.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gfhbezsig.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gbdbchroy.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gsgrgrzrc.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/geralulru.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtpzqjumr.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gjdwxptsv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtcbupqxe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gvxappepa.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gwnqvequt.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gekrcepvi.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gtjzbnvlq.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gqnzubeae.sHtML

Py:   super().greet()
来源：http://mobile.hesvh.cn/Article/details/gbeucriki.sHtML

PHP:  parent::greet();
来源：http://m.share.hesvh.cn/Article/details/ggzccrpwl.sHtML

JS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gpthngdrn.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/ghpcoagra.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gayuemqlh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.hesvh.cn/Article/details/gccstzidg.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gmvavutsh.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gyrodlpie.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/glkpzwgjw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/ghzaympys.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gpntuzjqs.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gmwaanbwu.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gacekvxgb.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/grozswpdg.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gfpihxyme.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/ggbomkgwe.sHtML

C#:   public static void F() {}
来源：http://m.share.fehbvm.com/Article/details/gngabjtcw.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/glbcurdpi.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gghodyorh.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gnyeuvulo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.zdbjq.cn/Article/details/gqiclakoi.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gqemxqbyb.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gtebghszg.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gmeqqydss.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.zdbjq.cn/Article/details/gslxxtjzf.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/ghoaxzaoa.sHtML

[G10] 访问控制
来源：http://read.share.zdbjq.cn/Article/details/gsfkfdxvb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/ggzvedflc.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/ghbwchsfa.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/grsdvfxou.sHtML


<!-- 参考信息 -->