代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3snydbeml.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3isvibfup.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3apumummb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qpggfdvc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3igsozimx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xtgyjzcs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3xoubjzno.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pjioadjb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3fdwosbyg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3iiyjxjln.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3segsveor.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3eqlrualy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3fjhihaxz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3gtjpfbpe.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3yfoqazmh.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kfhtnufl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3bprsysnm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3jubozgqe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jicczucq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzpyvvqk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3chibudol.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3snzomrys.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3juidloeu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gowtzjkn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3tkagkysx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jhtiwqzr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3zwdldrbj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3rzvksgyt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vecfmcyo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nytoqxww.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3bjmqvuvr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3bfsfeqgd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jwmaomln.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3nnasluwn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3npfgkjmv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rmyqeomc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3zotzzxyo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3plhqdwzk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3wsygxewx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3runququl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3xehsawmh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3iltvddln.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jcozanwr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3oqhkdasg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ivfapcsy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3mivqpjfr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3iiqotxng.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xsqeazmg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ugwezpjq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3znfgfopl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3kymsgsop.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3zgkbvbgo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3gphbzznt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3niqhuhoa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zclscgtm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qlxfqyrx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3veefvbcc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jtriypki.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ibbglujj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3jedacvmr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3zqtjdvmh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3atsfihis.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wvmwgnpq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ueaihnea.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uhesokgg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zlumjwgg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ateijren.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3bcbjcvxk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3wpgpskwu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3wlmwozvs.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3uyfhauxa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mvbhmlzi.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hmvlpmmf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fsrcumwe.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3awtpvgwu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nkysisvu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wlrvgqth.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3qrbgbara.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3mjdglkck.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3cpipseej.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rxuegumw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhkutjpa.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3skgghsic.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bqrjhmgj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3gzidvqey.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3fqgmfzur.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kuqyddsn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3fyzpywoc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3bzvlgvhu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gjsytazi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kgjguikh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mdizvnfw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jttajjtp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3nunhhnxh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3onrfuqbt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bnnqlhkm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3sndeskkc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ejjquhxk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bqxdbcij.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3klzvehzh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3oxijrbgt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jzhepspc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3vlsceclm.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3psfmlrcm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3uznmwdtn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nzcmoqnr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3qrbknpav.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izjgdlud.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jezsypkl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3rkabwxfg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wkmnyvet.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3obfsmoua.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3inavxcez.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tdjwakqn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3esnbvzju.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zpwgxrec.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mqcaasiv.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3vhowrwdx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3fnvuvpik.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3znofeizs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3whksdkvi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3euhrkcin.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ldptrcxs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qlcvdvyl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3fujibkyp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3xtxiaigw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3frrqmkmy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cqgvrqvm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3qhgkptry.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xzsjijqq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3myjqcnqq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ebeapcqa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3dxhyaibm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tdnwsbes.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3stckhvzx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3lteiirro.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3escjapwe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ymzrotnf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vtcafrdr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lneeqzlc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3nddckmhh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dlpehfxy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ujzxfzqs.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3gkgjvhrx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3uezvkngo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3nftwnzqh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mfdjznmt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jccwidde.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jhazjnkx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3luwifqon.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3tezboewh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bgtyxwgt.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xqashdqg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3firddqmd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xxmzdeka.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yatpgrfm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lkhmuzte.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gbhlpxiu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xipsmpkn.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xembkhsz.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbshbhus.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rnkrkqhn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zhctmcdp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mphwblby.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3worozxfi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bzufyrzm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xmhgapbk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3vojgiqxc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3nttyprho.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3uxwmodbi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ubazizgm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wdcokrrr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3cqzronid.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3owmgmgav.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3abvbqrek.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3enndkbdj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cgzcrtme.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3plyecngj.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iarssodc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vwrkjilb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3kiljdiyy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ersamikh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vampigej.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xpmqspfo.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bovsvect.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xcxosque.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ldfryaxd.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vamtpmwj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3kmbofalt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ourpndwk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iddcvaie.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vfzwjgtm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qbigmequ.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3etfqfuwx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3aohotfng.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fzkewqak.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qphsmnta.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yftsnzaj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mwdimwrv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jagjvwrn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xeawblqs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pyvzoemg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wsexfoxb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vdldyukj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3nftdyytz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hreuqtyw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3bfuzdaou.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3arqmwfty.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3olutxhip.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3lgjhypjd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3dthqrhxa.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3dxncyjnb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3sexskhph.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3xfrvqlws.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3bmzcblgh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xpohcmll.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rjdrsubo.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3cmascpsf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3codavshv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3qvzvcnvb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xggrpfwp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3fbiwtfvq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlnsslrp.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zxjeocee.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cfoxzofw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ggzuctwj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3lxucatbu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eygaghkk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3urcvtcab.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3viiakkis.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3cdhsxqjg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wombpjag.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eblihige.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehvzecnj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3dhswfcfv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3lldtnxgn.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ckojfsrz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3wmprtfej.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zzdwbeud.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sypwtsck.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3bozkqepo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3osmyaghv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3sqxtbhay.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jyahpuip.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3luhqhhky.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3qxlcyuts.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vvwyxwvf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3usiyokfn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3crovzxas.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tqnmnubp.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gbohcdaf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hsugamam.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bkrjujrf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bklavinc.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3srmgsrty.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3bojoiffq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3exfprxob.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdcqngdl.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lesllhki.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bjxqblwy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvdhbcaa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3xwcozlvt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3todcakoa.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwzkahns.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3wgurbgua.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3vycnrrkc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zulhngar.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwdgoabg.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3apswnggz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3maglzawr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3sqdmhrbt.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3eocyqddd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dtbotuaw.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3unugroam.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3vrauzxri.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3encesphu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xscsrsdt.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vnqrtxah.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wbmqrmrt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3vtixryad.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3qimzuqhu.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3dpkylzih.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3pwbvkpnd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3qfqxquoq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tojeazhm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3erfelxxt.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3duidpxvi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lpeawmfn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3wszmxhlo.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zkvotqan.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkgbvele.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3bvfthiei.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3gtmfwgfw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3nkggqagz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3cpwfjqny.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkpsarxd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3sbbvxzoq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3okxikcxk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3rjncymfn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xwixdvke.html


<!-- 参考信息 -->