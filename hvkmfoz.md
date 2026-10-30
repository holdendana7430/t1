代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gvfdqxuhn.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwnwgedl.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzvteslj.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpatwstc.sHtML

Ruby: s.reverse
来源：http://www.share.fanxiaobao.xyz/Article/details/gvysjmqsl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fanxiaobao.xyz/Article/details/gnrzbdpxk.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fanxiaobao.xyz/Article/details/giurqvqih.sHtML

Py:   s.count("a")
来源：http://baike.fanxiaobao.xyz/Article/details/gxbbjcnyy.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwctuxrx.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvfqnhai.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fanxiaobao.xyz/Article/details/gqprlaqlt.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fanxiaobao.xyz/Article/details/gsabckxbd.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbkkdqrn.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrygvtwg.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.fanxiaobao.xyz/Article/details/glnpnzqpx.sHtML

[E13] 逐字符遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gufctqcyd.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fanxiaobao.xyz/Article/details/gupwdllvf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcypqctm.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fanxiaobao.xyz/Article/details/gfcuemoto.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghgroowbl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzslmadzf.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gektpnzmo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fanxiaobao.xyz/Article/details/gvihapqyg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctqwdldf.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gntimllnz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guikozfee.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoxvefex.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guhdiuaag.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gmboihofj.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszicgesl.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fanxiaobao.xyz/Article/details/gwgronkjw.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fanxiaobao.xyz/Article/details/gvydkrjwv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbxmykwt.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fanxiaobao.xyz/Article/details/gsviloptc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbbfzfgz.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsleposz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gqkhiqvia.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gdfwvsuno.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnkfbqew.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxipplfh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/guskajvzj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fanxiaobao.xyz/Article/details/ggjeerson.sHtML

[E16] 数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/gcruqsmtq.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbietlben.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxidjvgef.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fanxiaobao.xyz/Article/details/gvyueqjsz.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fanxiaobao.xyz/Article/details/geysrdmeo.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcydbhwcu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fanxiaobao.xyz/Article/details/gilhnhwua.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxhygont.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fanxiaobao.xyz/Article/details/gfqkkthtg.sHtML

[E17] 首字母大写
来源：http://www.share.fanxiaobao.xyz/Article/details/gazgeweyd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fanxiaobao.xyz/Article/details/giorfcdzf.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gjfhjtwnt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gtmnqhgnc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/giwtuxnlq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gmkvsdneo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gzgmsbqqe.sHtML

Ruby: s.capitalize
来源：http://blog.fanxiaobao.xyz/Article/details/ghbbnskbr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrxdzflq.sHtML

[E18] 模板占位符替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxifualh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygvascic.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggmnthfyt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gaigkeoys.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gapcmonbe.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/guahoequa.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gawgrowsc.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fanxiaobao.xyz/Article/details/gneboczro.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkbyhsdpo.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugvqvgvp.sHtML

Py:   s.splitlines()
来源：http://m.share.fanxiaobao.xyz/Article/details/ghiciennb.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpzmtprw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkjfkyor.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxalptgr.sHtML

Java: s.lines().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdjlxjoz.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/glhfecdpn.sHtML

Ruby: s.lines
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgxbhhlc.sHtML

C#:   s.Split('\n')
来源：http://3g.fanxiaobao.xyz/Article/details/gvdbzidqz.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fanxiaobao.xyz/Article/details/geslkabgh.sHtML

Py:   if not s:
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkolmoqc.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fanxiaobao.xyz/Article/details/gfduoelzb.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gdjjrqria.sHtML

TS:   if (s === "") {}
来源：http://baike.fanxiaobao.xyz/Article/details/gpfygqpzk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/goghkibvv.sHtML

Go:   if s == "" {}
来源：http://baike.fanxiaobao.xyz/Article/details/gpqnejcuj.sHtML

Ruby: if s.empty?
来源：http://baike.fanxiaobao.xyz/Article/details/gfezefntd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcliuyaqw.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fanxiaobao.xyz/Article/details/gbuenlldh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhtfygmu.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gdczbpyen.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gespovuvd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fanxiaobao.xyz/Article/details/gthqdqaym.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gyyhystqp.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fanxiaobao.xyz/Article/details/gbdxfqluf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzuzrhrw.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gnvqpyeyp.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fanxiaobao.xyz/Article/details/gjqlvmxmr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmiildai.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxitdquv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gjlrftnnp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqaefrpf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzyytwxv.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgunjgbe.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/guixjutli.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fanxiaobao.xyz/Article/details/gzpvargbd.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glufemikv.sHtML

F. 文件与目录
来源：http://3g.fanxiaobao.xyz/Article/details/gxozlomyg.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gssrvyydc.sHtML

[F01] 读取整个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxkykgkqv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxowocvde.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhdieqgz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fanxiaobao.xyz/Article/details/gwujkwdbb.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fanxiaobao.xyz/Article/details/gylsdekov.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdodullqv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fanxiaobao.xyz/Article/details/gzottirkw.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gqbqgghej.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gsiaqevpg.sHtML

[F02] 逐行读取文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmlcujakk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fanxiaobao.xyz/Article/details/gczlhgfad.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkruwilrp.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gxtzstrsc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gmkogvbgi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.fanxiaobao.xyz/Article/details/gskinyjga.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.fanxiaobao.xyz/Article/details/gmlgizfad.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.fanxiaobao.xyz/Article/details/gntrqkvqu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fanxiaobao.xyz/Article/details/gijazpcgo.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fanxiaobao.xyz/Article/details/gblkyevui.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.fanxiaobao.xyz/Article/details/gwzdktmef.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmsyxdpc.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoammhgg.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggofcjvsz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghcigwyyq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcwknwbg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqclmmkw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhqhajem.sHtML

[F04] 追加写入文件
来源：http://wap.fanxiaobao.xyz/Article/details/gyylwuwuq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gtpekyirl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqayvybeg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fanxiaobao.xyz/Article/details/gojgkyfhw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gloypjvra.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlexkxem.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gisjgqkko.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzhzibtk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrbauxdo.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjuxuvhs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqkuvgew.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/ggnptqydl.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkyihehh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjpgvuyk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghfqprggq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fanxiaobao.xyz/Article/details/gjvllupao.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvpbnfbn.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gkmungmmo.sHtML

[F06] 删除文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbsxcehas.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gteeccumq.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gmdplrgpu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfvndgis.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gjqzocovn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfyvaxjs.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gslmraetp.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifzvblsi.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuypfoco.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwjegoya.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobqzacej.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoqkmiow.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gkizqrxlt.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gzwecltyp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqgeksmd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fanxiaobao.xyz/Article/details/grzjfdjao.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fanxiaobao.xyz/Article/details/ghbfohzra.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdxtibsh.sHtML

[F08] 遍历目录
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgfuwuus.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvvxrvyz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghuudvesj.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/grzsapsba.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gutvvlztq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmwjtqmm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwciglws.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/guvuhormr.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgnwtoda.sHtML

[F09] 获取文件大小
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjtlilqp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gemarnxwe.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdiuxjwwz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.fanxiaobao.xyz/Article/details/gcyhkhqcn.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fanxiaobao.xyz/Article/details/ghzsucnnh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fanxiaobao.xyz/Article/details/gghidjdvc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fanxiaobao.xyz/Article/details/gelknxqft.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljylyphv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fanxiaobao.xyz/Article/details/gsesphfxx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxtakwfrw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwjdqlbbr.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/goardkuho.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gnykazyof.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gvkzauinm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fanxiaobao.xyz/Article/details/gpjgkgrbo.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnlgfpuhy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/glztidfyo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gmjmjhmmp.sHtML

[F11] 复制与移动文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghhtmbbki.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfnideyc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gyefipfby.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gbxasepzj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gbssnycah.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlwpcpjx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fanxiaobao.xyz/Article/details/gsshrcroc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gbimmrsvs.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcxfhrcs.sHtML

[F12] CSV 读写
来源：http://mobile.fanxiaobao.xyz/Article/details/gfqxjperw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fanxiaobao.xyz/Article/details/gapxftueo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpzhvauu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fanxiaobao.xyz/Article/details/gkgtggumv.sHtML

TS:   // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/gevvuimem.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fanxiaobao.xyz/Article/details/gndkkrggm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fanxiaobao.xyz/Article/details/ggiwqghhf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcyvswtcd.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fanxiaobao.xyz/Article/details/gyljfrcoi.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gncmivwar.sHtML

G. 面向对象
来源：http://3g.fanxiaobao.xyz/Article/details/gxlrjbztl.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcimxrtyb.sHtML

[G01] 定义类
来源：http://wap.fanxiaobao.xyz/Article/details/gfxsjhupb.sHtML

Py:   class User: pass
来源：http://mobile.fanxiaobao.xyz/Article/details/grknxvytm.sHtML

PHP:  class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gsklilgen.sHtML

JS:   class User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnskikyyk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnanqpwty.sHtML

Java: class User {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gobczutqm.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqefphxye.sHtML

Ruby: class User; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxrqxirn.sHtML

C#:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gplcwbflp.sHtML

[G02] 构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkydmank.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqptheeg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveqmdzhl.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkvmedih.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwjdjjuu.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxtosrcq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdxqcafmm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gisxqpatk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtjmevgj.sHtML

[G03] 实例属性
来源：http://3g.fanxiaobao.xyz/Article/details/ghjcyjitq.sHtML

Py:   self.name = "x"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjvfjxoq.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwwjgoxy.sHtML

JS:   this.name = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/givvjpuoq.sHtML

TS:   name: string = "x";
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoiosknv.sHtML

Java: private String name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxebldbk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyiwwvjx.sHtML

Ruby: @name = "x"
来源：http://wap.fanxiaobao.xyz/Article/details/gjskyisws.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaqhkdjo.sHtML

[G04] 定义方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjaxyamy.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fanxiaobao.xyz/Article/details/guqrvywrr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmcyhant.sHtML

JS:   greet() { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmdzqtjd.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxvpwjzsb.sHtML

Java: String greet() { return name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdqtxclqi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gmkjcolcv.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfwkwbpv.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fanxiaobao.xyz/Article/details/gemcudwxp.sHtML

[G05] 继承
来源：http://3g.fanxiaobao.xyz/Article/details/gcbkbksna.sHtML

Py:   class Admin(User): pass
来源：http://3g.fanxiaobao.xyz/Article/details/gqhqlloek.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcrmuafkn.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmzurlzd.sHtML

TS:   class Admin extends User {}
来源：http://baike.fanxiaobao.xyz/Article/details/glolzlyut.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdohxbee.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpznxuaa.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fanxiaobao.xyz/Article/details/greuohebo.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxldmqbpb.sHtML

[G06] 重写方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjzmwgde.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkjuhonz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbstntwqv.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxzelhja.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcorqjplm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ghrtmxctp.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.fanxiaobao.xyz/Article/details/glbritrio.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdqanvfx.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fanxiaobao.xyz/Article/details/glvsxfdqp.sHtML

[G07] 调用父类方法
来源：http://blog.fanxiaobao.xyz/Article/details/ggnvmdqaz.sHtML

Py:   super().greet()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegyemocd.sHtML

PHP:  parent::greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbmbnyqq.sHtML

JS:   super.greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gvimndgfw.sHtML

TS:   super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdluioja.sHtML

Java: super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gmukrrwaf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.fanxiaobao.xyz/Article/details/gclqdjvvt.sHtML

Ruby: super
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgrcozue.sHtML

C#:   base.Greet();
来源：http://mobile.fanxiaobao.xyz/Article/details/gumczafgy.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhgjcjrp.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.fanxiaobao.xyz/Article/details/gwzyfqzbj.sHtML

PHP:  public static function f() {}
来源：http://3g.fanxiaobao.xyz/Article/details/gkuozvqma.sHtML

JS:   static f() {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdryqrxcq.sHtML

TS:   static f(): void {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gdeqqswch.sHtML

Java: static void f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfkehwva.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.fanxiaobao.xyz/Article/details/gndhtjemt.sHtML

Ruby: def self.f; end
来源：http://read.share.fanxiaobao.xyz/Article/details/gwihndvkq.sHtML

C#:   public static void F() {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmrjiczs.sHtML

[G09] 接口 / 抽象类
来源：http://3g.fanxiaobao.xyz/Article/details/gbbovggme.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaajdciyd.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gqamtvmft.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fanxiaobao.xyz/Article/details/gmjwausdp.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibwrkcnw.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fanxiaobao.xyz/Article/details/ghteoxydj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fanxiaobao.xyz/Article/details/gcleyxcfx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fanxiaobao.xyz/Article/details/gppaouxid.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/glrugdpck.sHtML


<!-- 参考信息 -->