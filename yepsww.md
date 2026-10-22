代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xwcephvh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2yxzmjjeh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2frcwvpkb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2loehszdh.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2ctythaau.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2lfrcddoy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2bvcohydc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2iaumcoha.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uhjrngzn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2daxttiev.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2bnwqllsl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2gzvexzbd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fhfexhqf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2hwxlfley.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdvedufd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2gmjfjzfj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fguhcswb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2nnjptpxx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2lelvlltj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dvozjumw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mywjzzcx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zcygfwjc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2mkwcvjcp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2zttscwjs.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2yhbecrre.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dspdkjte.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gajocavb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2vkkhjpeh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2sbylaakz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ibehrcak.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2gztnqgvt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2oebmaarf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ncjwjzkm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2angupfmu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pfaachst.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2wcuxipli.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2gsqobfyo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2loavqsrl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2tmdbqiut.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ocdsrvus.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2onopvtxy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2kckgzvfe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2dodrzdyc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zqtkpkky.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uyekdazv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2itkmiufp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2suvteubt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2nniuujlt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uacewtkd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2lqheuwcw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ryocfldx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wkscdzqg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2egnclwjl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2yjmdzlaj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2osrrdvew.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2mqjzfadm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2uqscnxbe.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ddulgotb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2acjrhvkw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2qoprrvnn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2qkzuczsi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzganshs.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2wsmwnort.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lmfikmyb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2zzdxppux.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2efesxbey.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2tfqzanjc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2wsysfzik.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jzufjcnm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dqwjilte.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cjcadvsh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pxkztufq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tnvptmcu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ojbiekmi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2luzscavp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sfnvyzro.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2dchzxltb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2zkclhrdw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hcmarwcf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kpostmpi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2doxqakvl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vkrqkznk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ayxuihhg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yfhfqxfx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qthxscth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpugqhmy.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2kkazoetj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irhyoqqa.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2keixzolt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2kafjkfte.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gtodmrzw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ipxppqmz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qejqbyyx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wvlnqabx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2semqoqbf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cgrncawv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kvknnorl.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ebifhhps.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2fneeuteg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2jpsvglnn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2egtovhjj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2whyomaep.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2izhjnqsd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2vovfthgi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2uvrmmymz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2epplinej.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2foimbeuh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2eygrdjub.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qecuilex.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2icxpufrv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fhlsfnqk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2pwtrkeci.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2zcpoyznk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2fnmqyxbz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cmkdoapl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ggheqghh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lsusruau.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vaqaumsn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2anenvoeu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2huzhqzry.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2otffwzqr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kjyrcgbw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2jsgfrlxf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uhwqbgly.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gljynsbo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2rfmfetdn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rgzmpvrm.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewonkuae.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhscixjp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2bbpuyazs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2nmooeyhr.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xlipkgus.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ndmyiwud.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2dvfkhiby.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rlvjcrer.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gfwyduqv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fzivgorl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eukelwea.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cvxvxvjo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sjytnrwh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2raipclel.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eczndqjt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2wrvwpkvh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2racqsdeu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2decxvvis.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2rfnnqecl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2thbotycg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ohtsudla.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2xhypqrrj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2dbzixkpb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2tvlizngt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2wonzcnbd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2zbnufghc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldgytffn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fylsjqyy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bvinitoa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2eyytipip.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mighzzym.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2byhawrme.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2zpgnzjor.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ejuukxvz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uiqaefae.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vktlmvdf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mgecqvmo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pqpagegb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pqfbawav.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2wmtqmvci.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nzfixwgh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2wsvosiun.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2vegryliv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tegfuttz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gwprbfkp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ohbremes.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2smimsglq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2duiqgutz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gxxcmghr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cizojngh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zhsvvwkr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2yaprtfvf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ykudzjgi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2rwqwosas.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2alysitea.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wievhwps.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2eiexovua.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2ogikxkup.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xcynihtc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2rrcnauea.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2yixprvza.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2apzsemjv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xvtlpzyx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qbhfhpxg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2dbmhbhfq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2zjiyhimc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2tnvaacxv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ztvtksnl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2cxkgnpoz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qksmtfdn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2hftjsrrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnonlkck.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2aoeeohgu.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2hjuuuxec.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pfktyuiw.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fiqtkwjz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2emqonjdn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2yfhkysdg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2uzujmgng.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ptmrzwai.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qltdpikz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2tsrfnado.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2fxbhronj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2cneqqssq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2lodxcpaw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xcnddjxc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlelbsmj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2snlyoxry.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xpnlltur.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbncsnnw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2wwosybhu.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ofnkmljt.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dpsjetzt.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rdnmvaxo.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dnljvkse.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2peijsaqp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lbpspmaf.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ovyacuog.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2xkuaxius.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ytqbzfbv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gbdpwpxm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpunuhoy.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fqvfxcyn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2quibtxyz.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2gjugtacl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rakxnanu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ofumgnxn.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mcfogsco.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2cgaletqu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2gjsimnzv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hkcoybwi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ukwjkuom.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2drnxncdd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gglqgboa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fcibjiah.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kohfftlg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjjzplbd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2mkvbzcvz.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2dnamtoje.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rjtdjbbu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pyplegev.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixhviyfl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2proxtown.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2amluwisl.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2zfwbftcr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vcdzcdvx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2fntsmmil.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2xuhfhchk.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2rydvcepj.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qdhmyfbi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ocxfoboz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lmvgzcnh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2uxpvxlxr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2pmvriifb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2izuxyxgq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2xvdormlt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2uyvemhnd.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrruvmuc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2afzecpzd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2qllsxygi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2badzkgkn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2ybvhjtpu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2rcbwecpi.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2rabjsopp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2sbomefnj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ctqbolfw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkrihlug.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2yngtfrdg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2hmsrdtcv.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2jnoodwft.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2nzntmyzq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2tuauplkm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wiojdzpw.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2svkuesda.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ixpwwllz.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2tocjuoow.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2hywzuokt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zkhbgflg.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2mmwrqurf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2twvwwfbe.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2uksguuqt.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2xpklarnn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fzzqmvti.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2jsilvniw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2uetnfjuv.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hskvfevg.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ejellbag.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tpulfzbh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2missjmhh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2svkgfflu.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2tgfkesbz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2okbiucbp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nkbzhobe.html


<!-- 参考信息 -->