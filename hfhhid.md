代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tbcmysxw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3smdlhhvi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3wtdtkyvt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hhqasxma.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3prrfunev.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3oqljhrah.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3omulwzmm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ogdexzmd.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3oddnlajg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ellbxumw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3adkskfjf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3tfhbbffb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3fozbukpw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ovwtquvr.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3zaoonwut.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kcrkxokc.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3djhbjkqu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3limaytuy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wwbpdltt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fpsybepi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uunpqeqg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zgcbadek.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fvhgkloj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3irqcxxyd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3nunbtueg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3eiyzgcsf.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qdebunbq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3zkvkgxjr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3lcwqwavm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3bszyapru.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3yyarhgsf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3dpepzlge.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pcxuvqjp.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3hzeopesw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kapaknum.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eqnbmpdh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3frwmobmc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ekatruog.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3hynrgbnr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gwzfsnsn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ymdruqlb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xifpeagr.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nleuiwgk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ihsjsqoj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ptkxbbrf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jdhzpube.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hwyvpeku.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ulbiuiut.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3flfpiaro.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xhnbwufl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3oodkaqsl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3vpwvarua.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3nqtrfyph.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3greoylqi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fgrjjazx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ugsnkoey.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hmbpypii.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3lzoqjvel.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wrujysjv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3kvfrjhcn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3akolawnq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mqfniflj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zqbbtjkq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rrmnpcwc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uonozgjt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mugkrgmn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3obpsgjxm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rrvjouai.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3paxsccax.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3msztbehd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3epskwtte.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qufrhhfp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hfnqbmdd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kroaxsmf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aoxqhgpn.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3illqagtg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3trpfyjmt.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3wvwndtjs.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jtcgewld.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3vqcbpnjf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3gpyjmguc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3edacctlb.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3homtraod.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qebcomcx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3tewgnxru.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3otjyhomv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3hnwtrmeq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3mtfcojgx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3kvfrqpsa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lrawdmlr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3plstwtdu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3grzyfiqr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3crsidfay.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3rucvtegb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fqmkqkoz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jsvxrwsq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3iordyscc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3rnkpnfby.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3kiwjsncw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nunjpkcz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cfopxqqn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wgbtkijb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3eygygnwz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3onmfnbxp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jhejsfjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ybmvegaw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ilsvczfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqpraksn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3sgspestf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3qfvnumqr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gthewlxl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3vhmbmiks.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xviiwzop.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rslsjiys.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3tyeyqpcz.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oejyloos.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nvmiwugr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljeowinv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yuyykaga.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3pgubncox.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gxwwvxhv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dllvesrs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lqfdeghf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qvbkhsee.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3exgpbwkc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ueujaerp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3eppgcapm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sncthdgn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lmbmdols.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kauabked.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gnybutib.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gljskeid.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3znnoxjnp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3hostlsfv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nphgurze.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3wunbjjkc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oajnxxzn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3khizzjmi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3llcfbkav.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3dtopudjr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3celgkhtt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ibdduehk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3odmnxnqd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3rwhubnub.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3jmxdkptq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3swxphxuk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ibevurvz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xohosprr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bkfxpokd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pdhqsaxc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3wgoqsfns.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lfbckuxs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tghgescm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3vvluikzv.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cbgzpper.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dincuvts.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fnowzivr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gcbqysck.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uqnvuppr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wernugak.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3otdfocuo.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fgrevzjl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mekwoirt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3eiajbzvt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tazvrsws.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lxduwupj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3sxlzlrwx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3uvkenlbv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3shonblet.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vsyqpblo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3lltbiqyz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3viwzjywx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ggndzlcf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3fycusfqn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3swvjfdzq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hjgfnjqc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ginrgfye.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vmentzvq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3vblkirhp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3hbsoazdz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3mgtvzjhk.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3imzrhaze.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nvqdpxmi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3plojjptr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fzbjtpxw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kqduiepq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3crqnsecw.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fippvrnb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3raytcanf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3yzcpdqwd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yeklsgoe.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ixqgexbm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cnejphkm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lynkfqyd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3kcmxjnnk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3exgcwidl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3undmuqwe.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fmcleaen.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3qkolheni.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3linhofoz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3mlnwmgne.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yhhgrdnn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nspoiqam.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hpyxcemk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ogmefxzn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3opywkgnq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3reiteswh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3exnjysxk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3pmuvzdyh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tjacipyj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vcqvqrsg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mtphqhnu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vevmkoda.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3kvbytjtm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rfyicxeg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xgxkmyir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gwdtmzql.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3fhwkkcjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sqgcsoam.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3kjjlxenp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ussavxum.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3kmozanuf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ibhamkgf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3lygeiwmf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zoakkeln.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3bhpwdcyd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3fosqjtxg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mmkhfnxq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3yozqcoqq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3emxbhoov.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezptrykh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxqpomtg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjdprzjf.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3grlshtej.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ocazjivj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lzadllqt.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kpvfkytq.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3mlqlhnkw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gnvevkds.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jjgjwnse.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ryquwpaf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wucxopsz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3yrilkhyl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3uponhrnu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fbyjawng.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3shdxvwly.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3lcokocuc.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3phzazywy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdmcwlzk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfatcubr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zlkfsymn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3adipfoqd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3adgfhcbk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nywrrgzm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3kqjsqfqm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3hahcmlhr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ckhekkiv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3noeemrjf.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ycnjsvnc.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpuwwtuj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zelmhnzl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3czqnrzaq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3vsxcprdp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3eynoqroj.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3uhucduas.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3mmswnvvp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwmslgfj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oidsmuzq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3evejsvim.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zoqqrnth.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3bisfbmzn.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3wdrizhsb.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3zrjzkymn.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3pqcunhlf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ltelpwhb.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3osiifdwi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hgojodcg.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3szrvihuh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bobhuqpc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3mfuiozbi.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3evvbezal.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3egumcaug.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3atwfsjoh.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3dobiragt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zuauooca.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3qvwwijii.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3htzimxym.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3libmdizl.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ldsxlgts.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3tlkgpfae.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3hgriunat.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3umxrukiw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ebmwwsap.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3jrefwhdb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hcbdqprn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3qepnhtdq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tipeuatj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3lccskqaf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3texakyhn.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3bcwyhrrh.html


<!-- 参考信息 -->