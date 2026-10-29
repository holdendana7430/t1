代发 wailian999

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gnxxsnamv.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gohxchvvs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gomiyiscx.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gauzorbon.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gnabptqeg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gztowhzqw.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/guypljclg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gqzlxsdkm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gguouieju.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gqmccwhwu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/gzepzdorc.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gaczjqfcv.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/ghjwvidtt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gtfifzwmo.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.hesvh.cn/Article/details/gtixxsicc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gqhxdvzkc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.fehbvm.com/Article/details/grcfiqthg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gnvetmqhb.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gnxoawhkr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gonwlxfaf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gexyndudb.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/ggjxupoab.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.hesvh.cn/Article/details/ggrrvnjrz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.hesvh.cn/Article/details/gwevkdqjd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gvurbthss.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.zdbjq.cn/Article/details/gjzakolmy.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/glsmqbjyg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gzgzckfbj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdnkulrmv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gbgzlvoul.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gdbjpbxgz.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gqkdymtif.sHtML

PHP:  number_format(1234567);
来源：http://mobile.hesvh.cn/Article/details/ghslpgnhv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gapgebfyr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/glsdfwtjj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gxmzzhkza.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/gixsduakr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gjbgfjuud.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gcebrnbqx.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gmytoyepa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fehbvm.com/Article/details/gxlwvofrf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gevlofakb.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gbmxrcpir.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gppsvkmdk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gxxpjxgbs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/grvujwiio.sHtML

Ruby: s.capitalize
来源：http://www.m.share.hesvh.cn/Article/details/ggtlfyerc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gkaloikdw.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/glosozsqm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/govgvhfql.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gmaivznvl.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gqorpehmd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/ggnepatgw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gggonzxnp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/ghcqsojsp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/guznlpdri.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gpbezxxjj.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gwrnsoplm.sHtML

Py:   s.splitlines()
来源：http://m.share.zdbjq.cn/Article/details/garirprdr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gmygkuyma.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gbdhjslbx.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gtxyrhxls.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gxvxpbcyn.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/gmviswixd.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gqovclogn.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gltjcpkxg.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.hesvh.cn/Article/details/gmxvtmjrf.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gwtkcftgi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/genkzrjqx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gxmqxahim.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gavirknxa.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gsjtgqmgo.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gvulschfr.sHtML

Ruby: if s.empty?
来源：http://m.share.fehbvm.com/Article/details/grjuvjnmg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gspzjyehl.sHtML

[E21] 超长截断加省略号
来源：http://wap.zdbjq.cn/Article/details/gedvycteq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gyfqwagbw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gxllcuqfy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gbrosazrt.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gyffgkhmc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gudlbraxb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/ggmgfyieb.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gdvsqcpgm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gaftpqzzc.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/gxgyaxnmx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gkmtbmcqn.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/ggszazfuo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fehbvm.com/Article/details/gwqnqcmym.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gjoaelaof.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.hesvh.cn/Article/details/gtnxhibiy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gxcdisfbj.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gsrcoxpoh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.zdbjq.cn/Article/details/gnaakrxke.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghzuywouv.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gdepxnktr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gccfqkxkd.sHtML

[F01] 读取整个文件
来源：http://read.share.zdbjq.cn/Article/details/giukfvydw.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gbgxmzrfg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fehbvm.com/Article/details/gskgdhavi.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/grzkkzorg.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gexppxydy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gnxkqjqjz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gowdsqsiq.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gqoxvqpcm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gkbzvsvsu.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gptebbnrn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fehbvm.com/Article/details/gfatslrdu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gwfxnjqeb.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gybvnwpnw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/geuelcgfl.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/geplladja.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gupqjbtpw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.hesvh.cn/Article/details/gwexluulx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.m.share.fehbvm.com/Article/details/gfsnrahkq.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gjvltfvtc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.hesvh.cn/Article/details/gnvbliiij.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/ghfidypdr.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gtzpotcuq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gylwehcfl.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gpvqlrawx.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gpbpmbvnm.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gdcnsrsvy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gbucfaqgv.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gdtzulpzo.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gmqwqvxlf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gbtdwmiqy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gmdpwixnw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/ggxdbhycj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.hesvh.cn/Article/details/ggtfzmsxl.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/giramowmj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gfcxdcfvw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.hesvh.cn/Article/details/glowpncml.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.fehbvm.com/Article/details/grlruroua.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/ggdntelvm.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/geenebmnq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/ghvjngxno.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gajkgnbai.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gvtuyoozh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gtbyfoclv.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gigeftqzf.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmjcnptnl.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/galqnskyt.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcvvxaghx.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gskweumxk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gslqzlpey.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghoghpybl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gtoesefcw.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.zdbjq.cn/Article/details/grsglyrhf.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fehbvm.com/Article/details/gqqlquktp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glncttdov.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/gmsqyhgsg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gqtonnslg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.hesvh.cn/Article/details/gcisyiacz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gtjgupvaz.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gmmjsieku.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.zdbjq.cn/Article/details/gehbviyma.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.zdbjq.cn/Article/details/geuhemrqw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.fehbvm.com/Article/details/ghzkfpssd.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/gojfqkcwt.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gqclyphet.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gegdswgqn.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gzgwyoiqk.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gfisgrezv.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gwvcpadem.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/garzxyxaw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gzmwhkaiv.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gmhrwykyd.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gxddcwtjn.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/gnoiuewjp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsbqjowgu.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gpjkekjhi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gddfvsduv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gitdnzago.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gwciymrka.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.zdbjq.cn/Article/details/gfkiaujur.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghznskhkk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.hesvh.cn/Article/details/gbtfmdkzp.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gdsrlaxcx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwsjskzkg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.zdbjq.cn/Article/details/ggwrlzjmr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwvgrexyd.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdulymmwc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.hesvh.cn/Article/details/gkmgdlyss.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/ghceoismu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gptwetksr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/ghinohgts.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gckifcmit.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqiamxaxn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/godxvxjmb.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gvzhmjigl.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gxeuaqgxt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/grhrefpuq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.zdbjq.cn/Article/details/gmgguvllw.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gkiyzreim.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.hesvh.cn/Article/details/gjerrfgdq.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gwgekzewm.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gqjpnmmna.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.hesvh.cn/Article/details/gywtofmzp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.hesvh.cn/Article/details/gxqurkcjc.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gdxdhmmrn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.hesvh.cn/Article/details/gdjndmugv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gxsbgyftq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.zdbjq.cn/Article/details/gehikdlwk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gigvyngsj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gmmirnoth.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gcmotplpi.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grmvnoktt.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/ghhmtbquo.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/guthsyiay.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/gmzijzjrr.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gmcwjoxuw.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gqfimsilz.sHtML

Java: class User {}
来源：http://www.blog.hesvh.cn/Article/details/gklumbbcw.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/griefnpjk.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/ghdeykacq.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gxphemqct.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gwjahukst.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gowdpjcmf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gatifmvhh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/glxktiqyy.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gzpdosggf.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gnieuffqd.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gvsodibdo.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gxkhfxisn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/gduasgvzk.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gjjoukukh.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gqrcjzbql.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gzkjlcbwj.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gqefuzxse.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gifsxlfjz.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gvcpfqyno.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gnkjdkvpb.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/gyazapsrh.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gswbtcjrh.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gqszeuzsn.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gpietwqgr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gxhecgmuh.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gymrtddsv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gfknbuolj.sHtML

Java: String greet() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/ginufpopy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gianbokgu.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/giogrskcg.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/grgvqdnfd.sHtML

[G05] 继承
来源：http://www.blog.zdbjq.cn/Article/details/gzepwgfki.sHtML

Py:   class Admin(User): pass
来源：http://wap.zdbjq.cn/Article/details/gcitpyhaz.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gmlecdbqi.sHtML

JS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gemvlyyzl.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/garmugbfk.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gtcbbebtp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.zdbjq.cn/Article/details/gygnzxnex.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gjdatxouf.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/gcihjvgqf.sHtML

[G06] 重写方法
来源：http://m.share.hesvh.cn/Article/details/gmrjygfuj.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gocytzhjh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gvgirutyw.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gwkvebjda.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/glmquivjs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwnlmsobt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gcgiypulq.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gskinpiso.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gjnptxtsn.sHtML

[G07] 调用父类方法
来源：http://m.share.fehbvm.com/Article/details/grrmujjlb.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gwfitrvwc.sHtML

PHP:  parent::greet();
来源：http://baike.hesvh.cn/Article/details/gkbuqjgcx.sHtML

JS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/gfheatarc.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gdjbaeaxa.sHtML

Java: super.greet();
来源：http://m.share.hesvh.cn/Article/details/gxhiamhun.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/goooslvzt.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gceohhbyp.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/ggwralbdq.sHtML

[G08] 静态方法与属性
来源：http://www.blog.zdbjq.cn/Article/details/gqqujsoei.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gtkdsfriv.sHtML

PHP:  public static function f() {}
来源：http://wap.fehbvm.com/Article/details/gymkgicjr.sHtML

JS:   static f() {}
来源：http://www.share.hesvh.cn/Article/details/gzvijuzew.sHtML

TS:   static f(): void {}
来源：http://mobile.zdbjq.cn/Article/details/gvmeesnjs.sHtML

Java: static void f() {}
来源：http://mobile.fehbvm.com/Article/details/gnnbnzquv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.hesvh.cn/Article/details/gbjnuorfo.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gmwdbgaab.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gvgkwmoaq.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/ghbdtjgfs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.hesvh.cn/Article/details/gudtagcnk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gceqtogzn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gunchclpf.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.zdbjq.cn/Article/details/gjhihhqyn.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gzpyjwshx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gplzeopqp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/gwbnbmeap.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfbrvyykq.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gmepcemyc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gqbhpdubw.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gmfincdmy.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.zdbjq.cn/Article/details/gdotdjcwi.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gbdjttwpr.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/golntfbuq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.zdbjq.cn/Article/details/gsqpsrghb.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gtlpwpkcd.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gskmtcipb.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gpdijjylu.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.hesvh.cn/Article/details/gybxkaafw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.zdbjq.cn/Article/details/gzwawonzr.sHtML


<!-- 参考信息 -->