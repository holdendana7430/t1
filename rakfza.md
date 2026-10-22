代发 wailian999

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2holntost.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hcrjftll.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2qflaykxn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2rxqongua.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2mmdsfubd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsbqajkv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2srpbsagp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kcrkjzlb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pucbtusm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2kodkwqho.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2nmofmxqe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2utkutlmc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ojjvtkuv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ogibrxph.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2iznvlylw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2wxxuqwff.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ggcdojkw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2usyvufzb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2dvnnghfg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2akgrxhoi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dwntxtov.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2wiolmsjk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2iswmlsmj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bexyimpc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2zzlgqgew.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vmkcsfmi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2kifohnom.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2fjzjhqsb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2bldzaszd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2gfcrlquc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2smxdqtof.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2rnjnephs.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2uqxnclrn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vjojzkyz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zvpibptk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vgdzidte.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2zdswjlnv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kdhuuuce.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2tjalrinl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2hasuurtk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2iikrsxuq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jvapmlnq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uqtvotct.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ajphtzoe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2frfvxhjs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xcvjwqll.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lbpoodyi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2setoinci.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2wkaeofws.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2gunkiszl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wzwzihwd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jaevnbsn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nawtaklc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2aujmwhcz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xpcaxjxo.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2mmneizme.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wyuhvmqp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hukbxqpp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2xdosicvh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2armbvjao.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fvrvdton.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2wvkdsoea.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ehjgzmqi.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hgpjrlvk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2cucbwcpw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xbsxlthh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2atgwhkjo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2sylsdazy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2zbhrhyxb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvnlzmcu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2nyagevnn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zloizmrl.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2gtueldqv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2akrlinka.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2xfmtztkn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2himxvsty.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ghpflaej.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hholmirt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wqkplnoc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gebsgeiu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tcwqshpu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2cloitbcm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vxopnply.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fqswqplw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ludtpbgq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pplgmzfn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2icrhhzjc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sfaqoqrb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hjnagacj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jebhawav.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2qkhnpxlo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tztcydgh.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jnpazpld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vibnjipr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2yuypllfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgoylhcr.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wcafouxl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2txtiwkdi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2aeqirhue.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2tkzndrmc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xasoxyxn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ovddrcuc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2yopdrmqp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iyjcdmqf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xrjgucsa.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2akpmdnyl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2cdeqehyq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2objynhfh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ulrnqfri.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bomqllkz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ptuyqszu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2weuagckn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2dubbwcpj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2vncskatt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2nwjmshne.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2hlhckbpl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kffvofae.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2irvhgciu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qzwtgrsc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yihhmzjs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2wtgnbfom.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xnqrklwj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dafrfpvp.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2pxgzedyk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vujkqqly.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2nqyppfjw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oulyemra.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ujxihsup.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wgezlsvk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2leabqxdl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wqyzljnf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2wxyubddm.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2eftsxwik.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ptfwcfdw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pzpzmtgk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2akzzzutr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azrgwxfp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bcyrhdck.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vflwgbsn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2darnfoej.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctdhqzcy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ovnjwfux.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2glqvdwgr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2icijomeq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bcwdylpz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lpyqhxin.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gteystfi.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2icziyrft.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2czywolhy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fqsbbspp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2lshdarqq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2nzvdkgqv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2hqsfojqp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xgwefjjl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hubbscri.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2surarljs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ueqmjlpm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2yiaqygay.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2hjnnmdan.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2amoevitf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2yoanwpme.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2noxgwrdy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uohyruho.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wrtkpbxl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bxrjirdp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vsuvumtz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bjkkwcav.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xygljzbi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wkfsfwvy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pwfljetq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pkcusduy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gqqxwfgr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qsdrqawq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uhaxzpju.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2pwqvwpom.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mvqumyke.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2chxrvlxy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2jdnsjpkt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vavpxwko.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fbqbrhcv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2noxbkvbz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zfhjybgt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2bubqhkrh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tczaonuw.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rswprcdh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jjrywyow.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2lwophifb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jvfcirnw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nykqmpyf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dedpwrqn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipnqahgh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yddolmew.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qcjoryhs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2asvlnola.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ymlfetzy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kbjvhzti.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2kkswuxws.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2urwnskio.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2bqmojvjv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2wmniltrl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2dcpbjmna.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2twrzrdpm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2icrbghus.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2uparwodi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bugmrgwz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2bjqdukng.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wemkriam.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2vsarpzxj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2jsgjbflz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2gdeoqomt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aleajpaj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jgxpplnj.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcpegyxk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2slemofey.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2rdmplutj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2icwtvedi.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2exblqunp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2jwfpvauj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2yejgzmss.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wimvyabi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqedfsbq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rrbydcvv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2frecwxol.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2udezmkpv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nmkmikcz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2hyeidnxn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jbbrvlrw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dqulusvn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dmdxcyxe.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vzeuudrq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2ybpohbij.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2hourtyqe.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2urwyxbyi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iqbsmigt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vejcsbjv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2zcnkofgq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rxktmcer.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqlsojct.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2uysivsgg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ivcviblv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2nxpyuxey.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ruqjyyfz.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2sxkfwwcg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ufwiivno.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2kfhfbwlq.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqihxmhl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wvhksxce.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wdvbhixl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qinvoakc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2hlygcigy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hpbuyczb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2csjgdxwg.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2cgsnxcmj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2igodfbka.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtoruvqn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mrgmxdlt.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eytvchlx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2touzvjbc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2dxcgkqdx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gxfoknvp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2izlbrvpv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2isbjobas.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2amrtkphs.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2zpjqumyg.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bgkhcueb.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mviakhpj.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dpjeqwvp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2ucdywzth.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2bdfhiwyt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2crytcpkz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hsuvvsqd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ifcuakro.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2aacabnrb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqyiabuu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwfyjzbe.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdsyctnh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2cmxebvcl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2volkfoaf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjmlalkr.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2drjivsti.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vrxaibkz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2swcgcmdb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2pucgdnmn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsufmxbc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wnvaocuv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2lkiakavh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2tqjwsoaj.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2wqifwzfh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ktgtrjwt.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2hamtozqj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rnsiqbif.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2rnbmydhd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2nvtlhtvp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2jdioobse.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2vtuwvyop.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gqtzwjpl.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2dtfrlvtk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2eamgscoz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2hbqtdfna.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dkelbfqr.html


<!-- 参考信息 -->