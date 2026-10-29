代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gajrbtlaz.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gkfaqncov.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gctikjjvz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/ganpbsemc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gbojrlzwz.sHtML

[E11] 反转字符串
来源：http://mobile.hesvh.cn/Article/details/ggmnzkotv.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gilqtwhon.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/ginurfbtb.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gzkhycmrh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gtzckodag.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gnchsztkm.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gwkerxrmd.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gxtxuhlaw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.zdbjq.cn/Article/details/gsimwiltj.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/ghugnmvqx.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gwyyaknyg.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gnsmocbhg.sHtML

JS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gwbalbxqd.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gqcaaagvm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gcpdtzigj.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/grlanjooo.sHtML

Ruby: s.count("a")
来源：http://www.blog.fehbvm.com/Article/details/guuvaycdm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gxxceepsp.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gwblpfkpp.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gyoswdkkm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gqnuumufy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/girauobjf.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/grfsoswfj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.hesvh.cn/Article/details/gkjweabwr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gcichluev.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gzqzkezrr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gkadsbsdu.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/goasdstki.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gkxpavogg.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/gnzlrcsdd.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/ggxfsgews.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/ghauskrry.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gxijfkocm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/ghfwxnlnl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gukgrmqnu.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.hesvh.cn/Article/details/gizcvywrf.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gianuaozd.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.zdbjq.cn/Article/details/gylqxgddg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/grhodesyu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gwheuqgrr.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gagkugoze.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gyupqdxuc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gjnjddlch.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/ghpjpsucv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.zdbjq.cn/Article/details/govedphde.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gmeeqyqea.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.hesvh.cn/Article/details/gnnishmoy.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/glgbkgovr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/ggzxwzomd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/ggdloqpxf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gsbjrxsfg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/guhkkcfpa.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gjwjnkxce.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gfvmotjlz.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/glxqusdkr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gitfcqvzz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gatixpmew.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.hesvh.cn/Article/details/gnglvvkpy.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gwfevmcdk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.zdbjq.cn/Article/details/gaxmcvjau.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gejiedrfy.sHtML

Ruby: s.capitalize
来源：http://3g.hesvh.cn/Article/details/gmtcakijq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gczzczhfl.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gwepmarpb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.fehbvm.com/Article/details/gvvsqghup.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gyvaeptfd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gferhzkje.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gsqldsjnn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gpulbmtmr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.hesvh.cn/Article/details/gctbcjbne.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gmlrynqbg.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.hesvh.cn/Article/details/gjrxiytqr.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gnrlwphba.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gxaxbdoia.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.hesvh.cn/Article/details/gwmbupvhh.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gdvcqdvsn.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/ggcarsoug.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gtktzpxwx.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gvtgidsaw.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gqrfueofz.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gzspyfyip.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gxlrabgtf.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gyhljrdzm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gmgkkqlhh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fehbvm.com/Article/details/ghgzealmo.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gqldbushw.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/grvraqpct.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/grkxjkkww.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gfgynfdjc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gzkljpmhc.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/ghkumtrvq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.zdbjq.cn/Article/details/glumeiqmd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fehbvm.com/Article/details/glxdgicgg.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gofpwjzrk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gihjwwfjd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gqiyldrto.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gwyejfblz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gzdusjayf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gnnduptgh.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/gwrkmbuyo.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gsudjgqde.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gtjtyucac.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gqwkvwbtu.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gvayxgmkm.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.zdbjq.cn/Article/details/gwrpyxxzy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/grjdarrkp.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gcmnjeecj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gedukftxd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggdnkxfah.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/glvqlmxxz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giiasghgj.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gwltwpxej.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gcmybljjj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gtrygshaz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.blog.fehbvm.com/Article/details/gfcklfwyl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gcdwdecau.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gogyoxula.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.hesvh.cn/Article/details/gjocqoisc.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfidmatkx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/gvndvywor.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gtxrvhpfa.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gbzjvxwin.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.zdbjq.cn/Article/details/gnxvneoly.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gbizquuci.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/goaxudfjj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gguogpenx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gpzihcxgl.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gkvspajca.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gwtytdluy.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gzbjtegui.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fehbvm.com/Article/details/gjssbxmgf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gmzvgvkjs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gehlnkqrx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gkngqjorx.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gwxeplzxt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/gfvwjuihv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gkyoftmas.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/galirsdnm.sHtML

[F04] 追加写入文件
来源：http://blog.zdbjq.cn/Article/details/gnzvrbyig.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gcchvxiwk.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.zdbjq.cn/Article/details/gmbknsjue.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gjzyebiih.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gprzstrfu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/guyekinjw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gjudrvgpm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gfwanvoop.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gdyzslfzu.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gzhsuwmje.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/guvecfvat.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gokewgaxj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbldhpcsx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gehuqrnrz.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gfobfbrts.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/grzsralgo.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gofphfjgm.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdnpluwzv.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/gyjfsyhyp.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gvhnioevu.sHtML

PHP:  unlink("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gjjxoamxk.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqtsfhkic.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gksgyriuc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/gmcvolkfo.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqwxlirgw.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwdqzikaz.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/grsakcxol.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/gzripfwqv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.hesvh.cn/Article/details/gycoiwlim.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gkoixaywa.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gencysebx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gqwqtlokz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fehbvm.com/Article/details/gpeywosuf.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gwomqybgy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gelxzcwpq.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gbzqwioei.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gobtpblaa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fehbvm.com/Article/details/gmouxfcdz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gvogdwljf.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gngaxbprl.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/grqbqkqyr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gxhumvxtb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gtxyaubbk.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gpqbsydsb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gcieissbr.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gioqxuzzn.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gurrrgyto.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/grsqzkiph.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/ggtjnhvhr.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gjvyjxwrj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gywgrbftz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.hesvh.cn/Article/details/ggujwufbt.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gryahfoiu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/glongyoqe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.zdbjq.cn/Article/details/glaivrdzj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwobdfojg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gaoonqvkq.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/godfbikbl.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gepwiwzbw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fehbvm.com/Article/details/gxrnjtuyn.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gxocpssaw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gpocijikd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gtixwehii.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gbodbldcd.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gqrymtbpi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.zdbjq.cn/Article/details/gnfqhiydn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gybqbxxuy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdudjvhho.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/ggfbyurll.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/glzlfrodk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gmkvispkg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gfbfaxdut.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/grbmaylth.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gkjoliwin.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gdnbktaph.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gcbtumcbq.sHtML

TS:   // 同上
来源：http://wap.zdbjq.cn/Article/details/gpiklpkba.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gpktnbcnt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.zdbjq.cn/Article/details/ggfjzegom.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gxppckhbg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gbysxnllv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwvtlvaru.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/guhdgkgcr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbxgbugpa.sHtML

[G01] 定义类
来源：http://m.share.zdbjq.cn/Article/details/gkbtchcyw.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gravngxlr.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/ginuqtqhp.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gqsunpcay.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/gfxvhmhps.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/glqbonics.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/guurvndqe.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gzlnusium.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gicowglle.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/glxmhozmp.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gzzqnvpdg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.fehbvm.com/Article/details/gqbddaktf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/ginsxcsza.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gyheiyrqe.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fehbvm.com/Article/details/gbxqqtwlk.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.zdbjq.cn/Article/details/gvnjuslln.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/giahlnlpc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbweugfmw.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gxketkjmq.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/guhgfyaqj.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gqanrxcjs.sHtML

JS:   this.name = "x";
来源：http://wap.fehbvm.com/Article/details/grjlzneob.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/gdhfpgzrf.sHtML

Java: private String name;
来源：http://m.share.hesvh.cn/Article/details/gwainngpj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gpdmlfpfp.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/gddcwzwmz.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gcyhaeknx.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gkuelfusq.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.fehbvm.com/Article/details/ghdzhseqs.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gubujkyyq.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gqwkumlow.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gnzpjstfo.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/godapjyzz.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gibczwsek.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gndtcllzq.sHtML

C#:   public string Greet() => Name;
来源：http://wap.hesvh.cn/Article/details/gjtlfmcby.sHtML

[G05] 继承
来源：http://m.share.zdbjq.cn/Article/details/gqfiakdnv.sHtML

Py:   class Admin(User): pass
来源：http://read.share.fehbvm.com/Article/details/ggouwxgot.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gjevfholi.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/grcjiiyyk.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gsqckxrni.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gfioprxlr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/glysbwysl.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gdbwrpgtf.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gdwomlaqc.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gohprlwmr.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fehbvm.com/Article/details/gifgbxcrw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gitdixwgo.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gtfbbbsih.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gfwikykqh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gsagilvhn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.share.zdbjq.cn/Article/details/gonisjeyr.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gqhdbmhjz.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/ghxbsxvnz.sHtML

[G07] 调用父类方法
来源：http://read.share.hesvh.cn/Article/details/ggnzkmvrm.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/ghkzehoto.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gjoxveajq.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/goetmpdgq.sHtML

TS:   super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/gpgzgkqzc.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gcnnckfba.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gxxbkirct.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/ggbnfisgx.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gwznhsvaq.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/glamapxdx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gxyiuoysd.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gkszpkeeg.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gxwpbddix.sHtML

TS:   static f(): void {}
来源：http://3g.hesvh.cn/Article/details/ggfcnzccl.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gusbxlfbm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.hesvh.cn/Article/details/gnltxfixf.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gfeetyoqh.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/gkxjfzquw.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gvzsltrqe.sHtML


<!-- 参考信息 -->