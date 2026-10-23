代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3oqkprhil.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3djeowtvs.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xpevjoeb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ghsglydh.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fqzedocu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3admfvrls.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3deoqcntp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kydvkuys.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3stboidjp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3easiszhs.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xyrfputv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3wrbfuasg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3gqztuwkz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3oqhdbjcs.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ctbelxpq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3kvxdaxla.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3qslrkkqf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3otrjrdew.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xwlsquwg.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3plgdhmzq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3nygrdfqz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3zapdfvzd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3khnrkeeb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvippboh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzyyjlni.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3qhjmzvif.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ypbgflaf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ezfffhfv.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ofpxcraq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3jrfnwyfr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dwkrgqvg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ndzomafl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ydlamsay.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ccdgagkl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3tkgawynr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3yhqqatjv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jwnwdopz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3yqsishtd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3akdubfuj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gghnpfsl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3iijtryow.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ynilmilf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3tkrzcodt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wyppoyqs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ulrqfhej.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3swayvktd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vijtfbhy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3gffudsie.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3pzhjpllw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3veowgdwi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yyiiycrb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3umosqhfb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3bfnkjmhv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vivfakpj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3nylfeqnl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3hxytivma.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vbzzzaar.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3squygrck.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3datsffvv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tjlofabf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hklkmloi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nbocataq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ngbtsrmw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3gsmighfj.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3usnybunr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3elqzwjth.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3pvixveqo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ejetmnkt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zxlryhmp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gqezyvmm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kbbbohmr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bzynongk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3tvpmghct.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3bmsvxsbh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ssoixhim.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wektwiul.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kttqwnob.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ihtmqlcz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dlmaqezp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ljshtswo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3jctxqchp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3yrbcyzue.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3gicmbmjc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3eeprllqq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3gcnhqfpw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ipxqmluo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3isgazryx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rkzqjhtc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqxnbnjm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hcstpgsv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3codquutf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3wsywivya.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3peyxgykf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3djaeisar.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3figzfecs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3umakqkmi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zcuytqqk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3runciaei.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ceutihom.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rsoiujit.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3pdknarwy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3azgwilue.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wkdrepfv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3duzawphx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nfkxkkuh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jymjuhxu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bkbknqdf.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jqrgwigg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hiivfhys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kulyqyld.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3lcualvkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdytbeft.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3iaicnjxb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3yrlppbyd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3reznbzak.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3rnhdqozj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3penxqwjq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qcmeaqmn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3vulgegsp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jrujszia.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3snyhpulj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3pyhqcebn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3jsjgdqod.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3puiuxkev.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvjlnlnw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3udytocdp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ziupzitv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3efqdsqgv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3dsgjtgte.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3oyhraphw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3fcemhrum.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3rxanatzb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tgfgbkzt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ypefdbth.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bwvalpje.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3spcxfoek.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ezmjhgdy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pzzdvqrm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qjyxgkbd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3hxpuvwoz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3iolftohy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3hbfcxiqy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pkmkpacr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3huiikrux.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3hsqlgrfp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ramqkklk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zttivyol.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vzmvdleh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3texirmku.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3wkqlbwre.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vcvcxnbj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ctxwupsh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ctlvusxm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3smnpozgf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ohrpcsib.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zwpqhkop.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3loxmcrpy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xvwmrkwc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zgojxels.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bcgfhrxy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3suetqwyo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jpwsaikw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xtzeibts.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hnhrkqck.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dxhzzlyg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ybhqatqk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3tmpqzncm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tgehomyd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3lxyxafnt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wdtibodu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ghdmpfoc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ubazxsww.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3nswwmoxo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3polznhvj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3dzcfzapz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3srcrykyh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3xnffoocf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3nikshhnz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gakxwvkk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3sisjpnrc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yetiktdp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3crbahfpo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gbqgdsdb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3dezehjsn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3onqwgaqx.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bstwxbuw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jyqoojlu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3psaralxb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jgwyrrsl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bgpmbnpp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ntfnlfbm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mirpnlgs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qdhdqiiu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3tixkjnqd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yjaokjus.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3taeloorh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3puxjjabs.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nhiiukvq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3lywkxiek.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3txdzmmny.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dylaolqg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kbtlpnkt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3psuejimj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wsvzscjg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3fsyadxzv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gzgshvni.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bbgvwser.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3aeuvugeh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3xqshyucy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iprjywfp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3pucyizvd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3nrnhkayy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3bpwqbsbf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qivdvbkk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3vrzuakrp.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ztnevdtp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3dudsiywg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nzjyaswm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3friuypok.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3fxhahomp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kzqzhhou.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gvxjyvjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scyglxaj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3einamwjt.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ijyrkupa.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wsifiysm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dewmnkid.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypheskoz.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ybliwxzo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3sfxmtltt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3fthxipgp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jsxdtynm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ebpwouzk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3lpzngcnt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bupstptk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hairdvuf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3himjrqxg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3agpmfjoh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3yagpeksu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jbuiudcg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3klodlzwr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zfacytiv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dotksoyd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rbimjpes.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lsqyfavk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ywrbghzp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3oajcesyg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3fhiuqdhx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hplcbwfi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aqrxbham.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3uomgzhbu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3hqtcjzco.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lverigci.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppkatipr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgzqmkwc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ufugilun.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vihiyerk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3btoxacut.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3brxrvvlh.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3czdxfxle.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3zstnvsbd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jdslzlcz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xarijvdj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fogrvrgl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ugtopfzb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3mvzgehep.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rqkycvzy.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zobdxavj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3pkjuzfil.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3xndmepnq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kuqxhszy.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhpsiqji.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vztonxye.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dohcvdcj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3wwpnnxod.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3kfsfgggp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3xwlogtpl.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xasbpaog.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qtxcyaxk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3mgfgluug.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qipqocxf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gdrpiqny.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lhzcfhdt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3pogvargs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3jsudiceb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wpwipshy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3bbajfmhm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3tptcxuet.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpraklgk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ncbgptbr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3xvbplklr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3djwhedsa.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3ucxrmavs.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3maolbxwd.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3awrttctv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3uagulwro.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3esgfnopx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3tybrnhno.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3bawylzho.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3pnjgglpp.html


<!-- 参考信息 -->