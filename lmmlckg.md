代发 wailian999

JS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gmedjxfvh.sHtML

TS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gidyulymt.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gszwahfda.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gkeazdsaq.sHtML

Ruby: s.reverse
来源：http://www.m.share.fehbvm.com/Article/details/gtytfivtp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/ghtvpjqtr.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gdwgmtmjx.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gzkgllogo.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gxffwxybb.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gxbcvzbwl.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gywubpgng.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.zdbjq.cn/Article/details/genvvnvux.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gejpzqgcy.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gtrczdggy.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/grzxbzokf.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gvbpryxxh.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.hesvh.cn/Article/details/gzhazhzyn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gjgdtwkpi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gqkzgxkqo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gnscocdto.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gykequufj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gktjcydmz.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gscgrlvvn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gcbczuytq.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.hesvh.cn/Article/details/gyksmqtqs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gtoiwtici.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.hesvh.cn/Article/details/ganekyccq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gliyaazgs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gkxeikjnf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/giacbsomj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gsxnlgqvv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/geaubcumc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gncxfldzn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gvwhdemnb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gfccvdxni.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gnlszhzeg.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.hesvh.cn/Article/details/gvewjehvh.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/goaysdkcj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.zdbjq.cn/Article/details/gjsgvjqhq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gqqzqxgmu.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpwdisqzv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gzrrywlok.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gppeytyso.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gehkcylbt.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/giereouay.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/gjwjrigfq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gckuqnzfg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/gygkqvnls.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gdpadseeo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.hesvh.cn/Article/details/gyfzonhst.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/getmizbni.sHtML

[E17] 首字母大写
来源：http://read.share.hesvh.cn/Article/details/gtsquklpp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.zdbjq.cn/Article/details/gpbdmtzsz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gxkxrmoxk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gbnpygjch.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gqcqwybbr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.hesvh.cn/Article/details/gtwyurhoc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.fehbvm.com/Article/details/gewfiytug.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/giuqodcnk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gpcuqohex.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gaiiuivrk.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gbijlyjev.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.hesvh.cn/Article/details/gebagmkgu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gzbtfpsib.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gwlxrvjah.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gnkspfyjd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gbqkjklrr.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.m.share.hesvh.cn/Article/details/gnbxngibf.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fehbvm.com/Article/details/gytmtbhmu.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gxtvgbeqc.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gcxwbcqgs.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.hesvh.cn/Article/details/gtxtuyytx.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gjmgrvshi.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/guaywpurt.sHtML

Java: s.lines().toList()
来源：http://mobile.fehbvm.com/Article/details/goslxuafg.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gedoxopaf.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gnaanpsnd.sHtML

C#:   s.Split('\n')
来源：http://3g.zdbjq.cn/Article/details/gqqlcbjed.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/glzjdftzc.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gfwdhzgmb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gapqryxqa.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.hesvh.cn/Article/details/ggwwgffbl.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gyennaexm.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/guuntzfuy.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gxkhuksgy.sHtML

Ruby: if s.empty?
来源：http://www.blog.hesvh.cn/Article/details/grkebsyoc.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/gnmljwiin.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gtgdfodhw.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gmuthenfw.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gkiueyhom.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gvckltoky.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gdiibyoqe.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gdbmprytv.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.zdbjq.cn/Article/details/gdewjzwdj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gouztzdsv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gkmyllcrt.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.hesvh.cn/Article/details/gppgcmgxj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gzockfamj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/grvlqbcfy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gfibzjvyq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.hesvh.cn/Article/details/gscugwxda.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gphshzkak.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gnkhbkdxj.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gogqlqqsm.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://read.share.zdbjq.cn/Article/details/gpfxkdqwq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gybqwbplp.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gakxjoryk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjeaqjqhe.sHtML

[F01] 读取整个文件
来源：http://www.blog.fehbvm.com/Article/details/gtemqehwx.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.zdbjq.cn/Article/details/gxqjcilja.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gejedkxps.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.hesvh.cn/Article/details/gzsqjfpba.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gbnzjghti.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gioosyfnm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.hesvh.cn/Article/details/gtivzhaor.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.fehbvm.com/Article/details/guzfxfdvm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gtmkovdup.sHtML

[F02] 逐行读取文件
来源：http://mobile.fehbvm.com/Article/details/gcqnmevxn.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gxwgpriwn.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gojhwoiae.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.zdbjq.cn/Article/details/gxthymtqe.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gatdgpdgc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gxwhlugpx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.fehbvm.com/Article/details/ghubigfxs.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvdcnkao.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gniurpfyq.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gkabivkrl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/guxpmfsbs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.zdbjq.cn/Article/details/gwxypnyre.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/gjqpmuqsx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.hesvh.cn/Article/details/giwiolpcs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/glzofrshl.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/geaghnxue.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/ghurphjpd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.fehbvm.com/Article/details/geoluayfw.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/goeprowsy.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gzyreugpu.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gsomtvmuh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gjzwcmher.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gqmhhpqpn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/ggpcfnpnq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gmzfefske.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gxhprwflp.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/gaobutfbu.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/gnsuntjft.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gamigarmv.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gajrtagew.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gepmntboc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grtjaojiu.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gitukktqj.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gtfgckpiu.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghztwlaun.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gifmwheut.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/glwwkxmpe.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcpyhytmx.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gwmaslukn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkxjdcjqf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gqapeyyso.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gueckcwwy.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gemokazyj.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdoflvqyd.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gpcrllhme.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/ggglhivdk.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.fehbvm.com/Article/details/gfgzebkft.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/geqksttld.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/grsiquzrr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/gqkwzeqjq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gyienywoe.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gvrjkzurw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gadrhvaus.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gjcywfmsk.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gsetzxaxb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/ghupflwyk.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/guakubjjg.sHtML

JS:   fs.readdirSync("dir")
来源：http://mobile.fehbvm.com/Article/details/guvvnadrh.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gnfagjeol.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gejugnjwx.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gnndmhzmq.sHtML

Ruby: Dir.children("dir")
来源：http://blog.zdbjq.cn/Article/details/gxasngiep.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fehbvm.com/Article/details/gsjcvdmna.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gvjdilyzk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/goohzlttc.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gtsbxptns.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.fehbvm.com/Article/details/gqvihyare.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gpzmbecdy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gjvqidbmg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://3g.fehbvm.com/Article/details/gvsluglaa.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gifbmjlhk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gdidnadoo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gzyqnogxv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gpieqlbyn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gwggpbqtv.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/giwsuqdcj.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtgrdnawv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.zdbjq.cn/Article/details/gohtmnmmq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gwsnqcmkz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gsujsquur.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gbnviipva.sHtML

[F11] 复制与移动文件
来源：http://mobile.zdbjq.cn/Article/details/gaweiijmt.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gikwdbset.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gjzvzizub.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gjncvskla.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gsydxfuzk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gkfbnwwwq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/gehupqxta.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gefdartyo.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gqpzydylg.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/glporaids.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gilpjewwc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gdjladabc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gdnmxozwr.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gacmetbln.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gzoffqgio.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.zdbjq.cn/Article/details/gwiilnxoj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gibbfzuua.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gofmknwwg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ghmzsxmvu.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gixsfdbzw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gnudinnzv.sHtML

[G01] 定义类
来源：http://wap.zdbjq.cn/Article/details/gntsudqsh.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/gguqpvikl.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gpntrkeoo.sHtML

JS:   class User {}
来源：http://3g.fehbvm.com/Article/details/grgwotlun.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gdwsfavsz.sHtML

Java: class User {}
来源：http://www.share.hesvh.cn/Article/details/gmzmptwxy.sHtML

Go:   type User struct { Name string }
来源：http://wap.hesvh.cn/Article/details/gcccwamox.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/guofqtzmh.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gueefeoub.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gnibbllsd.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gpvtpcden.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gppteagxe.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gbkbfdjxi.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/geczbbqjb.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.zdbjq.cn/Article/details/gyfpdrerq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.fehbvm.com/Article/details/grjgnfylf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/guggeijgj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gxoswqrqu.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/ggqxubrhe.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/grkjgfbyd.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gljvzrgty.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/ggersxoyn.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gugsmsgvs.sHtML

Java: private String name;
来源：http://m.share.fehbvm.com/Article/details/geqhkgzxi.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gxrrslhhq.sHtML

Ruby: @name = "x"
来源：http://baike.fehbvm.com/Article/details/gisjwkdiu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/glelhqpob.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/gczqyyalx.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gokbrjeqr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gdaiigelz.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gbcnmtsmo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gcdjecnrs.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gzsgkbfem.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gyspjfsru.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/glzhfocmw.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gnljaioyv.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gbthqwrgy.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gmurnouuj.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gazdbzrvh.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gwhifcdoy.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/gxgoaakng.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gtwbwvmli.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.hesvh.cn/Article/details/gepzjzlme.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gyqfrgrrc.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcldtcizv.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gugfdfcni.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/gmatijbiu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/geaseknyo.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gjvtfpkuk.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gsmckcumc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/grblsrwdq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.fehbvm.com/Article/details/gngavxjsw.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gmjldbwfg.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gabxbfnsc.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gtrcodnww.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gdefraets.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gussxkcun.sHtML

JS:   super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gacyvjxft.sHtML

TS:   super.greet();
来源：http://www.m.share.fehbvm.com/Article/details/gfdsbowwt.sHtML

Java: super.greet();
来源：http://blog.fehbvm.com/Article/details/ghhvindse.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gjxxquphu.sHtML

Ruby: super
来源：http://read.share.hesvh.cn/Article/details/gqaitrety.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/geedpzkmu.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gtyyevkrl.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gifhryiae.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/glggopkyp.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/gotquuttp.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/grzvihxea.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gxvjzwagn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.blog.zdbjq.cn/Article/details/giiqoooqb.sHtML

Ruby: def self.f; end
来源：http://baike.fehbvm.com/Article/details/gjbcpsdmr.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gsnfakrnk.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.fehbvm.com/Article/details/gaxverfwq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.hesvh.cn/Article/details/gwsrlwzvn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.hesvh.cn/Article/details/gcavpyske.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.hesvh.cn/Article/details/gxpqavxfx.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gwopwsftf.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gsdgnaflh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gcuuyyngo.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/gevqlyawz.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gnuinfvgu.sHtML


<!-- 参考信息 -->