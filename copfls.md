代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ijnfybrz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xvjgfpxi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2psgosesz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2yzqohrec.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ujiueaxf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2esmlsblm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2bjodqqzv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2aspdaxks.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hiuoeutx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2zqaiuqwe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2pbfdvuhg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2eclsvnzf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mhjdxijs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2otdhnpiz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2iuljjbpr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2umrblchm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ysvzmsnc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qjjwdbep.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yqucbvop.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vzmjguyn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xxqsnjky.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2tfcgspya.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ghsfccit.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2uxhrghdz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wacsvldt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2chgazgsd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2byobcmhs.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2jpusluxu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dfzgxrrr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2nphtinfj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yrbeccpa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2idwneimz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rwwtouxr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ahumxenk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2kxquuttk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vstkegml.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2dpoibhjv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2hpwrglzu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kbrexcme.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vquekflg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2skulyqda.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2oxzetozx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ygequmsx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ptmzqtic.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mevvsgyg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2kjoprvob.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hfqordkc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kobfgwnj.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hbhajnhh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qmdhdbrm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zamkifyj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lmqnetrs.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2jrxzoefa.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2aqduyeqn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2evwxrbmj.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2wwqbcjqm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2hnnfbfta.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ulzprers.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2fvqcldwh.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlrednna.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmfttkok.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2pauodzhi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2cmugorzd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2osovoviy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gamkwwmk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xouciriv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2albmloya.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wvzzibsp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2keadmtlu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2vcnqpldu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2padynydq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2plyslmqe.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2lasbldro.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ofuuqycd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2slskfcqu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ngfyfhro.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xyazomes.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2krrzdixf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2keasavbz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mjkaekrq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2boqgygha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tjqibqow.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2wauaoxac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmnpgwbq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2lkesqhqr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2kwdxmxbc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dbpvsevp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2wtfgkenh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bckajask.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lmqzoocs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2zejndclu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2szjuoffh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xhtkzwwy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2uqwkocsb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2fxbxssgv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2geiaralv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2inmipacz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cbhyoner.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wfvskvis.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2vzkopvwd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2bcvhlodb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2mpmowttb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2rdthxtdw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pplyowxq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2djesejhx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2adjoycei.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2oqmnyugz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2kstzmasc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2adsowzev.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cdsfrftz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2anqqyvks.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2eviotgty.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2odicebxl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2rpqmiekl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2sjwedfsx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kkipkuad.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2xzuseabh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cmkuvcmp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2tifoaomo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hdurphfl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2scglsrzi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ugsengeu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qybioslh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajdkjuvs.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kltnuayd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pevinxwp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2oadcrdge.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fnhfinxq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tqjktysc.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2koqcmmsx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aveejxjx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ibppuczl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qkkumtjs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bifqcqqy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2teeczopl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwscqrdz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwbxmoat.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xpipjfpf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2pqgofkdx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2qyvtwppm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2szzdduut.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2uyqdnpgg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ltnozgaz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2iiyjsboc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2zabcgiyl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2fyjqduwg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2exfysncu.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2cmaypouy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2olrqadov.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2aihqzeoi.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cewxszok.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hrkkufko.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2umkmqlju.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nnzecdvb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2vgilnvik.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dvkszffh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2cnsnotyw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iwfgvjyl.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wujuhwjz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bjrpouor.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2avyrztqb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cykxihvy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2xlzxbiaq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwldjcbf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ldshvrxq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qriskiwu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2istoblrn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bcntcozn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ygjgpypm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oovbdhcs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ptbjswtd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pmrfpzfk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fiwpusdg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gighlend.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2jnfiincq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nnkpwrfz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zoihyrls.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2balujozf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2mwrqmlir.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gzriqish.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2syxscgjg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipcsyrvq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2zkpvkajg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2dwsaznqh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2tbhyqjyq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2lheuzunf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2tlcuygbf.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2uasobfjb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2viopexzg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2pdrejotb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ofuuwsdj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2etadrtsa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxsontnu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2hfizmina.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iilyfqly.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2kspnlhoi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2yqjifkyu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dsphfhhq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ytxyxkry.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2viwfjrie.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2eftwenee.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2lwupnvtb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cvlkiggk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmwjhcge.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2djvkezju.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2zjeidsib.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ukwpdted.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ldzdfjvr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2abkmfudb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2halypfpk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2segbpvbn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2jkrtmaeg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubasdwzi.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2rpxjwcva.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2pqdyimzs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wlvxrsvy.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ubzobjlc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2gaptawpc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2ghohhhpb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rqmnnavz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fxnsvmbi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ocjfsoqq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2mihfjiol.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wmigdbkw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zihwhtlj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkiacawf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rzcyrsft.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2efpasism.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bwsxpoft.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pjktniys.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2rklmiyrt.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2baqrshnm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2iqwhgiks.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnihnsom.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvmxnikx.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xqxwfjjb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uprtzrzj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2enefzwrl.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hgiptdww.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2snamtvwt.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2wizzkfxe.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ipqnflct.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dergpivf.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkbecmrt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2izkymqiq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xgfceiku.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2czfujsln.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vklvsqoz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wihusrpi.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2cafhusip.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2ijkrgorf.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2fflhfvat.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sebnsjem.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rijprvnd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ortwngwd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2nuiuzwmo.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2gzzvnbdq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2caqgnnqp.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2gjhpzxza.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jndljwmc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yiqcmxhk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2xemfyzss.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2yzmqpdcw.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wuoirmsl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2xnjyvele.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jjkwactg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2rzbsbrmy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2juggcppi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2kdakmtez.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2auotsdst.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2oqxkmffz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2sutnvnqb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xjnahldg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ztwaoidn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2lulqvlgs.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2uheupims.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2grnbvesn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2aiwnxrvt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zhrfkzrw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2bzfdgbxy.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2etpytbxd.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2bwcygyaj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2euwbsvpo.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bufmkiiy.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ohebkgdg.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2rqmomaih.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zwxafovu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjaurxor.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2zjglwlye.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ryduvxrr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2marmcdjp.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2cxgawhdn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2huviyhtt.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2krdnaape.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2wlhkaaxh.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2phubngnt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ldvamdgb.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bmepitvp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2doapodse.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkhlbdmm.html


<!-- 参考信息 -->