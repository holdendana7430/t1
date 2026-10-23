代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3masrbawh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rwglsoyh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3kjhymkbp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3llbnddeq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3xitlxphw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3genirzug.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3spdeyicy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3axssiwma.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ebfkicqz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3uzwiudzx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3agmfilfy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3uvgacawn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wmoicwdn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3uepmntxt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jemdpudh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qnvjsedb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3eadmynar.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vitnzrlm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3jglivdnp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxphpkvf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ydwrvlut.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3tvzbsgev.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3khiymbii.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3uygncart.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3gxmgfzsm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dlcgnzoh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bkcmgiwl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xzsangwf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3kqoalhxj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3idhbzgml.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3blbnsxig.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jqvqinsi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ximbvnui.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ywgvbnvh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qmyoxlmo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bslebibz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3etqkkaen.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3bjfcjzhk.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3sejyjkhe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3thcsonzm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nrirocrr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ihvqdxpu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3kpkagkba.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3yyjsvwgr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gwhffbjh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yirpnntw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3njlxibxa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fufzxgrl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3pbvezxxh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3cgucunwe.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3bimmgqcv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3njxthiar.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jxteufzk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zbqrizmy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3kqzgwswb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gdztyubh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3txaaxslh.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3zzccfvdj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3spgcazfw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3fgmqeyeb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3upyadkdg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3alohpeoy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsxfxiks.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gtdrccrz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3cqetuftb.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3dmllrzgt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kkshjeup.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jqiyugve.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ediehtov.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ygyxglhm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wetkzbpe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3higbvlqe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3blmakuuv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ilpcbmim.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zzbpwxch.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hrfufjgr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3gwzzpzhv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jjjgokkg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rgertqhu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pbkzmbtx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3oviuajbu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gfejbrsq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3desbyjyk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uasrjknl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3iqdiutku.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ryjqttep.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ahyeiyry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tvivydhw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lrqdbiau.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3bbtxtmpm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aypsmkay.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3ebctjxxk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3imcjwphi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nwcbqhtg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3alxqjpme.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3boibggar.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3frnyggvx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3juumnopm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3gbdwtafc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ybjtgpoc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hbnteoke.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3agwgolts.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qpzdvtlf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3dvjmodpz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3dpyqrnrf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3spoqmmls.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3tdenhjgp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lntlaimc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3myvelgty.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pdlbhten.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wpnaiyfw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nyocighs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3httexfgr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cwidyurh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3lbetplaa.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3eptgupfh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dwodrein.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3muclkskb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kqlkjuyq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pruqszof.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3zxuvmljv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3trmzvnov.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3axhdnjbj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3kppivyhn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ieagqyoa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3vvtbsuid.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hsvrekmh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgitafid.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wsxfyzhk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qbixgszi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wlshvwxi.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wbeyrsew.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kflilnqu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3kflngbet.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yjkuhyla.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3impzwgpg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rvfzfkyc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3arfwctkx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3oakdgozj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jufpwxxk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wraipbeg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3retkiaft.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mfbmhjid.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bzarcksp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vswmxgxx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ezzhswpc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3aiuhocsd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3dnvxokje.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3xcafwbbh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fknugnri.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3lzdvdbcb.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3nnmnzocw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3llhdesff.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnmyjmbt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cuxxdchu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dqsieeef.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rxpqusrv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3svxbohux.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ykamncbf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3tagwkgwx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ldwmwqxa.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnhnwfqu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uokyewzd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ckhndqjo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3kisoounx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bepjajup.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ukktmsfe.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hnrbqhhm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zmsmgoee.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3itefvggz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vseyaecs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ksuunbrz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ekbhdwcj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3defbpsfu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ztazmvvi.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mzddrmtm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ffrubzwi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3itkhdwuj.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wztpoifw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3odshtiut.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ucsuyids.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ieycetbm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3aazyvqaf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3mxxjfkun.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3zczxgrrl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ctahqijt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3mecfhqjx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3lfyuakpb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3glnfzbtp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3haqyknnt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3qmdjvjgw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3aouczsrs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3bqtjjjpm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3khbapzcq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3nicjculm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3pzkjwatt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ovmgzboj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3qtcrgxhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jmmhsksa.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hwjnzmme.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3uushqjuk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vnavsxay.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3amykmyhv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkdxddgf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3wvcnpqiq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3bliafnqt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3mmekggpp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mtvcpppo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gxxrfxje.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3mmfqglfh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3xkysnpld.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3plgcfoba.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3stzwmzsn.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxtvzqfw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ckyloydz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3sikohbxa.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fdiuxjfo.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3aixqdesj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3uhyrkems.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3znkoeics.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rgzpdsvl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hxquarzn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3maejimot.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vpnbshwo.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dvyzpcij.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vmjhmrdc.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3logciwgb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zbffptao.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3npyghyzh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dfawclrv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oevybbrg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gxmrfweb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ijywozgz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jctafbid.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qpdmybxb.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3buijnwzw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3uvtivrfm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rjegkpxb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rrsazbpf.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yplukcoj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vneqvgvf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3zncjzbla.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xfnhizva.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zvmyhffh.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jwpltwte.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3kpevqsgj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fmompxkl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlbfnzag.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmlfdgqt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mheaxgfw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3xarpnlue.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3glcmsvvk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3yymnayzg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3huebyebq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3yjjgynaz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3foxshqpf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uwvrexlj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qeamhbwu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3eluljiac.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3koeclemj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3vmbnxrrg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tpmyelau.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mavrusvi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3mjzgkzug.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3asxuucwr.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ksqtojdv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3olkaflqr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbolkmbh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3pqltjrkd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3oghyotai.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3pjgruqnb.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3wmymzswl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3rnsuqzhb.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3vdlnvdsp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hrqexhap.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3fijupgyb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3pmtcnysw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3sfugmacd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3vstmaesh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bwahrglo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3nlprlovc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3rzkvioww.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fqiccwkp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3jlxrpdec.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3nexptwnq.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3bkleuklw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3qonupcqj.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ynlkulhu.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mycstqam.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3khdohyzo.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3sjdmmnza.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtkvqfid.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zqpmyehz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3noxtxphk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfevqudq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ujczrmhh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3jmplgbwd.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3jwjlmwpc.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3oghxvnef.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zzbjzkjn.html


<!-- 参考信息 -->