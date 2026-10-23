代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3uwkjzryj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3sgnioads.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3xccrjfwx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3keebvwag.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rdeijsfl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bvugyurl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3rjzuvbqo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3wxfbolta.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cubokekx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3aojckjen.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zthjxqet.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jsrsspba.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rqslogcq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vsznpiay.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qrqawwmy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mfvlixjt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rodviwwn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3njmxaunl.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3aorzxqgd.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ekknfiqv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3obyxjdzn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kowrbedl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hjgkpjaz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3kvkbangh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3unkwbwbg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gkabeqkx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3kiljegyk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3tmorzlbf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3zhbqaqyh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3hepgdpba.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lmfnarsg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wlowjhlr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3efadixvx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3atgjboha.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dcyectvd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3orrwpmbm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wkzaltra.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3gvmpnnig.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3nrlgolro.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tyvaudjr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jepyiypr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ulxllwih.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3arjloyat.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3nxyqbkre.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nktztbrk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vfdbfpir.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3fncetjyc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bpriklht.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3caopxaqv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tzzwwrkg.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vvbdeoqq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tqwcdueq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3qpvrelrs.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3hrjcpybr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3gplkzdtr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3obpvygbs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3jjkongxh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qbkfoyta.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgitcjvb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuvygbpz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3tqdndpcu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zskinate.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jswrmhsl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3bzppjzqj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3godlkccz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dzuuqhea.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3svgepzen.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uhrpuilv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xrvohjsh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3vhsrsugg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bqllwvmh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vlrfwyxw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rxtrfxyo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zsubxuvs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dobrrrzb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xkwgulkf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3brumwidy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jkkbliep.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3vmkiilny.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3qxxjiyss.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vldblgkg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjhkkdkj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3decgwoai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fzuacmtw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ykscqdkt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3giaiikae.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gsjbgthg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3vmcesitj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3imrymvbh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xlypjhex.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ayqizckl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oddjhane.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yjbppnzj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3evcqbmcd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3lvyohmqy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3rshmmzbn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3kjovoops.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqtnvdty.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sxmmztrk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ugzfscmg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wifraito.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3zkyaonfr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3igatscgl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3atufaqhp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3gwwfxasj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ajnfpytk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3okghhkrc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sqvjazvm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3crfweiuv.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hhuutped.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bklztbtl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3yixsfxou.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3grwaszup.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ybmieogl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3agkvxlob.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rgdaundq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3vrjyijyr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3annmrsyt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vxqcqjnx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3elpkxdjv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pfpnppfa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3qynsitze.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fvxyizjv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dcwqpchf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hyeufbbs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ldzwxsdx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ooxzoemo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pwzquqqs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ieckuqtf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3epddbpam.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pjmihzmh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jktxzqnc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jtotatjd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ojmscgfo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3efxahrci.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3anrptqmu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nbpfzvjj.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3riutdrek.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3vyvowhrk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ukhrdphk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3zchibxhd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ocmifbmr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ujkblthj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3nikxajbl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3rjuumagq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3bqygucgw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3wgihthvh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3fdmdduib.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3wvvhfesf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3addtvnsd.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pehkcrzt.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ilzquact.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ixxwqjuc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fuzshwkq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kwuyhzhv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3dfounqwk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3rbztcqny.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bpxkrdvp.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mwhlnyoy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3eitvalji.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xyazovyx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gwhyfrtj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3iwiyhila.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3saxuepuv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ttyazbli.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3krismueh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cogcxvnt.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rhebxokj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uijqhobh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3evuxjzsv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3vzkelrhf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kvyxtdrr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uycrtnlp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bpyhuyrh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3tyrksugh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wyvyxfkm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fmrqnsic.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mxlxxiqj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wsoumwah.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xrppuryq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3oyuqigyg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zpvinlvs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zlfcogcf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ffsiivep.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3kwudcxxr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3cnujujcw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hoguetkr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ylgiaphr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3kqavohyw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3qgzcwumz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3hadhutit.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3iqvgehii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etcuqyde.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3flupqcew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tiqtoeai.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qenxthde.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3jditixqg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sywheicl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ivgkqbfd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ylqakhmf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cmdoqfat.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ktumdrws.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jiizivoh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ovhpuqgj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3pjhysxys.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xzpgjben.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3apdigmdn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ottflyau.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbqtzuuo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnpapiyh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3lychpzwv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gjinwxbh.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzjesizw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3lmsjadiw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dsztnoeg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gitjulqk.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jwzzkltu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bqrgpodd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3balwtnfz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3roufjikx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zjlzhuva.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3wdkeunbf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3tjlinghp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mytbrucd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ctolbhke.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygkritay.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ynipkyau.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mkpncpls.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3noksubjo.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3cqrzawzf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3iaedcnry.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3jysyrxba.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3qgaqsyfg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fiptxpjt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bklestva.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwmamlbt.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ybuvmdhf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3hhsgrjht.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3robczjgk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fselqqbm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ytjuwjvz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3azfgxjft.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3patkxywd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3wridhkkw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3znsviptv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3apoyttiu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3droqvefz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3zplcgvwx.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3aeawmmko.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3psbxajfq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3lposxxkm.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pidvrdwx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xdkrnbkc.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3vopgmwrd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3gvwmrhfu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3nsqlqnhi.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3yqbsjehz.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3gxznyvof.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3uzyttfne.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3pcfnzqer.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wtmfzgwj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3coyzizul.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3mmifcutd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3iaatljvo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3bmcdeoxk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3wmyprurb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqruboul.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gxpiocih.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vokkiocm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wvxrdtss.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3yxdllzcl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3emolshrz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3hjslazvw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3kpvvaxdj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3zvafzewn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dhbcpcmq.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3aobndsez.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3ttsoaono.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3daxduqyx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3suymohcf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ihivpmss.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3lgekgsyr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3tkmkoawb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3yrmtkpou.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3letefkbx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3criwtmkr.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3hgehnryb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikdrivwy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qfvsmbbk.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3seguwadf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vxjlzfzw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kmacqquc.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3dxefizup.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3luebgzju.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3lhlkknhe.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3arvjysts.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwqfnidp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3sdbqnqbb.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixonrguo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tydvvwld.html


<!-- 参考信息 -->