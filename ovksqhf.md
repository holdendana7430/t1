代发 wailian999

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gldeorftk.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gkutfjhkh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gtiztxtcl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gvhggpssq.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/ghutulqpr.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gprshpwfk.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.zdbjq.cn/Article/details/gjoqlmhnk.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gvcgsomef.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.hesvh.cn/Article/details/gxfdebwqh.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gpaklktpp.sHtML

TS:   s.split("a").length - 1
来源：http://wap.fehbvm.com/Article/details/gfqezjwik.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gtoqnkoip.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gfufpiiaz.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/ggiwkqnhc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.zdbjq.cn/Article/details/gaannrgeo.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gsfgnihbc.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.zdbjq.cn/Article/details/gkrjkddas.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gonyhxikl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gjkwsloag.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gwqqmwkvz.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gisvypbyj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.hesvh.cn/Article/details/ggxmfaaja.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.zdbjq.cn/Article/details/gpjllernp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.zdbjq.cn/Article/details/gtyskldyf.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gwxunwltx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gzicpacwj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gvmkdwsng.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.hesvh.cn/Article/details/guwqzrypz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/gshbxcdga.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gvyurxbhn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gazxwtnnq.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/graadtelq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gmzdtjqar.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.hesvh.cn/Article/details/gbtxbrvfh.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gmvduejbq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gslybtskn.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.hesvh.cn/Article/details/giwwjcjdc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gmuilrefi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.hesvh.cn/Article/details/gspbazzuo.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gbhqmdxkf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gnvnojftk.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fehbvm.com/Article/details/gevlfhqcm.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gkbtauchf.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gyskkrdbk.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/giqicsain.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gwnnihmvd.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.hesvh.cn/Article/details/ggxudttkq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/giyszlbjx.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gwxyemrcp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gsqphafpm.sHtML

C#:   1234567.ToString("N0")
来源：http://www.blog.fehbvm.com/Article/details/gsiwftikn.sHtML

[E17] 首字母大写
来源：http://read.share.zdbjq.cn/Article/details/gtetdvifr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gnxnvtowk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.fehbvm.com/Article/details/gsqsicpyc.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gdikeilna.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gtqrvkkbg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.zdbjq.cn/Article/details/glhgazphj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gcdjzaruo.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/gqgvabgwn.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.hesvh.cn/Article/details/gporrvalc.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gfmrqrzwo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gwbypwpje.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/goceujmgs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gnodocqvn.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gejrgdtjp.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gqfpenfmc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gvshsusus.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/grrotlogj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/garffewuo.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gftyzalfe.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gwybhncnp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/ghbitileh.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gnaxwnext.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gxoyixoqr.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gfsjnrces.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/ghkmyzgyn.sHtML

Ruby: s.lines
来源：http://blog.zdbjq.cn/Article/details/gsjackbix.sHtML

C#:   s.Split('\n')
来源：http://baike.fehbvm.com/Article/details/goslxuzhv.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/grgwmzfuk.sHtML

Py:   if not s:
来源：http://www.m.share.hesvh.cn/Article/details/gvywfevvo.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gbeobmwsb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gyeyrqfzg.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gbvoakjfn.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gtbkooqan.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gvzmfvmlb.sHtML

Ruby: if s.empty?
来源：http://3g.zdbjq.cn/Article/details/gmbjvcqfw.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.zdbjq.cn/Article/details/gtptzqxnr.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/gownnhlrb.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gxapweuwl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.hesvh.cn/Article/details/giirkpove.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gmfwkvuvc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/ghaletvuo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gscqkpgzp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.hesvh.cn/Article/details/gacekufpp.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gairxkitg.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gkkklgymy.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.hesvh.cn/Article/details/ggtsgunoe.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.hesvh.cn/Article/details/ggndvxjvw.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gdydlohhv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/gnqtebibc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gqepdjecy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gkgcehmpw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.fehbvm.com/Article/details/gjghwksnq.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gemlflivn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gfinguidw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwdchtdpo.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/guxzcrurj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyhbacaau.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gwmtmqifg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/ghnlotbso.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/ghbitwgke.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/ggsxgucme.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.hesvh.cn/Article/details/gdxdnyowy.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gvhuynqbo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.fehbvm.com/Article/details/goxzqkkuu.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxwqaercm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gpgnefguy.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gmvkyglsd.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://m.share.fehbvm.com/Article/details/gisrkwmia.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/giwkxykcd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gavotjzyo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/gmmpvtoqr.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gshrgsrtn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gcfgxuaej.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gdzbgdjaw.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/grbhhaxcq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gvjpgxxum.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gebgfsjzu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gfwtqqkof.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.zdbjq.cn/Article/details/ggrsemjvk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.hesvh.cn/Article/details/gnlnlqvfr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gygvopikn.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/glkrbpiit.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/ghuoyiuqy.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/grhfaprqh.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gniivxvgl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gevcawtwu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.hesvh.cn/Article/details/ghskjzbtk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/ghnaoowlc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gsxggstfh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.zdbjq.cn/Article/details/gscyghdus.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/ghzhqnnaq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gjhyukxbw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gnkgsxnsa.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gcwrklmpn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gwvjdkpek.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gikjgnryi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gctcfpixw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gwxnntrgn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gixqpnvxp.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gvulifzff.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gytvlikul.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwmgjsxgf.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gvimpjgcw.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gudqjtiew.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gewabhmsi.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gdcjnczpn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gwnqoxhrq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gcwaliuaq.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gzthzvzmb.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gnsrucxez.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/ghcfwkudm.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gqytwxlsp.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gtrwvsgim.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/guquerxtb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/ggiygwiqj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gajlashci.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/gxnxueszq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.hesvh.cn/Article/details/glkmqqlpu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/giptvmfsl.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gmiamzeco.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/ggmpfpjeq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gaoqanbxj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gfhgnjfdn.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gzjsccsci.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gjmufwsfb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/gxhwarngq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gqafguhlg.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gxybadqib.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/ginmkfuam.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gkpfhhals.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghaszepso.sHtML

PHP:  filesize("a.txt");
来源：http://baike.hesvh.cn/Article/details/guueqyrwl.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/ggfqpmvhn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gtelvjifx.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gkhuvwnzk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.zdbjq.cn/Article/details/gzpkuoafu.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gwaqvijpy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gqytjrpvs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gohrtlbds.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gvranhznc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gvgwppsds.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gevndmxxh.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwmsiroft.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gavrohzsb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gifnlpsdd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gtogmadob.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gryzdvxdz.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gcgoktegr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gaopzkogu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gwxrhcwop.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gwuckwlmd.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gutjpqrmo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fehbvm.com/Article/details/gglsyvrly.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gbybsxafb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/geddjduhc.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gkqgirdpu.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gaebkqlwk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.zdbjq.cn/Article/details/gczssisen.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/giylgwhwm.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gttrottuy.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/glfzqotto.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/gkoytuuac.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/gwnclpncq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gyjhjnufj.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gtuzdmibm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzqtpufoh.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/gqkjmafma.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmucvssjg.sHtML

[G01] 定义类
来源：http://www.share.hesvh.cn/Article/details/gnyezaion.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gtvbzwazu.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gpvmcydej.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/glflmmprl.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.hesvh.cn/Article/details/gawccnkfw.sHtML

Java: class User {}
来源：http://3g.fehbvm.com/Article/details/gzpwsbqaf.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gfsekmmgo.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gtltwjhbz.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gprltxfps.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/ghhnamzpt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.hesvh.cn/Article/details/gssthlipf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gvsxcftqy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gjzaqgpag.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghvefzidh.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/grifqpled.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fehbvm.com/Article/details/gqvehsvaw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.zdbjq.cn/Article/details/gkulkvjjw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gowjhnmyo.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/guvkchbfn.sHtML

Py:   self.name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gfawlgjxh.sHtML

PHP:  public string $name = "x";
来源：http://3g.fehbvm.com/Article/details/ghzjaddjl.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gfnzosbry.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/grkxebdpx.sHtML

Java: private String name;
来源：http://mobile.fehbvm.com/Article/details/gsgbqmtdm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gxnotnvsu.sHtML

Ruby: @name = "x"
来源：http://3g.fehbvm.com/Article/details/glbmndoul.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/glkbocbmh.sHtML

[G04] 定义方法
来源：http://www.m.share.hesvh.cn/Article/details/gegdcdkkk.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/grrabjxmc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gddojsdzn.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gnkibijgw.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gsbrrivlb.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gngsmthlk.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gqmdwgmie.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gagttciwb.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.fehbvm.com/Article/details/gqrtistgg.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gqnvmafig.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gnupsffhv.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gjkenacdy.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/ghtjdqnxb.sHtML

TS:   class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gzbmlufxq.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gzsxqvyrm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gonywhsem.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gbaojazen.sHtML

C#:   class Admin : User {}
来源：http://baike.fehbvm.com/Article/details/grhrgngbo.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gtoczinmw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gvjbujkmt.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gynhzrmll.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gqakbciyx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gniwgjviz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbgyauhay.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fehbvm.com/Article/details/gknagoonv.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gtxidwikr.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gkqupdvuz.sHtML

[G07] 调用父类方法
来源：http://www.m.share.fehbvm.com/Article/details/gdcfcxhui.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/gxsuvnuue.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/ggidbpyfr.sHtML

JS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gdipljfuj.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/ggiwjugvp.sHtML

Java: super.greet();
来源：http://read.share.fehbvm.com/Article/details/ghwksbsbj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gttavvgux.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gtqywrkbl.sHtML

C#:   base.Greet();
来源：http://www.m.share.fehbvm.com/Article/details/gevzbwljg.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gewgjguvn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gjuxoezaz.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gmnkftyze.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gxnlmxefc.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gybeorspp.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gksramvmc.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.fehbvm.com/Article/details/grchmzxsw.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gntkyifjp.sHtML

C#:   public static void F() {}
来源：http://www.share.fehbvm.com/Article/details/ghmmevxzn.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gibfbajmn.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gmgddluoi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gjfppdqud.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.hesvh.cn/Article/details/gmoktagjx.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gpqtcevsq.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.hesvh.cn/Article/details/gciqylhvi.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gctabgxak.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/grdhscxtu.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gbinydwag.sHtML


<!-- 参考信息 -->