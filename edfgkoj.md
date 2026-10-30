代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwjbzonj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fanxiaobao.xyz/Article/details/grahpfuis.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fanxiaobao.xyz/Article/details/gostrdchf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fanxiaobao.xyz/Article/details/ghzjjazyp.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fanxiaobao.xyz/Article/details/glpnvgdub.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fanxiaobao.xyz/Article/details/gpeycibiu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/glvgufowg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fanxiaobao.xyz/Article/details/glfbgrqyw.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gwvxobskc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnkdfccu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fanxiaobao.xyz/Article/details/glfougthd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzqupbih.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbpuknec.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fanxiaobao.xyz/Article/details/gsdoxartf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fanxiaobao.xyz/Article/details/guyrwfvna.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gybfhlseo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdijbzcmv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufuobfrx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgiepnok.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gpjkmqqas.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gkxrymqbp.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoxwgdzc.sHtML

[E16] 数字千分位
来源：http://wap.fanxiaobao.xyz/Article/details/gfwgwwdig.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fanxiaobao.xyz/Article/details/glfibooiz.sHtML

PHP:  number_format(1234567);
来源：http://3g.fanxiaobao.xyz/Article/details/glisijzsb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjynwiod.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fanxiaobao.xyz/Article/details/grkgrzryg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/glzyddyio.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gurtnawub.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.fanxiaobao.xyz/Article/details/gqwpsgunv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfspxqcfb.sHtML

[E17] 首字母大写
来源：http://baike.fanxiaobao.xyz/Article/details/gasjvqcke.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.fanxiaobao.xyz/Article/details/gveanadcp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpetllgzq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaitfyutd.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gvwbcmjnr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/guietekwe.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiqbgvva.sHtML

Ruby: s.capitalize
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdojfhhd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fanxiaobao.xyz/Article/details/grnrkqkkq.sHtML

[E18] 模板占位符替换
来源：http://m.share.fanxiaobao.xyz/Article/details/glgmwfwso.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbppefgq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fanxiaobao.xyz/Article/details/gsmwvmfdi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqujlnee.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gpxtpnbas.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlkaywbm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuuejhwa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fanxiaobao.xyz/Article/details/gmwrscodg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcrduzvmk.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gxubfolrg.sHtML

Py:   s.splitlines()
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsiyqdkl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvbbtcpo.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/gynnlkrww.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fanxiaobao.xyz/Article/details/gosqivyci.sHtML

Java: s.lines().toList()
来源：http://3g.fanxiaobao.xyz/Article/details/gjgzhgevl.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwakwhsin.sHtML

Ruby: s.lines
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplybuxcg.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktpxuaqi.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fanxiaobao.xyz/Article/details/gofbbkvqb.sHtML

Py:   if not s:
来源：http://read.share.fanxiaobao.xyz/Article/details/gilpgzbzl.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fanxiaobao.xyz/Article/details/glxqurzlf.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/guievolen.sHtML

TS:   if (s === "") {}
来源：http://read.share.fanxiaobao.xyz/Article/details/geycdotsg.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxoqgbgf.sHtML

Go:   if s == "" {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gctbvvrlm.sHtML

Ruby: if s.empty?
来源：http://mobile.fanxiaobao.xyz/Article/details/gcorrjwjm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gutdaxbfz.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fanxiaobao.xyz/Article/details/gewjfunig.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fanxiaobao.xyz/Article/details/gzkggbhri.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gpwxqyzzx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/goshdqymd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gaypdgrgg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gntuqkvdr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fanxiaobao.xyz/Article/details/gzaqctrje.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwwfmzxm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbupnepz.sHtML

[E22] 字节长度与字符长度
来源：http://wap.fanxiaobao.xyz/Article/details/gfudvebtn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbonmfya.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmxwtoec.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/guuryzhma.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrjpmrph.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/gsftkqhpw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fanxiaobao.xyz/Article/details/gsdlnjffy.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.fanxiaobao.xyz/Article/details/gkipwtddi.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvtosipv.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhvvenkm.sHtML

F. 文件与目录
来源：http://blog.fanxiaobao.xyz/Article/details/gflathpzh.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwdsqkiv.sHtML

[F01] 读取整个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gavgvybif.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gficiugmm.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gvymovpoa.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnjlddhg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjwdcave.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gmmnzxxol.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbimzvfx.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gheuahcop.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxlykrrs.sHtML

[F02] 逐行读取文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnoqnrsc.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fanxiaobao.xyz/Article/details/ghjnbpvqi.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvbvtnio.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/ggntwwdbm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gqhihjhvc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzesftwqx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gygikqwmv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfubfdbe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fanxiaobao.xyz/Article/details/gbnjllxiz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiegzqfn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.fanxiaobao.xyz/Article/details/gqmyiohid.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gnflgmxpr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fanxiaobao.xyz/Article/details/gabazzocj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghummqepf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/giykzjufb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtkdktmu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfedhnwg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxiemwtyv.sHtML

[F04] 追加写入文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzfgybzn.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fanxiaobao.xyz/Article/details/gftzsfwjv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fanxiaobao.xyz/Article/details/gozwuiroq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gratroujz.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gcvbsqwbc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fanxiaobao.xyz/Article/details/gxcezlaqy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gynsllfce.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzvknwvc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fanxiaobao.xyz/Article/details/gkobdpoxl.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkyrdaaf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtxqaykc.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gjyslkiyd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfqbykiy.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gigxatjij.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gesvnwqjw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fanxiaobao.xyz/Article/details/gvwlmecvy.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghpzqyzff.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtacxwrfw.sHtML

[F06] 删除文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmcjjqaq.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxhgnqpp.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/glyhfpunu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdxasdfo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gthapmmsv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhofsnfj.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gxovphnth.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkustyix.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxmjffit.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvghylll.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/ggqzqtdve.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fanxiaobao.xyz/Article/details/gjydpgrrz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/grmspgaal.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gasqgsapi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gignfrfje.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fanxiaobao.xyz/Article/details/godqlsjnl.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggesjnusx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fanxiaobao.xyz/Article/details/grmwbwwxq.sHtML

[F08] 遍历目录
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgwoagtg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fanxiaobao.xyz/Article/details/girbjgbnx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggqhadwhq.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gcjgibszf.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gzefqmxyj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gopdkozav.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gtyszzpkl.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gbgrbzvoz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/guhqrvumo.sHtML

[F09] 获取文件大小
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwvbsimbb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gqjoonuyp.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gnkxseael.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fanxiaobao.xyz/Article/details/gchgkbyci.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyhweuzv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fanxiaobao.xyz/Article/details/guvtwxzgq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fanxiaobao.xyz/Article/details/gdphvfrcx.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gxnkciguo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdijddph.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdjsflqsl.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gyoqtncbg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/glagdzorw.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gfmhdbvjj.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gpmmlekgm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fanxiaobao.xyz/Article/details/gecpldqza.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/giqebtbsk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gynjrqbsr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvnzqnsj.sHtML

[F11] 复制与移动文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvfwhcnb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvvtpyqai.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gsvfezkvn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gnocnipfj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/getbkehsy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/gojpukdul.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fanxiaobao.xyz/Article/details/giyjfnwzd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gctpgbbbw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkxztybb.sHtML

[F12] CSV 读写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmvbwtqj.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fanxiaobao.xyz/Article/details/gktmnzbmm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fanxiaobao.xyz/Article/details/gjmgdiaou.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fanxiaobao.xyz/Article/details/gtyevmyot.sHtML

TS:   // 同上
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjkfkpyz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.fanxiaobao.xyz/Article/details/gldyydhne.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqsxgspe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guvseeprq.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fanxiaobao.xyz/Article/details/ginryzhgv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gnriirbry.sHtML

G. 面向对象
来源：http://baike.fanxiaobao.xyz/Article/details/gbkkcqfqf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlwhxgng.sHtML

[G01] 定义类
来源：http://baike.fanxiaobao.xyz/Article/details/gqvrmtnze.sHtML

Py:   class User: pass
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbfayaba.sHtML

PHP:  class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gijnvmcad.sHtML

JS:   class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/glszdkfws.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpxunseh.sHtML

Java: class User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlvhecoc.sHtML

Go:   type User struct { Name string }
来源：http://baike.fanxiaobao.xyz/Article/details/gtzxvrczj.sHtML

Ruby: class User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gasjvyvzb.sHtML

C#:   class User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjroryuw.sHtML

[G02] 构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuiwpujj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwweatmwj.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkwnwdsq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/guvtuzign.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamehxmcl.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuxanjpf.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhdeftcb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gkntesubs.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gavjpgqfa.sHtML

[G03] 实例属性
来源：http://read.share.fanxiaobao.xyz/Article/details/gfospqhmo.sHtML

Py:   self.name = "x"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzkihehq.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdsowmpo.sHtML

JS:   this.name = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/glzbpyujl.sHtML

TS:   name: string = "x";
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaffzhpx.sHtML

Java: private String name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqdcupgp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzitcyfw.sHtML

Ruby: @name = "x"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewwusjor.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gokftalil.sHtML

[G04] 定义方法
来源：http://blog.fanxiaobao.xyz/Article/details/gxysvdqcl.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxwziuyk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fanxiaobao.xyz/Article/details/gneeewltb.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuxvnqmi.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmqgmishv.sHtML

Java: String greet() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gfhljvisy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqpympkz.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gytoyshho.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxvhxugo.sHtML

[G05] 继承
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhqgvydc.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fanxiaobao.xyz/Article/details/gotwdbwrg.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdfpgxxcf.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcetpfsuu.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvgzfwvt.sHtML

Java: class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gztiwmxcy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqwlfmtby.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gefkvmviq.sHtML

C#:   class Admin : User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuildvdq.sHtML

[G06] 重写方法
来源：http://blog.fanxiaobao.xyz/Article/details/ganbwtsqa.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkyilpuok.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnpbldktx.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/geqmstylb.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guqkooydl.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliayvevz.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fanxiaobao.xyz/Article/details/gsyyeadui.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fanxiaobao.xyz/Article/details/genlnvcye.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fanxiaobao.xyz/Article/details/gclqcihss.sHtML

[G07] 调用父类方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gonfwzawm.sHtML

Py:   super().greet()
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoieoawn.sHtML

PHP:  parent::greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gjufkazkc.sHtML

JS:   super.greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gamfecqec.sHtML

TS:   super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/giqmrzzck.sHtML

Java: super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/gwnbqttkl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fanxiaobao.xyz/Article/details/gniggiout.sHtML

Ruby: super
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmhhxrqk.sHtML

C#:   base.Greet();
来源：http://blog.fanxiaobao.xyz/Article/details/gwouulrjp.sHtML

[G08] 静态方法与属性
来源：http://mobile.fanxiaobao.xyz/Article/details/ghejzfeuh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstazgwiq.sHtML

PHP:  public static function f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gofggzzvr.sHtML

JS:   static f() {}
来源：http://blog.fanxiaobao.xyz/Article/details/gsgubmfbh.sHtML

TS:   static f(): void {}
来源：http://3g.fanxiaobao.xyz/Article/details/gbtziaxkm.sHtML

Java: static void f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gxalnwknr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fanxiaobao.xyz/Article/details/gmkkvysej.sHtML

Ruby: def self.f; end
来源：http://3g.fanxiaobao.xyz/Article/details/gcswofzvm.sHtML

C#:   public static void F() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbgueerr.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxonilqo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fanxiaobao.xyz/Article/details/gezvvovsz.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gytededkc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fanxiaobao.xyz/Article/details/getnmhlzq.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gntsmkkwl.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fanxiaobao.xyz/Article/details/guixjjgol.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmobaxyw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmagcpgp.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyfgdieh.sHtML

[G10] 访问控制
来源：http://www.share.fanxiaobao.xyz/Article/details/gzodvuohx.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.fanxiaobao.xyz/Article/details/guxwrepgg.sHtML

PHP:  public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsymgxgl.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnyaydga.sHtML

TS:   public / protected / private
来源：http://m.share.fanxiaobao.xyz/Article/details/gdilvbtkh.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkjlnrcj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fanxiaobao.xyz/Article/details/gztzsziae.sHtML

Ruby: public / protected / private
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganwlnges.sHtML

C#:   public / protected / private / internal
来源：http://blog.fanxiaobao.xyz/Article/details/ghvduhllm.sHtML

[G11] getter / setter
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzgglczv.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfqfmflg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdarfjewd.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gokqvdfyq.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbunghpfm.sHtML

Java: public String getName() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghlkaumuy.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.fanxiaobao.xyz/Article/details/gfuldkepe.sHtML

Ruby: attr_accessor :name
来源：http://wap.fanxiaobao.xyz/Article/details/gmqrslbbp.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gpurchdma.sHtML

[G12] 对象转字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/glvibpjdb.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsihcpzzm.sHtML


<!-- 参考信息 -->