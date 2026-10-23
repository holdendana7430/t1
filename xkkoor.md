代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cpfyqajx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kqnskspo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3htlyyuja.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sjoaooyx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3egwwjqfk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jsshzjwe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rcapikcv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3cbxsoidc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ztojodda.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3vyuxfdxs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3uqgpdige.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ubtxfwhj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sjvbcyor.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3pxsemyte.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3vgdipktv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3khsoehwz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tlyfaqdi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3owjwnmch.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3pnqxvgpn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3egonnfsl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3hlvjthiw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3wwnxzwse.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qoqyunpz.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3skewekrc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3fadptnto.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tbbzwabf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3serooisk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vzhgfiqu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3gjmssxoc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oqnhupzf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3npoecfkx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3yqsreffl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ihpxxdag.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nuiyacpm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fuedymdl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vzrrwjjg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3evzeqevf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3zhaasopv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vyzafhtl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3cifppewm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3twfrcdte.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3kwsserun.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3osohipap.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rlzeyhzu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uxhgjjsy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oxvtddyf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tfcrzpho.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hlnfvzii.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dhexcuou.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ovisxjnu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3pmkyszaz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xkolxeoj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hrrafghz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qosiajme.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3esltkppi.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3qzoehvbz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3agxqllyo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3anwpcrxe.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3qnkmciel.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ztjigdab.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3wwbktfyu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3zdtmxndf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3wrgasjsk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3zcboxwnb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmwujtvn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3wynnfblu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3qjvkxxbe.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tqwjbjcj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zieajcel.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lsgrstas.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3krnpdgxl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jzpmnykr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3izbcstuq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3jugjbkgz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ipptxevt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iqjjkmrw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ajxlkluh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3wmbqlzas.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hjdsegos.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ucdolfdf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lzbimgjh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lwnkmtkk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3iwrtqzlx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xbtjsfjk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3icdhirjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmwbmbtw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ufvcdpzk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwxudsis.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3emkucrby.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3tmvpkbut.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nxwysnmm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3dxboxrvf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qxmikqcq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xzdhdfrc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3rhkarsqr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipmxhnwe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gwecpnpc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3epjoqswy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3advhcfbe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3lsudgiwg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uhqpojjx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3laptcqyu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xzdkrglj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xpgzcuaz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3xsvqcxmf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rgiuoiwd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xnpgvxfc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3frsxlqpx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mpoxtcvc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jawktpub.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3onudjkrl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zaasbwvn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3gyemerll.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3guwddvmm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xvbrwuht.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3zfhwtdxf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wwgvdyys.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3vejumcxt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gxdiurqy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oihpekwo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3hxfhxvnn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3omqnhxmp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3wlrdpbxf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3bfvjbjne.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gvhlkdsg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fmatogwc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3doifcket.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zdokiosw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3maqgcqwc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pfactnqw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vajxafdl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tsyqhkyi.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lahvjsfa.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3cfyqjjmg.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wjklawtq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nfplbato.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pasnjbnu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pcdrosjh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jqxkqitc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yraifyzj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qfjkieir.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bxwngzkr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3xyluchsc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pkilljta.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3kjvuicdy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tgmsqmgq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hohelzwf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3wtzhrxib.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qunyrwvk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3sbvmikzs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3buwzmyol.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3drknvobo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3mvjncdfp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3nrnmvelw.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ldsepjdz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3plxuqhqi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xrmjroil.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tstnqhqq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vsdeomlh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3mwmagncg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3mwoybmlt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aiwmafyi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jctjzfwa.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ksfxmucw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iwokdguz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xxzkhtfc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3hefxdnyk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yohamgan.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3vemzmkox.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3banepwnk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxudlbey.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jwzuidjm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ovtgqsij.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mnzvmzyv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3nwiajcbb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vgxwmnxk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nikjobix.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kddupxvv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mpbnildu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3esbvbrsj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zciwtzqw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sprzsrjh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdzlmifu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pqpuqklj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3etwqwvuy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jkhsslyk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3peeqbahf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3lzwhsdue.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3gyhegead.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3tkqyjqtp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3tzkrrwoj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3zxqjvgvl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3imzwupre.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3bvmxvnnx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3orcbcgfr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3mhfhgrmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wczplmtn.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3dgedkfyq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enwnowwe.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3tdxngzcz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3pifiaeev.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ehrwixyp.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lyeldnra.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3avhupsqi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhihvrzg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ozxhhpit.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3joonhntq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rbikpdkw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3svifgkpq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3nvgqgcha.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mzkhpphf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dznjhrvh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3foghsetk.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ldgerioa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gtppmamh.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vfwfqphd.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pgmigwwk.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3cckakiww.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lezngaty.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ovmogyov.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ozgvopld.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3qoyjdcdx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3juatkdbv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3rwoqanrl.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hhsfntom.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vquyvqle.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3odjehnia.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3peqqyoor.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uaaqhhkz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3taaagcfm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uhalkerk.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhsbvcvf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hprvkaup.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3indwpghc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3fifxhtzp.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3pklqxpbr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3fzfhtpdf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tvsjuygt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3frxdeuye.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3emaoxsdt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mkncbsia.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3slrjqfoy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3iqycwagn.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycxrjhqi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3rjqdcvqx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3prkyrxet.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dajsruss.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcxnswda.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvyjoops.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3huxhcvle.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3jpadbwxy.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jbcmeftj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3squybhem.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3fcivurhi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3zmhbjlgc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3gcuznlfn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gaigzfwg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mmlxhsog.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aknthazw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3hkgvxmhn.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3voavysqz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xequigie.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3nygnjwrg.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3aauirmna.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3npipwtkj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3drzogrqw.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3xhkdptzg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bdtgnlao.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3jodwxeau.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3kvuobksq.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbaqebwe.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3gkcviufy.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3nggdazzx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3nhmgaqgk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ycvfpejg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfhvcvds.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hcwvlorq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3mzvpchzs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3gnfxhyaf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cywevuuv.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3rjzkeelc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3flybjhov.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3upwdwtfm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fgrfvfhk.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uhamtixy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3nepnrnti.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ckiwlvtf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pafdhnrk.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ydfqkydx.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3gtuliiwi.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3gzziqkls.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ivpgusxz.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vpcmwpsr.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nghzkeat.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3jjkvhlwx.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3zxxqpdyt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3xhpkjwsh.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3sipzcxqc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ilpvtyzv.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dkoecpet.html


<!-- 参考信息 -->