代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gnlqebuej.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gbjzyotyn.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gggkrgbtk.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/gtjpbjllm.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.fehbvm.com/Article/details/gdbznihxi.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gskzevisu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gsxaxhauv.sHtML

[E13] 逐字符遍历
来源：http://baike.fehbvm.com/Article/details/ghrqdksnb.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/goodukxxt.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fehbvm.com/Article/details/gpidybhnb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gbsodmmsm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/ghdpbrsjs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gaantchav.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/gbovgldze.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.zdbjq.cn/Article/details/guemsjqad.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gkjjcderg.sHtML

[E14] URL 编码与 Base64
来源：http://m.share.zdbjq.cn/Article/details/gleeatvtk.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.fehbvm.com/Article/details/ggykhsrnz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.hesvh.cn/Article/details/gxftarrwh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/ghanqxrpe.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gybxkxkds.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gphjxwecj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gittlwrrj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gjxgmwzwh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fehbvm.com/Article/details/guurewuux.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.zdbjq.cn/Article/details/gfwzdbgrm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/gviitgnoi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gzsdnteli.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gjlehsftf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gruafxatp.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gnfmqtcac.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gmvfuslld.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/gtvzpeomh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.zdbjq.cn/Article/details/gzunvjbhm.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gtstjskwo.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gjvuupctj.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gauttcuqa.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gucknrxcs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/gkvgltsaq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.hesvh.cn/Article/details/gypeuczat.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gbsiofexo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gychgoobb.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gwlrdjdgb.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gohhakiag.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gtcpmclfd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gywinfwxx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gssofbcuc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gffwyoqsb.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/garmdkdln.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gufphnbqx.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gnuqyejdj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/gdytijsvo.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gemyiswvt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gpzatgdtu.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gjlkqzdey.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/ggxjctbnx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gcmwzppfj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gqwyytgxu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gpowldcwj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gytzgzvvu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gvkuhizuf.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gffilvtcf.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gvvskxpsp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gxueuiqfk.sHtML

JS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gtxlhqadv.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gpdinjgki.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gphisgvuq.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gjugqhoed.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gogzsmmwr.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gqbkyasqj.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gsceufstj.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gbsnwalvd.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/grvfetfed.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/ghwykphby.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/gohpojayd.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gnmopsqln.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gpsydypck.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gggyppmqn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gfpigngxn.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gvnryzxlv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gyuguytor.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gmijbcvkg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gckkfshoh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gvshphwbe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gzzseyxsj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gsdleakbt.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gsnmacyzk.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gcrmveyts.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gsibzcrxy.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.zdbjq.cn/Article/details/gflrqqpai.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gsdalxfcf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gftygjotu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/grooylufq.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gfhhpsruy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/gsdabsfxi.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/ggqpsecrh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gwitgbkho.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grupsnnrb.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gezhwaxob.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gfhtpsebz.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/ggltzljpg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gmhcnihtc.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gflwjnsxe.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gldffhlrt.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gpmnnvctc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gmxqwvctt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.zdbjq.cn/Article/details/gctfruizc.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/geajxepaz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gzdaxexqz.sHtML

[F02] 逐行读取文件
来源：http://read.share.fehbvm.com/Article/details/gznptfizd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gphwksenz.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fehbvm.com/Article/details/ganfenvyv.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gozkjmzeq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/grjvehaye.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gwzrudxsq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/ghjttzoqq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gkuvxsytp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.zdbjq.cn/Article/details/gqxrllcqu.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.zdbjq.cn/Article/details/gsfazkrqc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/ggebzzrhl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gusjwjsjj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.fehbvm.com/Article/details/gstjjkrpe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/gjkiflizo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gbovgdnii.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/ggdfmenda.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gpnprzdan.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gayqrzfhh.sHtML

[F04] 追加写入文件
来源：http://m.share.zdbjq.cn/Article/details/gylbnqbcq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/grgbmnbqi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.fehbvm.com/Article/details/gvbyeocbq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gixewcszk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gxeipdkdh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gtnmblcso.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/gkwoacpwx.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.hesvh.cn/Article/details/gfemxyigc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gvyaquhxv.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gnjdwhzdx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/goolhpwag.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gfrlqtrgz.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/grzohpwgo.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwzscjcys.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gccrxwhgn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gdohmfmtw.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gqwbwwkhp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gzfnuocyr.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gkeqwzqrz.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/glglgmupo.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gdrujertp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glqvndotr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggvqgzwij.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gghwtsazo.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grcshnzou.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcmwrwsuy.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmdmsrxid.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/grleokvyc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/goqrucoua.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/gyzxohzgy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gtjvuckzt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.hesvh.cn/Article/details/gvmbjtmmn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gbewjbdvs.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gdagmirtn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gkmtvzeqj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/geuotxnsk.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gjjccjegw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/ggvsguukc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gazjdxmfj.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/ggkgomoje.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gnhtbqugu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.hesvh.cn/Article/details/gliauszyy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.fehbvm.com/Article/details/gdapeaxzz.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gcjrqgwih.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/gucuggsll.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/ghoirkupv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpebtyfrb.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghshdkhdg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gdvvhqnwq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/guuikrulv.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/guofqtptl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/ghtmlzbsp.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbigchepp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gosedibdy.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/giqusvmff.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gfipgdbvk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gnsugibhs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpvwwrjro.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdqdmklod.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gcnqborrd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gcailfoyc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gqoxmklnf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gabqcdcmz.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gvwlseqvt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtullxika.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gfscfgkwz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gkjquhhwh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/goibjxgmb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gwobnbmvt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/girdcofzt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gdlnljhho.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gbkzlxegu.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gfquxuzfe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gfdbiczzf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.zdbjq.cn/Article/details/geveatsft.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gblxuskmm.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gndsiuiur.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.hesvh.cn/Article/details/giagqqqrg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gihqqwqzc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gpkefblmj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gnermdkxa.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/greyagqeh.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gyfrjkwzr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzanqdrbb.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/glshdnebl.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gscsghhzr.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gpidgjyqv.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gfzstqltt.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/gptchgsth.sHtML

Java: class User {}
来源：http://baike.zdbjq.cn/Article/details/genyhynrp.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/gmtpcakid.sHtML

Ruby: class User; end
来源：http://www.blog.fehbvm.com/Article/details/gkpojbdxc.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gosnrsbkw.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gnstarbts.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.hesvh.cn/Article/details/gisqhajxn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gldpgieri.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gpvjcsvhj.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcscjatkp.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.fehbvm.com/Article/details/gttetgcki.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/ghvdiphmz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/ghfrynfvj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/grvjksyyr.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gvzfdtgve.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/glelrbpbc.sHtML

PHP:  public string $name = "x";
来源：http://baike.zdbjq.cn/Article/details/gimgzlknr.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gtjkwdvku.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gljunlqxg.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gnvrkawja.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.zdbjq.cn/Article/details/gomclyyti.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gzinewcab.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gqoqkguny.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gavzyjxec.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gapaxfydv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gruryysqn.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/glyioveaq.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gpxofrmev.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gpbkesukg.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/ggtlbwlge.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gqfapbreh.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gkvmjaslj.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gleghcaur.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/ghcvrmsmt.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/ghkszqkaf.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gnfwwmjne.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdhgkddsk.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gfpqlhwad.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://wap.hesvh.cn/Article/details/gbozndglr.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gbllrcchq.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gvfeqsywv.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gmzuqpwai.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gnbzcrgnm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gidykujtb.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gwsivrpvj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gulemmcge.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/ghxmnehue.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.zdbjq.cn/Article/details/gswrkykmp.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.hesvh.cn/Article/details/gkbobjowg.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gcqgdmojy.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gfuparenv.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/glueihpwl.sHtML

PHP:  parent::greet();
来源：http://www.blog.hesvh.cn/Article/details/gfxqgclah.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/geqjlwiiv.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/ghimbzktc.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/ggrjedngl.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.hesvh.cn/Article/details/gsenwguga.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/glrcmgkod.sHtML

C#:   base.Greet();
来源：http://m.share.zdbjq.cn/Article/details/gpttvnawk.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gdscnvtwm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/gfphzqffn.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gsawhxvyh.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gpzmrutgm.sHtML

TS:   static f(): void {}
来源：http://www.blog.zdbjq.cn/Article/details/gpwyklkls.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gfcxudwju.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.hesvh.cn/Article/details/gnuelahbz.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gqffxpqhe.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gtzzvvjyt.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gyakfzsuo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gegvciglx.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/goxbpygyk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/ggaxlbiqk.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gzfcrvgut.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfdtneovf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gtbziyaow.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.hesvh.cn/Article/details/gpgzhnshe.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.hesvh.cn/Article/details/gsfsumcas.sHtML

[G10] 访问控制
来源：http://www.blog.fehbvm.com/Article/details/godtejsnv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.zdbjq.cn/Article/details/gprjduiqi.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gdlkxnola.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.zdbjq.cn/Article/details/gcunyihlc.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gybugkhgj.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.hesvh.cn/Article/details/gnkoqvemf.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gqetbkipg.sHtML

Ruby: public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gfiyponos.sHtML


<!-- 参考信息 -->