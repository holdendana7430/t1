代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3nbbhyphq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3viylbwpj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3yhivkyeq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ucpkwhho.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jrnitwnx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hkowdung.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zlvajrab.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xxrybjln.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3dxlnojsl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3stglfsec.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ngkdsdza.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ovjdxhyv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3joddeehf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bvwxuook.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jfaeujhs.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ncqescwp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3dwvvpthj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3soosqzel.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dxeujohd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ptpfxzlp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3zbhlsuif.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ukpzylih.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3izwymmkd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3btyvqxmj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jnbvdoah.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ubwdbpgf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3keudialv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hkqwlyig.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mcjxxfpx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gadwbwiz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qdqnclqo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3lmwnbgex.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3zdcbgggi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3xlzhjqwg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3axotkxhv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kwyhcuwf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xyeuaeav.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3desliwmm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ufjcbziy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3smsnexlk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3wmdntwzy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vvnjgctp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3dalhogaz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eoooasfy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dnudlhbn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3furpiolb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3fvscvfii.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3zffxvzda.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3xmvtuhgo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3mdssgxlz.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3qfpatrsl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3iokrmrmp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xjhpvjru.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkdjjymu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3lpcwuqnx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3iqtcpzwf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3wvdzmmnz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3wzslnvjm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aadcffbg.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3yrqzbpzj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3difufnvu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xyedhaoe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pvnfafis.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pztfqann.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qhxrkunm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3hqcqqwcg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kpivzprf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tcexphgs.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3qxflsdap.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ldxqrlzq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3eltwtbtk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3edzazsnd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3niwpcygu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nsvxkwkl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3avllfqsj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3otikrrfv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wgldvvtp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3taulpvpm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3bexqrice.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pleibokw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ftkfrgwm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3fvfxflqm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qybcdosf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3msymmlhy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3btuonaxj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3itxpbctv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3xsqemsqc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oqqkiget.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ljcyjbjh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3txrtekej.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3faumkjvm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3tobzfjce.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kfqwpcgh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hbsbojua.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yegllzli.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3tomqftmu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3nvbjbpqh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3qoqlhqbg.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ekmmfcej.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3bafdehyg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gkbiodpd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ksgndyuh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mzsrqouq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3sujvkebr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3pffdrfod.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3urngibrd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3uddrdsht.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gypfdxjc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3monxutlc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3brhvraam.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rcryqzlx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qwynrkwl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3spzshjue.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ugvtbkag.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3gvccsxwd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ayiqyypq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3hwtxzoko.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3aiqbuxmf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yexxysqm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bijgrulp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3drlpqsaz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mmbojwrv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3cqdyqtzj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aeygfdme.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sbwxgdat.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3dcxeipob.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uaexkfjm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wktlzawk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fdwucfvw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwtdaqcq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gqhdfabl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tcjxtebv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nhuomxbr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ckbkksbe.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3susaxrhg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nyfceiro.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3yprqqlbn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qdomctfq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3elsudhpf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3vwowuyrm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3fghuvtyy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ohwtakdj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3dhmpctnj.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3moihbkop.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3rngmgnwr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3pecjwuhx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cqkudiui.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zwhfhcay.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3pmctkhia.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3fayttdgd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ynrrqatg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3htpusoqx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3xkobyyzw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3niaywaxm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3exvssclg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3glxcyxwm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ogysfabe.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wykudsfm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3nsbwtmmv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgjdqttn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3vljsczwp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3qbogitbg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jabtystt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vqaaqxrr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqfytobr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckiqywat.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3mztrjipf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pcouxavv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xlugprwd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3axhmhzoh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3rabptmlw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rwpmhwft.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sfwvddmh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sexdlola.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxzdinzq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kbfpxkiv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3xqxmjjru.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gxbvjntu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3stgggvcz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3euciwcfg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3hxroaqop.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3hhochmqn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3dlfkuqxk.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mzpatgyf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3jqjjulpw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3fbemmhxe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3llmjttju.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rnsjnjhy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qcfutqqx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3eavtkkdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whcxksvq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lzfgscsi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3eaankqhg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bypbdczh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ddoeovpx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3vnaanlep.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3alpwcety.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tdvojqwn.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cdxyqkpa.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3uxmzdsni.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qwldpojm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3fnotdzkv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3cgzuqprl.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uobydlhl.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ghatoiht.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dxuqbswq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ednrelor.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3vlqcenzv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ommekhty.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jcihumwv.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3csdwcznc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nvofttfj.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3eexsgayn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3hwgdgafb.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3alcesayg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3mutezndb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ljbzymqb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3weiajwik.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3mkfxiiot.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xyfvtnue.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3papmmece.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nlpjkqdg.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgozjwsj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tolnzbas.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bvwgcoux.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3duxgftic.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zrenwrhu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kqbkgnhw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bawdvelu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jallzyrw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rzyuswnw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3huxuaary.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pwlvpmfp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3mppuwmpc.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rxbkwxxm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uqqywzno.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3khbssabn.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3brhabyvs.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiuncxzo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydzbttxu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdjhvfiy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bznsvdtn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3xfzzhsbw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3zlbhzybv.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3nsvzlljv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3cckuacie.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ppmwviym.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pxrgyuwa.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wocoxbpq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pgpdzwxy.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3nkknmzzj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3vvnarlrf.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ogrjnzzg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3gkukyyax.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3xttnerxk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3kvkroydy.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3fiqtgwld.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3acmeblat.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3bphbvcry.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3trvzsscq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3gcuurwsl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3leccqzla.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojplacql.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3pffwpdiv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3bcvvkiyb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3lxkmqicg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3uboowhpo.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3znqlqhyp.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqkbonfx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3vaifdwfk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3akdwzpxn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3iyyjrikl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3fenphpxk.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3wpykjrdw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sqeosbcf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ewrtsbnn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kdqdntia.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3apgxsohw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3xxoqtywc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3naazqjvd.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3nbphisrb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3jxuzuufu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3scokkipv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ixdnpzut.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3uoassrex.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lytrakhc.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cbcohfzo.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3lvrynmlt.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3lvuubntt.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3thygvqoq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vtkmjnvk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mzejggld.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uswcdzsl.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtajmibg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tqwifxzu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hphkjqgo.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rplwmrax.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mqcqbgur.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jrvkuiin.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3dkldnfsa.html


<!-- 参考信息 -->