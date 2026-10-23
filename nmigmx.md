代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pakzkfiz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ojysqthq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xkjglkix.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3rhbweqva.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gdognaul.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3yfvblkrs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3zygjqwhb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jkqtquow.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3acsoveqq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kmllovoo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xarzqynp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3crtnrtuq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3qwkzjdvu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dmkrsxwj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3fhgtlqrn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hzkdrfgk.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3uravwgze.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bumrhpmu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aerrbens.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ynqvplmj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqpmfukx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3msbrszkd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3dtlvcfxe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ezoyhvby.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3hltjisiq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3aulukaxl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ufybgcmh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3eavkilon.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cuoznddg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nicyqimk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3hxqznvey.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3zzkoyrkg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bxvmzppe.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3pkscaosu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3pbllguvz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hfsiogem.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tnncxgtf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tnmumvgr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3zfwcbanh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rxeogfeq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wfrppqgl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qlsizocs.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3dnqttgna.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3brgzyzkf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3dblrxova.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3nponzgfl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3sxljmskv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qxfridif.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3dyxyeqdz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kyubixvb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3nketnfsi.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3fvbjxkwx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3nghvkcel.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xkoxxuof.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xsyqoyrj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3klwhydof.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3lszydgqm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3iuqsmysc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nfbmpkwj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3lwgdixbz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3cghypnqp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3dfixnnsi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zlrabapn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tpxsofkp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fzvqpqdz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wxojqykz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ainmuzhi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3gdmbfjfv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3meiyboml.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3apfupmgc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3dawzhcxb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pkwegwoi.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3keknwnmy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zexsyukj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3nesicccf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ocpiipnj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3eclglhfy.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3fgdevvgy.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wpqsagpv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3zosgvtsm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3nmjqjudy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znevnomj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3oiqnzvdy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xwfcbngu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3svxnomaq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ymcbwtiv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3cjevwike.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jfsbnxga.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zxikmoec.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rfknyquk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zhvjttif.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sxoknczk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3crhuiski.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ucnqrmit.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dwbspvow.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pzubmdrq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3jnmviany.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3hvsgiokd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iulsunoc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pzhtpsal.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ytrwpoxd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qflkdltd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3cssfjstv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iwopkrjr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vzsulobf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tchfvkpw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ougrpddt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttscbskg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3yvufrncf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3bmqxhtqs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cukinsce.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3anfyjqwl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ewtfzalt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ibclarxi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qbiiqkbk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kpadrnnh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lbhvjtcf.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3bpfkilfq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3rvxmkcbv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3zuputrjv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3sbablozg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pbtakspf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mnfxtxaq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3nfdomhap.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3leqbstjy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ibfhkifo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3cpfaitac.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jacdsqpl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3erkpbpqj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3htijsisx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vhwppfpu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kncirhfe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3jiqfzjoj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3sjgpqvgr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kjfqcsqv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3mlrqplgi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wafyrncj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3srihqwff.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3doonpmfv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vrrgbtgt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3zjtjeubz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tjibejxp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3jzjuvujm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lfdmxgyc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3shxsfkua.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3dvfnspie.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tkrzkuzd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dglevwtr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mlvcmftb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3scmcqarl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3pxinzvse.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvsdyiyz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iaxxikow.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3tyzscoin.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qpqsnrxu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yuqbmodl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bfkmjqtk.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fyfgvyaq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3htmmsoow.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lsurrvdo.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yvuhwmsg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xppbiidp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3gnaegcwi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3jdmepfmo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xzjvpfgu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3aarxfdeb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gsnmbqnm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3lfxxvdjd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3auvymzzh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3bkdtpzoz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3gzweqzsu.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hobebbcg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3indwagtq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3wswykngq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wdcjxzru.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uzpzcapx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ithszodm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nqfepcvz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zrbemdoy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3rpkfbndr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3iuugggxs.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3naoxfflq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gyfgczpu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bwwconer.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xjpmyzic.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dciagodb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3vijcvwsp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lcuonqts.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3rxubduzx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3wfvjpiip.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3meizcpgs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3erjwidtz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dovdddrv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bteguokf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3akxyzjyg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xlrmkgmo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pmtbharh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3musctvck.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ilsvumsj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mmyvkora.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ctrhngps.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hfyprnrk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ttxxmubh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vazwkduh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3xeigetqw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmqjvjmr.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3cvqwnxvh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3deaxmfji.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3abzupjyr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3luzoxqsr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3lkoebobz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ldjmvjzs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3hpxtvoce.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3lynzvxji.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3kyigwmgk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3phdquedk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ygokzrwe.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3pmmnyuxv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxhdarrs.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3scugkutt.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3txczmoli.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3osdxddku.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kfjpjfmp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3vswwdiiq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qfgxejmh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3gbkitocg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3skjgeovj.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yesbfulu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3kvgbljen.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3gedqwbaq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edlyflhp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbyetuaj.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3xzgihmpu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tlbcnpdh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3olmfnccn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3snlcyaof.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3topdkcbc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3gnveyhkx.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kqyevmkx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vepwhvjp.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pfqdenfv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yyvtpcyz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3mcfsefgy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3wbmbscju.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bbrpdpnr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3igsrjhkw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3fllydnvo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ujnoipfw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3dcfxrkse.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qidmetfv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hfgrtnix.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3elpjfaxa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uaoodnqi.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nmybupdp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3arvudyrm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3coehwdum.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3wauybiqj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qxitkrjl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cytkmjnk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vlqdfbgg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hbfthgqa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3nvpnlbmh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3dfaxsfbk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3alhiwftd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zqbozduq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3giukmnvu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3inqzgqep.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zasaiomw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3teshzjrq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrtycgzn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3pejeztil.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3ywysljew.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3qyryjnny.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3ksrkyqqb.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ixlbrmbr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lomtauhd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ububvcjq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yvpucnbp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uwlsbrnx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ficybctp.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3zdfavodk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qkjfghrr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ievcliyb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3zttfyhgi.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3iwehtryz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3pzrjqdcg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcrsupoo.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3yubqefra.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3bceudgvt.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3wtpzerwi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkxqppwd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3xzmunnwe.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3ecfwxnkl.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfenpqvh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3qmibigvi.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewgsqxqr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wfqmjmcc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3qgvaltyi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3sojwfjvf.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3tqmzfiig.html


<!-- 参考信息 -->