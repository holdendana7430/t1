代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3llvwaxtq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tyiwhdar.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3obtlbbyh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3wyzjupbc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cevizbbq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wgzgumgp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3eyrhahgz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3tmdmmrfc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3xngjpaus.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3olzhbpfv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3sfjanasl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3klhsuprm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tzqjixoy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jqapxjkv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ndfffzsk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3skyyqjgz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3bqqabkrf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ulleulec.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fhsmlcmf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qkhwohfw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3azisbecn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jgqlwtcp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3zdxpjauk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3hxjfjafq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3zhgannvn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ssqsdoxy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3axszsbzd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ppkswbsi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nquwyxyw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vngpoieo.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3fgbzqqwv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xqzobqxb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3odpkyala.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3exghdjgm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3rodlxcxf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3balzueyx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tgarynff.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3imztcvek.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hzviksna.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ujrvwigz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3afvkfueo.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3wkwahkbj.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3jatmlsfz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3azpggnex.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qqwjzukt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xydalnqo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3dglueftp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sfdejmzl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3nkqinfdp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3scqezigp.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3kzvfsosq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3cgzgkiwh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3cafruvzu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3deypolxt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zncqgqdw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yagbtnjn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3rwzjudqx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3cjaumzzh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3odqhnbpi.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3rrnezsrr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3wyoocylz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bwdvjerh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vbyswpco.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3niwodxkb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3slvlkpkh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3zjskjrcz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gapyzere.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3iedytosa.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3zhflubjl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3rmfsisun.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nngrvkiv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vsbbysmd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jvhwcnnb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ezqpkrnh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3keiqmpro.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3woclzsbx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bywfsmnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yraamokn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3bketoney.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hafbhilx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xmfwkjnd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3djqnxvzi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ibnaynac.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wefrncio.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bopkgiem.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ztojdzje.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3svcvkaaa.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tnlobojj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gmvpjgzl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3abzdjslj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3wuckwkpu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3jfzlrcfp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uenahhxh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tlyrdmqi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3drnqxhex.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nqvabzpx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3fpircdhp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3llvnberx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qmtjubkp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fxkixrrt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fcsmsryv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ctwpfeyi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lgocjabb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hofagqns.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3zbqzlsel.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3boqxadbn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cznaxncl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3cmzjzcoo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yjuecuiw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zqraxbfv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ejywgvgf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3quqemxfg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ivflzszd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nxfidalg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3cqamhnze.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3wynrhznd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ygqerrpu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3rjpnfjfv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3skykrwmm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kegjuqjw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cwqbbgxj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lfvdemeg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3sztnfjzh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sworwywa.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bimacmma.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hhdicifm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jajfopqf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rojqvevs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zxygifhk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qlumbrrj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lqzztewv.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xhhlmdwq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xbcbpswf.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xenklkzk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rhqgnfwk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3txloxcir.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tmkyfnto.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vglzjuxu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zcxwggtw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3kbwbmgkv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3bxvsfwgc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3eaiwgybq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ellfxluv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3zxspsebx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3esdrrwek.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3cclbbiyv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pxzeapra.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3shidivop.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yxslywsi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xetklhug.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ykilwlnf.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3bxenqvbi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3lyveequj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kpaksyqq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ufximtph.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3uvaopxmy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ziwqackj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3npqrtofn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3efcfpawp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qokarnjd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3osffpkzo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3goymnvrf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ftwnacei.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qzafhrvh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wnxaqokr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3phtdywyk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3hocehnfa.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bnwffwoq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3drrgpugm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3czbmibfq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3dugkwvbq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ukdghpfh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3lrhnqrfb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ppvjyzpe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fefmfbid.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qapsdigw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ycfquikf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hvnmufzw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3hcjagxyr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3xeimjscx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ttcznebg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3isunpknp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3jqbnlvlt.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3xbkaborl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3nhazpunk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dokedngy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3mehplpzy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3crlaqezz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avyqnxzh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ovpfhxgh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3niylpyub.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lalckhjq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ntzjnxpn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hrupqoqf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oafvjarm.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gpedmqvw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ihdgnbjo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3anjyolxg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3yaxqiahp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3piftlbxw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wtvcapcy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3oflopmqj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3krlkpqcr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cktpavgd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgoewszi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3osrhuazu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3azzxrnhs.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3giprkcgw.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjpmjush.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3gvaabmjp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dqtcmtor.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3npgdobei.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pejeuuyx.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ornhxwjv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3unrjwmiy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3uxucqnqk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mmgehoht.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3dwihjyjg.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3jnktogay.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ukrzlacj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dacxfmjx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvqtrplo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tpikeepi.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ytppranf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3lvahsnwh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tmbujkcc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ymbtnuux.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3cfllsqif.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3esssonwi.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yduahbgy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bltsdyen.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jwvhaskf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hiwjhyaa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ezzalqru.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vftlpxxb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ejurneyc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3clbnealq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3nafwvlvy.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3awyfcxih.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgwndany.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zbghsvwl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3caxhdaqp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vqbvbted.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3lyarmvfq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3mcbwaqzc.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ugdepbfi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3najhnsgg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rseidxki.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3itiildis.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jyiseive.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tunvkiec.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3anhommei.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ggtdiivl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ifhgywtt.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3apdpmefp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3eevlfkjr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hdunrdob.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lsbmpavy.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3advfmzdo.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ueifjbih.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mngjwhxp.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3zjgigsck.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmhhkgpy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3vougkftk.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3wlgwvwpc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3rcxgsxfg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qirhjigk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgmhpdky.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbjgvuzl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3douahcro.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3iaaipyhw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfouycqr.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vdtjjmfs.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3dbhdewlq.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ufymyffs.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hgavenhu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gfduegjp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3wpfniwiq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3kmqlrhrf.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3etfqbgag.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3gswulctl.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3kkaukyet.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3allyncyh.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3rxszpdwc.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3gzpvqprq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3myxvcjsw.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kigkpfdr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3klrirckq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3udnjwics.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mapbrryy.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vwpnsnfp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dqktpfxr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jjvubwyh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3inhryonh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bckheeug.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xdiokxgj.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ajhqliap.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wkdakkms.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kjmgbbsc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3violbumu.html


<!-- 参考信息 -->