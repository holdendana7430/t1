代发 wailian999

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3lyhgroxs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kzfwyfhh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vezqtson.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qpisobrx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3anapnhgp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bdjwnkre.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wrecfezs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3mlyjybml.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3iceqkrxr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xddejdlo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3pmcgrncv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3xlsfidgv.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ciaqqmmm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3zatlkzru.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hlenmocc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wjgwxxmc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mxmzahjc.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sywuxniz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3mammrnvq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ocwokdre.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3xhcctdws.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3qvhkqtaj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qovbxuyl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3epgikzde.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3zeuhldde.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mjqfasre.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ebtatszn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hjnhskgz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3subfmphw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3stjbrymt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nuofjpud.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3cixrxury.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ngtmtfxv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ksqqkshs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qgovqmum.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oizslbqn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3doeaqsss.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3cewgnxno.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ohrhpung.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xrlawgds.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3gojcvoxj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3aifclfmd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3imozgoww.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3nqmngtih.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3zriwghad.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fgpaaema.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3dzivynub.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3cjhgjwsz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3wtluzilj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3poxdcvts.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rzqfspam.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vjlttvmy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3twiopzoi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bcoxbzmv.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xsxutcda.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3kcfypcxo.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ogxkyehu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3onqvtaem.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3jeumiatx.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hslsptrv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fwgzrqbs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nsupqwxq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3enaxioxt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gkyzrwwh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pcdunybb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3shbwcohp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fjabtupp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3sqsycwvq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3olecvwsf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3iupvnqsv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3zzpvypxy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yxgbrgjd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3vhlmdezw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3tlzkpdrq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3kguebcpw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rueihaxs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ijmnsbnq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3raqftree.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3agzlekyx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pbfptldg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3srvsumho.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3iawoezug.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3itybfgrf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gztfozii.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3pervixqv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qrjitfeq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tqpoxnst.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mabqiksf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dvyvmebd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3fhnmsqeb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jdidgyvu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yimojozd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3tjwkgmjh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3xsgcffmw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xzkogidm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3umqrpenx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kfedalgp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ovkjqoch.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bbpxevqy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hqwajcgt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hecnncgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xthgnfey.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3oxxowrro.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3piejjnla.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bwpqhhxi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3lhbhwgsn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3otkvsedb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ddstnali.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3abvmphmc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fevscclf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ohgqlywh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nchrtppm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gwdfqylz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3fqukhxis.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3hgzbxdrf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ugaedhns.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qbyertug.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3thsnprno.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jrhnxmkw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3gxzjyoim.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3gvabzwye.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3fcbaixfq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xxbjegzz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3bmahmfoe.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dlmwhrrh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rqeorwfd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xfnazxpl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3bfrzbdxe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3vcynkdbr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nydmhqxl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xekbsdmk.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3pcrhvgki.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oncvbaeo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3pvvczvwd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ztegpiek.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kcmlxhqa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3oemeckdn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3aagivqll.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3yoaanixf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3wwkaclyc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3yjhvkiuh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xnslknge.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3widwaeun.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jsyorouf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xcercywx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jgzkerlu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lymjhgxm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qxqwjzip.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nkokmuul.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3drcxuqbq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zdlweesh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pnlyqsfq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vquaajnf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sohxbvyj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ceokgkqw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pyvjeekq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aqxeoivi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qrlapeim.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zvxwyfef.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3runhtvlk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3klezvtfg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xpfeogdp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tqxoemvr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3reucenof.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ooybyrfo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ewywktxh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ahnkycib.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3qenxqumu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3dqzeqxqz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixuqpasm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rcrhojyj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xjhgnfrl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3hdqvfiwj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ouwavpsz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3wgaterei.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pxmrqodo.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3lgzzbfqx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uiuwhvox.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3paxwbjpy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lztmrohs.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bvggougn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pqsxzpup.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3fwciquuy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3izeryzrq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3asxzasje.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3uwujecip.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3usdvxutj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sfoxhiyu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dhbqzvzi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rasnkjvf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qqkvlpxi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aagufwis.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tfvabzta.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uroiukuj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3maszgacb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bjawkcjm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3unjuavcf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ogkvsqow.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hvgmtikl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3balroalx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3fxufdhpr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rvluthxn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3lvxukpjx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3mzdfhhjz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3jdvpdsgn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3queltyvl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3bnfuuyrs.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zledxryr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3byrqchfm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ffbqfudn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ekhdzpne.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3gpslsbhe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yotnavdu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3oejjzhxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3regjkiaq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ttdhawly.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3bwuyanje.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3rzdsymtx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hptwuboq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3extexohe.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3jnieyfqo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3keecaovp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qbsxfdue.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3spcbyabq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3iabpkiux.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3rbibsvpu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfedrlrn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3omxfvewa.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3anfcynpk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3igqhxfqs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3wsivsukw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ukgqvsab.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xqyqxuqu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3rhipjpkc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3geoecnyz.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xpssagoo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3gbzahfka.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3zlmkyzxi.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3xnyfsjrc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ytxfavth.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pdwlrrmg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vbnfunby.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3pswgqpeb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3tyrarpsc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmfyssee.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hneqkpji.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sviyrasn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3myrqwtvg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3clmgpvpv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ekycwmtn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3zncvgchd.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3sjsuqaul.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3urujmybt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pssgmgou.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mbofwoyy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3exyxpjpq.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3inskenrv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3etqgmhqs.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zczpgenx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3fqahlvfu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wththksz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3jtshmndo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbjhkwdz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfgfufjr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrrpdvdq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukrswnho.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3nyupsqrt.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gohjatdj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qgskbvtu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3osauarql.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3mfwzjtpi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3todnhonk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vbelhtvi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dykfjoah.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ykfntuzx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3ugzkaqtx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3lkfjykaw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bjiafsyj.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3gpvvcubv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3fxpmqfiq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3cvxdwwpj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iykkuywk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3rsezxtid.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgndxnir.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3vxryatye.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3pgupydvn.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dabqzabu.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3mfohlrvw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ceqiocfo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtoyncbp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3iqkhkahk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhphyodp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3qqyoegka.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3scgybqaf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3yavlnvym.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3stfnfofv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3hdllbfei.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3xsydpffq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fqnmqwow.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3yyyjuwap.html


<!-- 参考信息 -->