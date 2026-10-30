代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/giixmkulc.sHtML

[E11] 反转字符串
来源：http://mobile.fehbvm.com/Article/details/gzoqzrjta.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gxxsyccfl.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gkcpdpjyv.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/ggorktdne.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gxnjvtooh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gwdimmhyo.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/ginqtxtde.sHtML

Ruby: s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gvtllyiai.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gbhabaoci.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/geztpmvpk.sHtML

Py:   s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gsrauyijs.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fehbvm.com/Article/details/ggkzyoczb.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gzgtnparz.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gtanqdqeh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gtaatxhah.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/gfrrsgddn.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gbodhzawx.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gdcisckwm.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gffqqwtng.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gkwfjyzlf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.fehbvm.com/Article/details/gxzupmkvp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/getfwvutz.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gaitctxpa.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gehugumkx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gmdwnvkuo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gjzuiytbg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gpovwifaa.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/geaxssuai.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gdemmtdic.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gmmawaciu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/ghqcdgpbi.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.hesvh.cn/Article/details/gvwtqxdxd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gjyqyeftd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gnmtspxap.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gthbluwyh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gulzwusdw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gkxnfyieo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gfzykiwjd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gvzynnirs.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.hesvh.cn/Article/details/gtisslbun.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gtdequuja.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.zdbjq.cn/Article/details/giburafyj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gmxgbijff.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdhmxmluh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gwsutdysv.sHtML

[E16] 数字千分位
来源：http://mobile.zdbjq.cn/Article/details/gvhldrncq.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gvmalaszd.sHtML

PHP:  number_format(1234567);
来源：http://3g.zdbjq.cn/Article/details/guzohhknw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/gezntdqjx.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gyntsusud.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.zdbjq.cn/Article/details/guflwwawv.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/gzjzdwayp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gyimilrsa.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.hesvh.cn/Article/details/gjeebxsxt.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/geayeilyr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gjkhuawqx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gjhvyvkmp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/grixoxldn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gosgslysy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfihothgs.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.hesvh.cn/Article/details/gthvhahdc.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gazaeojsd.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gcynzcuoe.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gocrftlld.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gcxmiilkm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gschsiclm.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gutbmmagh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gbqqzimtg.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gsukzodda.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/godcrvhef.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://wap.fehbvm.com/Article/details/gxdyiukba.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gidbsxbrt.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.hesvh.cn/Article/details/gtchqcxif.sHtML

Py:   s.splitlines()
来源：http://mobile.fehbvm.com/Article/details/gkmclkuoa.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gxglrtzqb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/giwfddqtp.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/giabeoucj.sHtML

Java: s.lines().toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gjfdwqgch.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gfoxtikwe.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gbepbfcpe.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gihgqrtff.sHtML

[E20] 判断字符串是否为空
来源：http://blog.hesvh.cn/Article/details/gupujscvh.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/ghxwyzakj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.zdbjq.cn/Article/details/gcgarvgyn.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.hesvh.cn/Article/details/gwejtcuhs.sHtML

TS:   if (s === "") {}
来源：http://mobile.fehbvm.com/Article/details/gsvgnqsij.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gtlvmytnf.sHtML

Go:   if s == "" {}
来源：http://3g.hesvh.cn/Article/details/govpdzgyz.sHtML

Ruby: if s.empty?
来源：http://mobile.fehbvm.com/Article/details/galgtzzlq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gdizlmkkj.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gxjdeohis.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.hesvh.cn/Article/details/gepyltjrl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://mobile.hesvh.cn/Article/details/gmvarokyt.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gbynfbviv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gsbhqwjjm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gcvnhslci.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gnozphmcm.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gtfrbeqcc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.hesvh.cn/Article/details/gwapbepla.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gtrvsyhxw.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://read.share.zdbjq.cn/Article/details/gvfdrvspr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/ggnwgzjib.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gdcwbsmqg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.zdbjq.cn/Article/details/giiuyotqt.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gohljvzrl.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/ghusnxnsl.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gpmjunpsx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gwxgmgozx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gioxbkyif.sHtML

F. 文件与目录
来源：http://m.share.fehbvm.com/Article/details/gggqemace.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpkrjwvoh.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gzmdkqotg.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/gvjiyxctr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gqpmoulyh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gvztuciwv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/guyxpujpe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gcqlcyylx.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/gxhjasfzr.sHtML

Ruby: File.read("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gatxdrkqf.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtfttyomn.sHtML

[F02] 逐行读取文件
来源：http://www.blog.hesvh.cn/Article/details/gjstxyjld.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/grkenjxod.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.zdbjq.cn/Article/details/gojrjdanq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gwkrapjnv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/gioyqytid.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gjdkhektd.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gievgmhun.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/ghvufpxjm.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gzpgobotw.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gwstycbad.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gjbqavkcz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gtghhroye.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gjrwghexl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gxwjpwlwp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.hesvh.cn/Article/details/gwcihcwja.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/genovzsad.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gxsvijxaw.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gkjvdqzki.sHtML

[F04] 追加写入文件
来源：http://www.m.share.hesvh.cn/Article/details/ggrvrtewx.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gsruuybqc.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gxdmkxxmk.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gbgmewrbp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gyjpwezeh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gtzjkmpfc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/gbzkszznn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/ghozchuyu.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.hesvh.cn/Article/details/geulohofh.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.zdbjq.cn/Article/details/gikltsfpf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gcesukqha.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gdokewokj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gschhspiv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggvzgckqv.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.hesvh.cn/Article/details/guduamenc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/gsinsvroy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gochxewei.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gfhdmdaki.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gckriguji.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gtvzyopia.sHtML

PHP:  unlink("a.txt");
来源：http://wap.hesvh.cn/Article/details/ghbtoozbb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/guxebarxa.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmfomyeyz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gjinjwsqf.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gghffetpt.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gshmuxatj.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gompqoeta.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fehbvm.com/Article/details/gtnavmqda.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.hesvh.cn/Article/details/gyelnvoou.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gwbmurias.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gukdzitmy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gnlpfewrp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.zdbjq.cn/Article/details/gcrgvnans.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.hesvh.cn/Article/details/gsbmfogtj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/ghbtvwqml.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/glkrmpude.sHtML

[F08] 遍历目录
来源：http://read.share.fehbvm.com/Article/details/glbxkgdye.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/glwlfsyzr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gsyqsbcvq.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/grbrmvlqe.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gzlgrifkm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/gkbzvdbkd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gqwlxqcjg.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gclcvnbvt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gycyagktt.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gfvubilkc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ghfujdvao.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gnzdtvxtg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gxnxeazjt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/gvmhzkmrj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/ggjlpcocn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.hesvh.cn/Article/details/grvmwvmqp.sHtML

Ruby: File.size("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzoyyhblo.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.zdbjq.cn/Article/details/glqewribs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.fehbvm.com/Article/details/gyqvtpqor.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmhdagfqi.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gnjufqswn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gyncnrwbc.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gthakpgjz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/gwjtyhdfj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gpggftozy.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqoruaojl.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gfdidbfjc.sHtML

[F11] 复制与移动文件
来源：http://read.share.hesvh.cn/Article/details/gedrlcqvg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gkzqsefod.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.zdbjq.cn/Article/details/gilwjklbc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gruiuhqmu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gteomrfit.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/gwxixabuu.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gvpmcrwrk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gbwzlbddx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fehbvm.com/Article/details/gyknjrmyd.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gloksfyuo.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gyncupbzv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gxkwimevx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/grkjtibkl.sHtML

TS:   // 同上
来源：http://www.blog.hesvh.cn/Article/details/gexjufyta.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.hesvh.cn/Article/details/gkzxnrbpg.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gvesodyob.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gyaeambfh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.zdbjq.cn/Article/details/geivcuxhr.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gtfbeamkh.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gifjtnbnn.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvjibfmtj.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gyhtbuytc.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/gijqoqndr.sHtML

PHP:  class User {}
来源：http://3g.fehbvm.com/Article/details/gqqgiitgp.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/ghalyemap.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/guaksqrti.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gjglivogf.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gkcpxvppb.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/gpaibtnvf.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gmpxmnvxf.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/ggshkmzts.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.zdbjq.cn/Article/details/gvflkmrla.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gupuqttnv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gbcdqblzu.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gailamtgx.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gkrkofmrg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.zdbjq.cn/Article/details/gppohqmin.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gfpkekbof.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/ggtiqscfn.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/grscgdrgj.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gqcchpygg.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/ghacpgwmm.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/guvtojsej.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gvcspulol.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gryjxwckr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.zdbjq.cn/Article/details/gujhsafbw.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gjhzexxbx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.fehbvm.com/Article/details/gdqsppcsh.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gwjyfwjlz.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.hesvh.cn/Article/details/gdqrzsfsp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/geetrucqk.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gkluuljws.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/griajrpjl.sHtML

Java: String greet() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gswlwsick.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gdbrcmmmn.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gswxctqir.sHtML

C#:   public string Greet() => Name;
来源：http://baike.zdbjq.cn/Article/details/ghvzjfvpk.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gwyssumll.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/glrmleeas.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gzhcywxyq.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gsrstyjna.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gwvndrlqb.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gmqvqzjvj.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.zdbjq.cn/Article/details/gkthoqlsx.sHtML

Ruby: class Admin < User; end
来源：http://3g.zdbjq.cn/Article/details/gcttarxbr.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gbdmmekwr.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/glbjefhda.sHtML

Py:   def greet(self): return "admin"
来源：http://m.share.zdbjq.cn/Article/details/gmqkkzlqh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gwxtkufke.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/giiehueqf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gbgufclwq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gomoajufq.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gpnlxfmrn.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gyufqgksj.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.hesvh.cn/Article/details/gnsnlyecp.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gpzxmcjlg.sHtML

Py:   super().greet()
来源：http://blog.fehbvm.com/Article/details/ggnfyiltc.sHtML

PHP:  parent::greet();
来源：http://www.m.share.hesvh.cn/Article/details/gafqtwnjg.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gjhqhqbhj.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gqasjqqmo.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/geaprnctt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gilorpwaj.sHtML

Ruby: super
来源：http://blog.fehbvm.com/Article/details/gqggkheap.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/getsmitjq.sHtML

[G08] 静态方法与属性
来源：http://read.share.hesvh.cn/Article/details/gmgtzdefd.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.zdbjq.cn/Article/details/gutvrmoyl.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gcvlxghvj.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gpkrsdyar.sHtML

TS:   static f(): void {}
来源：http://www.share.fehbvm.com/Article/details/gdrxuudgb.sHtML

Java: static void f() {}
来源：http://www.m.share.fehbvm.com/Article/details/geztfhovf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.zdbjq.cn/Article/details/gmkyedckb.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gjwpbolol.sHtML

C#:   public static void F() {}
来源：http://read.share.hesvh.cn/Article/details/gxtulfzbe.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gfxyzftqd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gszgdwist.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/glbdssryk.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gzgkdibcu.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.hesvh.cn/Article/details/gguocluuy.sHtML


<!-- 参考信息 -->