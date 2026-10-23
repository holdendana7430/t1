代发 wailian999

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3iakmkzmg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jviadllb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jkjkmyvh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3nqsovvio.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3mucqmldm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3kwfjhflk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ohzywiji.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3skyqerec.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3mtvcnduw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3bpvvelvj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dulnbeej.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tejjicdo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rsjnrigs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hjtnqpcw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3oivdniwt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fgvexncy.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3zzhlrwib.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ttfjtebh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3ucdnwrxa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3btdmvxqb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3whqxiric.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ogvbfaay.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3rkqosddc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3gzposotl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cngpybbx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3tczdihyn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xvrtehme.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3widdhtfg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sfgqyxpn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3hhtnuzzs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xnitbjju.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ezudfrfe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ggtolqzt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dhzbjegf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gmztoqit.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kclefysd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3qumppjnf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rdmaqfcx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ubraxtty.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3otfacmnn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3jsnnaokj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qqlpygsg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3fbypvonb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3gfiadnrx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qnvzgfyt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3jglexzxu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dkbbckfn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpgobcnr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kbzxwvdn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ictzdiwy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3hbgvithf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3qxqtojws.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3juqiphyd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3upwqnykf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3sxmfnyqd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hkhpqnya.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pidhvgja.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vdzhqanw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lkltntwv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3aolmylig.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ewitadqf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nxzslnua.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3gjfifjam.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kvfnkadg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lbioedti.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kfmbfbdx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3okdevxzx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ktwakvop.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3otscnalq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3nhtmpayt.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3qpefdtpg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3zltnmvej.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3njzcawyz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3clnyfbqk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3tbggzpoa.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3soehlhgv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3izouewec.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dmjweffc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjwrvdps.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3uhphfiqb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ttjmuiqp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zqewfnnt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cquuzlmq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3egjkgjni.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aknfkodl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3mtdplhux.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3egajeatx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3epzkwpoa.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fonpxhks.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pkjgmnkc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kdjnkdjh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tddbnhhw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zyfwtylo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tmmezmte.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tjzloevl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nftzcirz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bpslzmmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fkwzaqjw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3qsicetjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iritpmlc.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3pdalnmnd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ivkydqqe.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nxcyrsin.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3gadlgtgy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jizxafir.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ycgqkrya.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3vnbchmcf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbhjiagk.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ahpuvhvo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3pivytkeq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3qoxdkbhq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3jkzmjdym.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fzzfjtwa.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3iibovbrq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3nhiimroe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ywawujul.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3eqdwewzd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3cpktsvux.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3pyhkqrko.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qeqdbuxd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3owwmnhcb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tascdovh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3btqubcpj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zsminffq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3roxftswu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3rouuwrmd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3smbytwtv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3sxarqbif.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xjhyjvvl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3egbpiokn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3clblyxdc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3snyfgmiz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3nzcirjln.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zsxbwbxx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3oukctsiz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3advivcqp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wdjfrfhy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3rzupfuoa.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jzzqdszw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hatkajuv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dllotykg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3niziyrze.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3jhxnflyd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ygktcatk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfngzelc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ucxfpvly.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3olowkfjt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hgxiomga.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqrkhtfu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tpvnaqmf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3esdfddjl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjtjezgy.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ppjysrqw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cvybwqbp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3npehupuz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qsrrwdud.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3pdyccsii.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3csapartd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rqgmbjej.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3uhkxhziw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3qaejudtm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3inmaytbp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3omvcwkge.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3nhbinnnl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3fhbkknqh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3emcjpfwf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3asuqfmeq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qjgeelbn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3oipnhwsa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ayzfucdj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ubopakas.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3vsuzvgnc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3uhlzckgc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wdtqhfzw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mwcfwjha.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3irurerlb.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hwxruisy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dcqskhrx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3kvebwqev.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ahefwvky.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3efucqmuu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3nranwuuo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vnxcsmwb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oquknnjv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fhahebrx.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qnirtdiw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3zexparuh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qzrxfbob.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pelvhhbo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ptgaxxot.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3mesxmqjl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zkezzgja.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ofpwceav.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jtlyeyfj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ftcdvnhe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3kghdumhu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3pwduwxmh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjjndjjf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3qfwznbgq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3mrdtswvr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3reveyldf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3pjagdwwt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3fvdcvebv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3gazuzkol.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3wrsxlvdc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kujwfuwf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vagwqjax.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3brchlihe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etnrmdzr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3jugixqma.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkbaqpac.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rhlmvqog.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3aesonlht.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3mdjykkyk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3diuzjwiq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbvwhghm.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3giqsspmg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pdcisvcn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3jizmflgd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzqiajbw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wkjejqjv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3hgozuewh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3hwuoxdiu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3oksxovez.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwpouxpj.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wffuablu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3qzawsthr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3tcxmljtg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bjkgjzng.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3fcnfngvq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zvsmlfhi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3bkvtlxcw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lghtxifi.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jmflumjh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ryfwuvcy.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ogobcycp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3buxswtqa.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3aoksolqe.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3hnqxjrvf.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ptknmdam.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3czojlqlj.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jbgbytey.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eypgnrlc.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pyxmoizj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3crmraagj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3abtycujm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3awmntneo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3mkcgponq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hacnogdj.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cvkcogej.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3usnolunu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocxgqeat.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yqfbsuqh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3hkxunyac.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3egvfwuca.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bgszrquh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3axyrtryu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3otlalfjd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qucdjnyi.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zkodxrbu.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hizwyiot.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hpxcocit.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3ngvaqrin.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3zrlselci.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3zivlyeei.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3orwdrrll.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3onhlowtu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ssfucmme.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uwmaiiaf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ceysqjdu.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lfdrsbvk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3pzizvxut.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3lwyybazb.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wlxtqxal.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mvtgjduy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3cpbexopx.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3flzlsnqu.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3bhnodjaj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3ncnpnjvn.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3iwaoawjh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3rdlufusj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3idsgbgoc.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xbnxgasj.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3bmjvkvtp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3aizhqlzg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3wvpaqtxh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3armeznkk.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3kcaugbil.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gemhxbsv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3bionzfrk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ivzmisvf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3atwbqmbt.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vpmomqcv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3wmcltogg.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kkvxamew.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3irhxjqtf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vxlukrxq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ywsqxkiv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3zjdsgkrl.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ryypnsah.html


<!-- 参考信息 -->