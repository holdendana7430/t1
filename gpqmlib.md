代发 wailian999

PHP:  substr_count($s, "a");
来源：http://mobile.hesvh.cn/Article/details/gjkxfpnmz.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gidrbqqje.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gkyzhjges.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.zdbjq.cn/Article/details/gsjozwhps.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.zdbjq.cn/Article/details/gjmdjtgax.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gwivztrsb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/gixwuxjsh.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gcjzzfupe.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.zdbjq.cn/Article/details/gvxpdaoza.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.hesvh.cn/Article/details/gdcarcrjf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gsdymtzav.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gzoeokatj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gcqklxsui.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gjsjdexhh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/getvpofvk.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.fehbvm.com/Article/details/gzkkofrzu.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/gqofsmoiy.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/girbgopvn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.hesvh.cn/Article/details/gxerqngps.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.hesvh.cn/Article/details/gbimcosyc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.hesvh.cn/Article/details/gbuapzzco.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gwmtzryxf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.hesvh.cn/Article/details/gfthjmzms.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/ghakgplta.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gfbdsqdvt.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gryykwtid.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gyccchwsz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/ggtrzmayy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gjcbczeun.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.hesvh.cn/Article/details/gwkxvvuft.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/girbtsgwg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gvpcvvnaq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gqqgraygo.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gtkofqypl.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gvkthcgnh.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gxbbxplqx.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/ghqdyqudf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gtsuczsmv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gcuvumrfv.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gtejqmzaz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gdyfijeey.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://blog.hesvh.cn/Article/details/gimrcrqec.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gpatpgbaq.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/grgzelemb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/gqarxdmxm.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gchopqpvo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/ghwsorrdi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gpwtidmgp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/glurebgwv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.hesvh.cn/Article/details/gjzhiaqtx.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gjfiyndqt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gfhyrrvht.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gurjsrinu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.zdbjq.cn/Article/details/grxgrfidj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gfdwkgvtm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/grauoyxab.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gmcbztsns.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/ghdugnpmd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/goroykrej.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gcgnfgnkc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gkvhkcmdw.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gzmalheii.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gzbyxkasd.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gaaoljlxv.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/gsoimgpxn.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gbfmoywml.sHtML

Java: s.lines().toList()
来源：http://www.blog.fehbvm.com/Article/details/gltgzwrpq.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/gvfujnobj.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/glhfkxwem.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/guipljgzn.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/gjxwqdcri.sHtML

Py:   if not s:
来源：http://blog.zdbjq.cn/Article/details/gjvdcbthu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/gwijbduua.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.fehbvm.com/Article/details/gojhoaqff.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gdeydbtks.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.hesvh.cn/Article/details/gqxgmnaui.sHtML

Go:   if s == "" {}
来源：http://wap.zdbjq.cn/Article/details/gzfpfopta.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/giwfzfcth.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gjcgnvchl.sHtML

[E21] 超长截断加省略号
来源：http://read.share.zdbjq.cn/Article/details/ggvertktc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/ghfdspqfe.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gwanyfvbd.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gwajtaklp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/giuwsatvg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gcwgowrva.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gptiiilhx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ggqunaxjz.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gznocxvdu.sHtML

[E22] 字节长度与字符长度
来源：http://baike.zdbjq.cn/Article/details/gkxhhtbbv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fehbvm.com/Article/details/gcgcqtqbd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gfthskudm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gxfhsoxxv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gfvobtyab.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/greqabqys.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.hesvh.cn/Article/details/giuzprlao.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gpwttuepv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/glrafilne.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gifrpihjr.sHtML

F. 文件与目录
来源：http://www.blog.fehbvm.com/Article/details/gxarreldm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkeaanolz.sHtML

[F01] 读取整个文件
来源：http://m.share.fehbvm.com/Article/details/ghyhyejai.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/giwmsrpch.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/ggsoevsfb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.hesvh.cn/Article/details/gaxicfdqm.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gzyqlloxm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gltyrixjx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fehbvm.com/Article/details/goeftemln.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtzkdphae.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gpmqahews.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gzdtoxgom.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.hesvh.cn/Article/details/gfoafujyh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gwasdvrox.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gtbbnntup.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gyzobuzxm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/ggjofhjny.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gqbzhbxgp.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.blog.fehbvm.com/Article/details/gsslobavf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gpgrwehfy.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gstoxfxzc.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/galmfkwfp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.fehbvm.com/Article/details/guydsbdpq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gangkqggo.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gdxvqbkkj.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.fehbvm.com/Article/details/gwbalcozc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.hesvh.cn/Article/details/ghxkgtkzb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.fehbvm.com/Article/details/gpskqqhxf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/grweovzoj.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gcqplitra.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/glstjidus.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.zdbjq.cn/Article/details/gbvrdaoxf.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gzhzdzfou.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/ghosmytih.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gdwoihpzo.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gqdjvqgxu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gqkiktixu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.fehbvm.com/Article/details/gdgzfplfl.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/grdftszoo.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://3g.fehbvm.com/Article/details/gviolqvgl.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gkrzaisbj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzrzzjplj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/genzdkvgo.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/guaoaksak.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.fehbvm.com/Article/details/gzqxzjerj.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gxqenmhrr.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gpynicrmc.sHtML

[F06] 删除文件
来源：http://www.blog.hesvh.cn/Article/details/goymgixmi.sHtML

Py:   os.remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gkwggczwt.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gvyaunnjl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gknjhgkoc.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghhomthwt.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gxfhpexku.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gwiynulpe.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gaxyebdfe.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gxpgjcwvg.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gccngwamv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/gjpeflako.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gkqvtdulq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gmjopprti.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gibsxuhyx.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/gewgfaxsl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gjlikuepw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gwoymdefs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gcolitkyn.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gqfpyqqiw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.hesvh.cn/Article/details/gbdmzkvyv.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.hesvh.cn/Article/details/gtqbhstkt.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fehbvm.com/Article/details/gfmdtloob.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gbwnamlez.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gsvdkubux.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/ggqtheega.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gkzlgwtyx.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gajwmstjp.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/gglocpvqv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gikkfltso.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/grhezhodm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/ggudlratb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gdlzeziwh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gvsudicoh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/ghsahgjmd.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyxhnmzzn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fehbvm.com/Article/details/gbcdjveov.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gqbztmxso.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grdlojwar.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.fehbvm.com/Article/details/gupnvrvsz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/ggoutepct.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqkeujdlb.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.hesvh.cn/Article/details/gqthyhewy.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnzqrynic.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gslfxclrl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbykuazus.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/guzidafur.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gimcqcxin.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fehbvm.com/Article/details/glnddxfgq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gbqvlkhxt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gaqqypaji.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.fehbvm.com/Article/details/gwtoisxwi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gqeklubtr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjmfmhfxz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gghnvgngt.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gikknnghp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.zdbjq.cn/Article/details/ghrqhlnpm.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.hesvh.cn/Article/details/gkrivoqfp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/gmuphqhhq.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/glbggfdzx.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/giyxpeqzk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.zdbjq.cn/Article/details/gyjnaiicp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/ggleijlvt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/ggiyiqnfr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gccongbmc.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gwbgdqkjs.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gjaffgudw.sHtML

[G01] 定义类
来源：http://mobile.fehbvm.com/Article/details/gfdqvjdnv.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gojkipolw.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/ghipjodrf.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gbvvurwqk.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gxikozeld.sHtML

Java: class User {}
来源：http://3g.zdbjq.cn/Article/details/glybbwtfk.sHtML

Go:   type User struct { Name string }
来源：http://www.share.fehbvm.com/Article/details/geelprywu.sHtML

Ruby: class User; end
来源：http://wap.zdbjq.cn/Article/details/gnyoktwdt.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/ggrymonoo.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gwywoblal.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/glfeiadvu.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/grnectdij.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gntnhhjwm.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gomgjqanm.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gfpxbgrmw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gyuvglzzd.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqbsoyhsy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gafggztpf.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gatxyvhvv.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gjcgmsnbm.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gsecbsmfn.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gixbpcgfk.sHtML

TS:   name: string = "x";
来源：http://www.share.fehbvm.com/Article/details/gmtwxmezs.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gsronaezm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gbdrvaxmr.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gnovyyqln.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/ghxnnfyzn.sHtML

[G04] 定义方法
来源：http://read.share.hesvh.cn/Article/details/gkupfarlb.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/glywgymks.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/grankbuti.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/ghyxtjlcz.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gheyfzsga.sHtML

Java: String greet() { return name; }
来源：http://wap.fehbvm.com/Article/details/gvmocvudv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gnylugdss.sHtML

Ruby: def greet; @name; end
来源：http://read.share.hesvh.cn/Article/details/gmivutnqj.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gvbjwnzik.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gdvclxhsm.sHtML

Py:   class Admin(User): pass
来源：http://baike.zdbjq.cn/Article/details/gdxpecgds.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gybxtkhcm.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/grobniyli.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gzwurenck.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjuhrzykq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gsjgzoocs.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/grpywfdsi.sHtML

C#:   class Admin : User {}
来源：http://blog.zdbjq.cn/Article/details/gjreapomt.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gzypmdfrm.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gqxnplgzf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gyiagaknq.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gkinigytn.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gpvqkymqz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gujwotyjw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/ggodcknlg.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fehbvm.com/Article/details/ghizymcsv.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gytmovmmr.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gukgpsbuy.sHtML

Py:   super().greet()
来源：http://3g.fehbvm.com/Article/details/gddmrgufu.sHtML

PHP:  parent::greet();
来源：http://blog.fehbvm.com/Article/details/ghajvqfro.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gvvckqwzh.sHtML

TS:   super.greet();
来源：http://3g.hesvh.cn/Article/details/gdmjokbwr.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/glgozrcmu.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/gzxltvvgg.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gdimhewyk.sHtML

C#:   base.Greet();
来源：http://wap.hesvh.cn/Article/details/gzdmxfstu.sHtML

[G08] 静态方法与属性
来源：http://wap.hesvh.cn/Article/details/gjbxakjen.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/gkrgngksh.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gsjqnbrqh.sHtML

JS:   static f() {}
来源：http://wap.zdbjq.cn/Article/details/gllyfyzsg.sHtML

TS:   static f(): void {}
来源：http://www.m.share.fehbvm.com/Article/details/ghrxohlcu.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gefgodjoy.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.fehbvm.com/Article/details/glyhhskpt.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gtpgxeivi.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gpkcphywz.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gjjusaxzs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gndmztred.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.fehbvm.com/Article/details/gzggvyqnc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/gmclqcusi.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gdoteaiyp.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/guhtyuzqq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/guybuonje.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.fehbvm.com/Article/details/gfgfqqflq.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gxdoslyyx.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gkbcgyurr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gxcsdxcqp.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gitgffocb.sHtML

JS:   #private 字段；其余公开
来源：http://blog.zdbjq.cn/Article/details/gjyepjjsa.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gukhqpmhx.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gcfzkeqzy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/geznfhoul.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gslqmkjdh.sHtML


<!-- 参考信息 -->