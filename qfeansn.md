代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gkyflpyjb.sHtML

[E11] 反转字符串
来源：http://3g.zdbjq.cn/Article/details/gasgkedys.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/gqlxxwcgz.sHtML

PHP:  strrev($s);
来源：http://wap.hesvh.cn/Article/details/gdibdwvab.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/grkjtonaj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gmlyvbsnq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gxcgipqme.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gmwsupdgs.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/ggxhkupmu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gmbstefhg.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/grpzspvwm.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gywaehysn.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gwfmtrono.sHtML

JS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/giocdzckl.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gsjxieupa.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gtyzddqfg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gbcoeirbf.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/guvzudmck.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.hesvh.cn/Article/details/gzjoicvdj.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/grzglruxv.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.zdbjq.cn/Article/details/gxddkjlyc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gujfgxyxf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gaisfywnl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gsspdxbcj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gaqbramvm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fehbvm.com/Article/details/gaaignccv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gnqpzjyti.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/glpxjdgik.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/gugcnpwlb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gooqmvlvf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.hesvh.cn/Article/details/gopmaskzc.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/glxksvwrm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gfxlsmqsu.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gfifboedl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.hesvh.cn/Article/details/grgqypshv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.fehbvm.com/Article/details/gnjehjcnw.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gtnlvwgtv.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/giaxgrkxm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fehbvm.com/Article/details/gfeuqwgsi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/ghrrnzong.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/gdkarwvxp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fehbvm.com/Article/details/gjdqbqyld.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.zdbjq.cn/Article/details/gdfmuriaa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.zdbjq.cn/Article/details/gjszfaufl.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gbxbjjapk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/guqmkeqki.sHtML

[E16] 数字千分位
来源：http://read.share.fehbvm.com/Article/details/gmiqiskej.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gldefalup.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/gvzafcanq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gflpnaogo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gqdvtfsca.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.zdbjq.cn/Article/details/grpxxysvg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gevpyrdpf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gpqitrrbh.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gazjlabqu.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gzxgifnya.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/glqzgtrls.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gbvsxedru.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/guftfuzig.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/gdvvrgojr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gjmbzdmzg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gyoqburfz.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gsddxfhhj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/gcittyguo.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gltzkhwyl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/grnnmiqpr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gehsiqqvj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gizuacsxw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/grvsmmhzb.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gqkkbdgog.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gxbuxgusl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gtakfiuyv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gonsfurwj.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gzwayfrdy.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/gdbkpwill.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gjxaochmu.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gydsczgaw.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/glyoenozd.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/ginwvvvlc.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.fehbvm.com/Article/details/gfiikvbkb.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gfxlqligu.sHtML

C#:   s.Split('\n')
来源：http://www.share.fehbvm.com/Article/details/gvudsnkoc.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gyzuafuwd.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gaxzafkdu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/ggmeiwmrh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gdcepkece.sHtML

TS:   if (s === "") {}
来源：http://baike.hesvh.cn/Article/details/gsfavvtpy.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.zdbjq.cn/Article/details/ggrwnbnej.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gjcapsuej.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/gzugdiwsa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gljparcuf.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gokewohki.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gxsnwsfit.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gwecxawtc.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gdpqkxzxl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gidkydtwb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/ggmnbhrep.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.fehbvm.com/Article/details/gmelzrobc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gffzxxyfr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gogtlizsj.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.hesvh.cn/Article/details/gxanglwjw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/grzlpdrpm.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gjvecpysv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gxdxprhzq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gixjvfiuz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fehbvm.com/Article/details/ghfkrcsdn.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/ggckidpmx.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/guktgwevr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.hesvh.cn/Article/details/ggatorpbh.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gtrdqnfsv.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/glzswsfbt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gkgcxichr.sHtML

[F01] 读取整个文件
来源：http://baike.zdbjq.cn/Article/details/gxqhhdfis.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.zdbjq.cn/Article/details/gvzmopzar.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/geiaxykyz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gostgrymx.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.hesvh.cn/Article/details/gixoxlzlt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gvhvhkocn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.hesvh.cn/Article/details/ggukiuyns.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gogyzrmmt.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmhnbjrja.sHtML

[F02] 逐行读取文件
来源：http://blog.zdbjq.cn/Article/details/ghslppbok.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/ghefsfmgv.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gowdatfmu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gyoagfxel.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gokodldzx.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gxubluuzq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/ggmpgmqpv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gqjdbgdkd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/glgowpsre.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gqsmqedlk.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.zdbjq.cn/Article/details/gwbhqqucs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/glkcyldnj.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gfghnrmpc.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gdtfkyqep.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gpbdipify.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/gnlhphkfu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gbcxcjnid.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/ggxrghufo.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gzfydedla.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gegvsjdmd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.zdbjq.cn/Article/details/grspiqiub.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gkydfaqwx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gwmvrfldn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gtecqkkrv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gyvfchovj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.hesvh.cn/Article/details/gpotespjf.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/ggubywqja.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gksvurxtw.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/gsjntnzlm.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gxskpisho.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gofsbgobg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbdzqvmop.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gaqsvlrhh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gvwmsonty.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.fehbvm.com/Article/details/gmqmyglgu.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxaiihteq.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/glsaazarl.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grtvruato.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gznaqlcoj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbeuapfaa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbwlhvgtp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/giclxwkrh.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gglribcav.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gukkopiid.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gmuwdlowy.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/ghdthdosd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.zdbjq.cn/Article/details/gyfyoqgcw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gzoetexcs.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gbcadjyew.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/grcjshckm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gsbnsnbgi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.hesvh.cn/Article/details/goijuaspv.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.fehbvm.com/Article/details/gwufpccki.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/gjzjuxbut.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gzlffqnar.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/ghzrxntpr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.hesvh.cn/Article/details/gvwjfhhac.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gjntisszl.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gjlphejto.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gnzatvbqd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.zdbjq.cn/Article/details/gwzxklwcn.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gcylvpfsj.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gmtmtbler.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gbheoxull.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glltgyxwe.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gugtwqddx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gfpocqgxy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gixuqgkck.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/ghqzaapac.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gfmgoemjx.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gdfbdtnrg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gpjmxglqw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/ggjhzpxjr.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gyevclmcp.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gnfgjibiu.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gkpkboiee.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gtkkwhkae.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.m.share.zdbjq.cn/Article/details/gtyalsppa.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzqlcayvq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gtohvbaua.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzjmnhgnt.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gwuxzbzbn.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/giqcyudef.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/giccuuauw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghipyxxgd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gcmkegccz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gfwglcdrs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.hesvh.cn/Article/details/gewltmimu.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gyvrobqvm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gcxoliejp.sHtML

[F12] CSV 读写
来源：http://www.blog.zdbjq.cn/Article/details/gqahqyoyb.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gceozlbiu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gsgyqznfl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.zdbjq.cn/Article/details/gymzechjt.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gkpwsejue.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gixxpmcqi.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/grubelfsk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gqmrfdfan.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gqwtxotes.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gberbmqkq.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/grgtvotmi.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glzmusens.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gsgttcwzn.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/ghzzsoqre.sHtML

PHP:  class User {}
来源：http://read.share.hesvh.cn/Article/details/gfdpbuhsw.sHtML

JS:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gggiwtzag.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/ggahwairl.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/ghfhdbiyw.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/ggkmkwtxr.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/gipjjdhzm.sHtML

C#:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gucbzdsyr.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gxgjkpkwj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gujvqxwwe.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gvkcudjbc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gzcmhwtlr.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/glyainnqb.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gtmthitpx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gzjsrcskw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.zdbjq.cn/Article/details/gtytpdtjh.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gzibrxzsx.sHtML

[G03] 实例属性
来源：http://www.share.zdbjq.cn/Article/details/grbtvhoms.sHtML

Py:   self.name = "x"
来源：http://www.share.fehbvm.com/Article/details/gljupbivx.sHtML

PHP:  public string $name = "x";
来源：http://mobile.zdbjq.cn/Article/details/gwkfkcokr.sHtML

JS:   this.name = "x";
来源：http://www.blog.fehbvm.com/Article/details/gqwglrwzh.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gliaufbtw.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gnspwxnpz.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gddfkazak.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gzbthtqat.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gbgsdabjj.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gzzlvbbjw.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gdmakebkh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbjwhqyro.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/garikgdhg.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gcutlandt.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghpylrzmc.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gcqmnocqe.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gwiysjspe.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gbpzerphc.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gbzabqwxf.sHtML

Py:   class Admin(User): pass
来源：http://baike.fehbvm.com/Article/details/gsxygkcuk.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gduajybkc.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gnrvgxpvf.sHtML

TS:   class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gbwnkzhvh.sHtML

Java: class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/ghnbrhxtb.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gbbawrwmh.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gcutmybgi.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gpvqynico.sHtML

[G06] 重写方法
来源：http://3g.zdbjq.cn/Article/details/ghrntubvy.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gyychcjhv.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gwbssohng.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gjbuvtmho.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gltqvwewj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/gbklktubt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gpupyiiel.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gftqojrao.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.hesvh.cn/Article/details/ggrhhbdyu.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gtyoktnwq.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gaeeardqi.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gmyryjpwa.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/gqdyrduab.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gxxajpesn.sHtML

Java: super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gickrtfln.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gsikkpnqa.sHtML

Ruby: super
来源：http://www.m.share.zdbjq.cn/Article/details/gxadxohsx.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gavkdzkxr.sHtML

[G08] 静态方法与属性
来源：http://www.share.zdbjq.cn/Article/details/gljpyxfbx.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gacifqgra.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gsfyofzcn.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/gniwvxbwj.sHtML

TS:   static f(): void {}
来源：http://wap.zdbjq.cn/Article/details/gdgbnfspp.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gvfsldkvj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gmyyaluku.sHtML

Ruby: def self.f; end
来源：http://mobile.zdbjq.cn/Article/details/gbysyuojn.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gdmrhthvu.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gokjswekj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.zdbjq.cn/Article/details/gwwylqylp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://3g.fehbvm.com/Article/details/gpcztlbxw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.zdbjq.cn/Article/details/gtirrjlhp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.zdbjq.cn/Article/details/gydukkils.sHtML


<!-- 参考信息 -->