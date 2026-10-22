代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2esqhxmbr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2sgqdvynd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2lhyghabc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rapqfvmm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ccrgevwf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2tjgjmkae.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ywnxvzdp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2txkuzoss.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2hbnbnvgb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gxdrunuk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2kpbaemhm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2rlivblie.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ezibwndc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zokczwkn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2ehbsaxqm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2djnhpgsi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yiguigfu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fqdlxssk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2iihtwxsh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2bxwlrjew.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2babanzoo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nxsuekzb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2knkczunz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kvumhhmc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2gfzigdst.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2btrlrujk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2edhvqgoz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2kjrtloeg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2eoralmpc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gnubamgm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2qjzqxyal.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2uwpwkall.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dnkhymrq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2qprlbyzw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2odqcodso.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2btxztofc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2rnyxijis.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2vlryrakb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2kzcypcoh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gkqmobzw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2abyzgjbb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2scwfwkoq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2drljpmip.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fgcznedu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pifmvvlw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cobvbdaw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dzmbfjot.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ulkifqnc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jciltzjn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2eecfvofz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2pehiqsyl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ybvupgwh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xluiyzmw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2otgelmxj.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2gtyjkfua.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wqhdscnv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2kfmgrjao.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dhogwqgq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2lxybjpci.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2dpgsftcs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2fudjevuv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vinvkenp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2myhfoibw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bcvmyiqh.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2pwifscrd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2uepymunx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2njmaxwaa.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bvejywmx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2iqogqgua.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xnxtmlto.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2isshkren.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xiayxqxt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2iejupsln.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2glwedaqx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2crzedkxr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qxhsjrhd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2rfbsglsz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kifvynmh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jehhjuuu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2reftkhqu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2edvihvpg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2nivqyztx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cezxumeb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qcrjtspo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ayimhbvi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzkyqffz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2yvnfeonj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwjjjdzm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zffpzjsn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2rpbkmpxp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2oqtflpsq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2chsewhhq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xtdbgykc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2grpmphio.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2dsqlhusn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aogjigbr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gqgpjebw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wfwjwqdy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dqnmfrsl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2krzrcuju.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xehkxngl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzpkgjai.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zqcevwck.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2obivpngq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2znvhcccv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2yodotigu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2auxjbubx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2bhgyztmd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2blhczzpi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rvsddzwb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fzrdifba.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hqqhodka.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2bbhpbmbz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wcrahrpj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ozyyqnjq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2lkrzjewq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zzzunbuw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2aknhcsya.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2msmzfmgu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hxowexlk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tlinaksk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2eklitxqh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2idqgfthk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xniqecyu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2krxtrdwh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ykgkdweu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2judftqmt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fkehejyy.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2epxpcbhz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2buesxskj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2xiftazqd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ggyvlpns.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ljqtlmfs.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2geukmotx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmyooxrx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2teuzgdbn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2voedthzp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2btjplisn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2apjnopuj.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chgoxcpl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2borrpgqf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eqfgrfjv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mfiwgeia.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yfzxtuqs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ljlfmzlx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bewwnusq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tghwqatz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2wzrqfppf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2rcoirlkc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2yqfaddkg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ktctapea.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2sqxhjyzq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2snpkdvoy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2ettgtlfv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2elxmcubh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2isjjuiqk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2djsivxup.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iqoulzwm.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ucbunvnz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ndxhbhpd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2zpeqqgxy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rckejzlg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gulzygef.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xskialio.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qcwxalxh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2viapqfca.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2lznhwulx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pbmcfutm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hgwrrxiw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qjyiiwud.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdcvjvpa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mxadbmbq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azptlycw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ovnfaszq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2utmnlwlr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cltnyqle.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jyqdeewa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pdgkofaz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ujllsgdd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gtdkcork.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ssbocnte.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rmemxfep.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zyllvkby.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yrfuvfyy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2wqciukas.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmyfmyjd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2jftyvrtq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2xdnhlmzc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2tvmmabvo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2jicpalzc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qdbhhkmm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2bfrtsapt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2qncpkqvg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2czaxtrcv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2haxesefm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2sbrzwrii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwvfbutt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2gwgqymdq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulrwhzat.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2llrwejvq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2mgyjejyk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eryolxog.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2azhmeqaj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2rfbivppy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qinsfxyw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2noklalms.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2gkuvibek.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gjqnahfu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2fohuoitp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2fcsfclqq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2apjmxdww.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rqmxesbi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2meocmtoh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2psbcrojn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2vsqndglm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nzgjqyjy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fcvuquht.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2smhwwyqp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2wblozhjv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2egynorsz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cmmkusrz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zzdrkujw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2cisiixoh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2oitbpxlv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ioxkosce.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ujlghbif.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ovfyjxhl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2bidrfgds.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dantplbn.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjxpwrgy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zikqihcn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncitiatj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2szuxfgzj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rxkfuvyr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2dpnrkohy.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2yxrsoaxs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2wcdtivxg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wkmwccnz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ehfxcelz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oabbynjd.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2awqpwnrr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2ucfkjrag.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qewgegze.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2scctwtlz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2vmsmjwgh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zcxgkwrl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xjhjfgjg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvyyibqs.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyscvlum.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vhjjpfyu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2jufwtwzf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2gachgugu.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2aagkponj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mhshmccb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2tnodqszq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2rqbczizs.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ywapkuol.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2boiaicqz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bpqnjsbe.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2bpbvaost.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2zuwtjjqn.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2niwsgwnz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zuvfvuof.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ftnmflqz.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2jknjyuqu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqfuviyd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2wijpbwoj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2sgdefdty.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2goptflwr.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2dvnfbixu.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fecgvfpq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2vxnuygzw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2nyejuzvo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2gerrfefe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2rwyaapku.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gelismdy.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rijiumdm.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2vzolhixh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2nyvxnjdl.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2fpgcyomx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2jywkocds.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2rvbgglvp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rbuvnlsv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2zztscuxc.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mmrrwjlc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2xqardlwq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2pazkjvxn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rcwkcuqq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2dabbualo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2owlbqqxt.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2uwfeaksh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2svstoywg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxqlnhnj.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sfdjgwno.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ahafzeqv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wjojqpbr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2vwvjwani.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vrmbyjxe.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ysruxpjz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2igddqfiz.html


<!-- 参考信息 -->