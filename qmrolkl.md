代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/guxwtxmjy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/ggevcdeiy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gzzbbbovm.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gllcosnvn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gmgshdizp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/gxxmgnpvg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gbsmxdwgl.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/gfrpxvobr.sHtML

[E14] URL 编码与 Base64
来源：http://blog.hesvh.cn/Article/details/gtvymhjlb.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gzkyloeyu.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gxqgkvour.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.zdbjq.cn/Article/details/gpxmmvavk.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gbpjdvujq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/glmywaqkn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.zdbjq.cn/Article/details/gilzxjlzk.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gbhksnisn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gcuhltzjl.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fehbvm.com/Article/details/gptywjltp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fehbvm.com/Article/details/gxfioxhpx.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.hesvh.cn/Article/details/gmotdzjtt.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gupgoruio.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.zdbjq.cn/Article/details/grnkkbfie.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gbkfywdkw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.fehbvm.com/Article/details/gkslvspjc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gkqnhxdsn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fehbvm.com/Article/details/gpshmhqed.sHtML

[E16] 数字千分位
来源：http://www.blog.zdbjq.cn/Article/details/gdwdcwotj.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gbvdyrnsq.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gvgujkoci.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gxrxqvfdc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.hesvh.cn/Article/details/gongsrmbl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.hesvh.cn/Article/details/gtgcaunlj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.fehbvm.com/Article/details/gswlhlpdd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gaauqpgem.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/gqiyghiih.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/gbxpfwlvv.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gndlkwfjt.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gxsgxkhws.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gdkvtviem.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gsbepjovn.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gjckbckoy.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/gpspmwiii.sHtML

Ruby: s.capitalize
来源：http://baike.fehbvm.com/Article/details/ghddujuqk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gtebfdihy.sHtML

[E18] 模板占位符替换
来源：http://read.share.zdbjq.cn/Article/details/gecrmccam.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gdqdcyntr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gkdubqfnv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gdjmuzrvj.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gbvhhxjnh.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gczkusctf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gznvhllbd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.hesvh.cn/Article/details/gpokoeiqc.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/guzqeebpw.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gspgdmvrc.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gkfllkcbu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gwuwapkhr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gsubmhbug.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/gocrsqmya.sHtML

Java: s.lines().toList()
来源：http://3g.zdbjq.cn/Article/details/gfjmnfkcf.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.zdbjq.cn/Article/details/giricjgcx.sHtML

Ruby: s.lines
来源：http://read.share.fehbvm.com/Article/details/gkgufyawk.sHtML

C#:   s.Split('\n')
来源：http://wap.zdbjq.cn/Article/details/gnezyzcso.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gnozlpfdd.sHtML

Py:   if not s:
来源：http://www.blog.fehbvm.com/Article/details/grvyotejh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.hesvh.cn/Article/details/gddgdvhaj.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.hesvh.cn/Article/details/gklwogxcx.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/grtbzosot.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gvowmynfi.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/gtyxxlipp.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/ghopfqeli.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.hesvh.cn/Article/details/gwagvpulc.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gjvcxqxci.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/gzojuxieb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gqnqajqzq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gocvscnvh.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/gfmquypwk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkilmzpvd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.hesvh.cn/Article/details/gzmlezzjc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gfywnywco.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gjcuukowg.sHtML

[E22] 字节长度与字符长度
来源：http://blog.hesvh.cn/Article/details/gcmrxxnne.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.hesvh.cn/Article/details/gsprmbnot.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gkwfazhuv.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/gcequkqtq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/ghalkftwi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/geccbveky.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://baike.fehbvm.com/Article/details/grkmjeexq.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gswpjqfto.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gitqafqow.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gxpzcxipu.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gjovwhuvl.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtezjhxny.sHtML

[F01] 读取整个文件
来源：http://m.share.zdbjq.cn/Article/details/gomrhwmmk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/ghuymcmcl.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/grlavzejz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gmdybmolu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/glozhivga.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gergzjajj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gtthmgovi.sHtML

Ruby: File.read("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gixtxjzbp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fehbvm.com/Article/details/gfapzbaze.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gldwipkda.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/ggmhbotso.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gycacflzz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gfuejqtyz.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/gbpjpqdrn.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gyukhlhst.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gxqvwnyqr.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/gpjtjpojp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://read.share.fehbvm.com/Article/details/gpmzwdiqg.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gbnnfkrdl.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.fehbvm.com/Article/details/gkxxajjwq.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gzdxqcjhw.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/ghedecdih.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gbdmjveoo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gxrwfecgv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gbabutjpu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.share.hesvh.cn/Article/details/gtxtzyvix.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/geytzxuwp.sHtML

[F04] 追加写入文件
来源：http://www.share.fehbvm.com/Article/details/gxdisfpsi.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gcronqdnd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gxophglkn.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gthkzblnk.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gvjxsngnw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gmclgycew.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gatbiowod.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gjrcmmmfk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/gvcpppoki.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gfoonlhtd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gtdpikmou.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gizjvkkcm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfwvfhpwb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjciuqdcm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/glbgwziva.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/ggyhyzxcc.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/ggargfmgm.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyyopitox.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gzcahjbjc.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gaccdpohb.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gunvmucbc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gsuifvbaj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gcphomxje.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gskasjqdz.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggyqgibvc.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gybftzhlu.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gqndxpvix.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/ghiuueaiz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gzeggfmym.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.zdbjq.cn/Article/details/gfcmwqoef.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/guuxanvxh.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gakopvwki.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gdaqxtglx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gkudgteni.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gzhzzqlrv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.zdbjq.cn/Article/details/gvqgplzxa.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/gcnymuyrc.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/gfqsslgfe.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.zdbjq.cn/Article/details/gzskoieyc.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gpyarkruj.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gitwbvbgf.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fehbvm.com/Article/details/gisjrbigw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gwizgvekv.sHtML

Ruby: Dir.children("dir")
来源：http://blog.hesvh.cn/Article/details/gscxfenhb.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gwawlatqr.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gcbvkjyyy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gxbhzzrjl.sHtML

PHP:  filesize("a.txt");
来源：http://blog.hesvh.cn/Article/details/gbzhlschx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gxfywahhi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gatdxgxqw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gpjoavpln.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gkcmuyipy.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gptptapto.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gqqtgunjm.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/grsyrxcqy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnmruqqkz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gtkkeqxcf.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdinlvgbt.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.hesvh.cn/Article/details/goiccvkww.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gkbmnydst.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gbsznmvgc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqodmomfb.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gfeblxzgs.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gxczlbwlk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/govanknwb.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gnfkkjxqn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/guxhcnmzz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghnlubqsn.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gnauvhptw.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.hesvh.cn/Article/details/gozysbuvk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/ggiernwxq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.hesvh.cn/Article/details/gbbthphea.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gcdxyasfr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gupdpadyf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gdtxohrtf.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/gtagohrxq.sHtML

TS:   // 同上
来源：http://m.share.zdbjq.cn/Article/details/gkmegpuca.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gwwxcqjlk.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.fehbvm.com/Article/details/gwgrasavm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gmgmhzbpy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gorgoycna.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gazfblbxt.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gvewzbesu.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gueokwagm.sHtML

[G01] 定义类
来源：http://m.share.hesvh.cn/Article/details/gkzhmlyub.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gjfbthfkn.sHtML

PHP:  class User {}
来源：http://wap.fehbvm.com/Article/details/gbnsqzklm.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gbhtxuatz.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gwfzoiyrh.sHtML

Java: class User {}
来源：http://mobile.fehbvm.com/Article/details/gisfdgblk.sHtML

Go:   type User struct { Name string }
来源：http://baike.fehbvm.com/Article/details/ggppeisrp.sHtML

Ruby: class User; end
来源：http://3g.zdbjq.cn/Article/details/gzuogrwlo.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gajvnyifh.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gksnlozzg.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gqvbdgqxi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gencnhgpr.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.fehbvm.com/Article/details/gquhfcpeu.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gwsuihuxs.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gxhguxqjq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.fehbvm.com/Article/details/guoijfmba.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gpdvnbjut.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmmzqchmc.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gvyichgpt.sHtML

Py:   self.name = "x"
来源：http://read.share.hesvh.cn/Article/details/gbjzzwfsq.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gfiiknpsr.sHtML

JS:   this.name = "x";
来源：http://baike.hesvh.cn/Article/details/grmtjkjxi.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gfyipnbbp.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gqrgjekbn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gymgmtttu.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gwhxybnzc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/guazusgef.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gzxfjpnoe.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gpuacwxza.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gfhmxtuee.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/glnnetlwd.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gbkdcglvy.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/ghzvaabql.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/giuyeaelj.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gftisjogf.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.hesvh.cn/Article/details/gfdkezqyz.sHtML

[G05] 继承
来源：http://m.share.fehbvm.com/Article/details/gxzlpvlzk.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gwumzwrlm.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gdbpixelx.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/guckkposa.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gjbuogrlh.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gapixoabl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gliaowdij.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gpegknces.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.fehbvm.com/Article/details/gxqlqwwjy.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gjxrxicvk.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.fehbvm.com/Article/details/gxurwjqaj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/goytxayci.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gjtkvhdxg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnizjzklh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/goadhlavu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.zdbjq.cn/Article/details/gygmuiieo.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/grilyajsh.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gxishyqud.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gvgjwuvdh.sHtML

Py:   super().greet()
来源：http://wap.fehbvm.com/Article/details/gxdbjupyp.sHtML

PHP:  parent::greet();
来源：http://3g.hesvh.cn/Article/details/gddcvmoxs.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/geooegprs.sHtML

TS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gltsswnfv.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gttlhhujf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gkehbwsyo.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gdalkwoly.sHtML

C#:   base.Greet();
来源：http://read.share.hesvh.cn/Article/details/gihnucdtp.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gnhfutatg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/gsoqrfjmy.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fehbvm.com/Article/details/gidvuaumm.sHtML

JS:   static f() {}
来源：http://m.share.fehbvm.com/Article/details/gwcqwujen.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gqfwejhhv.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gtmqxgmsn.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gicccrgjs.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gzivqxswk.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/ggqdovmss.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gfjzmcqcb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gbyqtitzc.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gxboimfxw.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gajoiuapf.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gjbilqdew.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gyavcodvp.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.hesvh.cn/Article/details/ghhtbbgzw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gfaabjkzz.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/gitiemunx.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gtfkkhdvn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.hesvh.cn/Article/details/gizktxcnz.sHtML

PHP:  public / protected / private
来源：http://blog.zdbjq.cn/Article/details/gdgihnpbs.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gwyttwsgx.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/ggzaitbmh.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.fehbvm.com/Article/details/gbaakhuuw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gozppygef.sHtML

Ruby: public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/guzfrjdlj.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gsbijggwa.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gfltagsac.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.zdbjq.cn/Article/details/glzuvrbiy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/guvzsfmgd.sHtML

JS:   get name() { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gasapkppx.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.zdbjq.cn/Article/details/gskyfbgxk.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/girtjadrz.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gjfazldlz.sHtML


<!-- 参考信息 -->