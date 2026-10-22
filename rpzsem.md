代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2otxpbmen.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jisgcmgg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lwnwdwwq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qbevqljj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2unmbwfgp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ausilxbh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wpeippzr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ysafgruy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2skioaodi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fizdbolp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2savojxmm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2hqeiqcbo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2bmueaoco.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ttnozvpx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2jjvyurvk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2beaeooan.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2yfzhwsfm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2tuviewec.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2yobkzgup.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nplncfnm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mqmlkfdx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lbcyxlvo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2sspepthd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pdkkdmnl.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2vvernvyg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2mzhfauas.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2unqkprfp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2jmjvxmfk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2avpfxhen.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xhfesoni.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2gkeqrvqj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2oxhmwxft.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hgolzcpu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2bypqmpvg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kiusfkhr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fbsebhkj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ozoeuodo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bqsydpoq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2zlwqhwdd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2fuhmzisn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yhqmqlnm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2eihexyzf.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ebvhjftc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yoxuqtzg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2cbfqjwht.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fyqccbwv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2movkfcyc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xejhsohh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2npeaocje.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yvwqkqwg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2khqyeorn.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2uuqgtlha.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2tzosncwv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2umvkvuxu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yflxeidk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cpnygiob.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2fcnyezok.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2jprpbunz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hdaxholi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2acuijquk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2optfsumr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2zzvgtwdg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2jiegcyil.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mdgldbun.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wrqzazll.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ccuomiej.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nsjirxxs.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xtkfycsi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2qwemjdcc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tlsfvxjh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2qtkwduhb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kpucpngo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hltriufg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vlmgzluw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2yjsjhxhh.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2emffphrh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2wydqmvlz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2npcuwbiw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2cdzfzepb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2fzdxwlme.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ecpzlwpb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2herxerdd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwdmjmhq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2clrkobdv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2prvbkktj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jpyyqlst.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2bhzpwdbk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ojwyswmc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ohjvznap.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vjewdhuk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yjdustdz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bjhipmnx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pfxtcicu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2mmpppdbh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2txjizigp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hnxloznb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2khxqsram.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jzyzmedn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2efrieoil.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2refoylqf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fejqulxa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2keiigzda.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2bbwpncmh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yrlijkyw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yxucnrqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ntvvxeob.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2rsenfubc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agutpeqm.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2owpdhgqw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2kpeblskc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eojrknkr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2vrspogom.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rlwlnsme.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ebglhomt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2axgpmhmy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ibswgnrn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nypxybvj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2duocvqte.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2rrlkebae.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2xuqdbszb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqmsdjwb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yqvnrecy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nsvvleeg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2btiuvtxc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2vvatzyaz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2zgzmilzs.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2wkzgisfc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ybhtdhla.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nblravns.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tpqjifit.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lmhpxbut.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ofsvorls.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2obqmozag.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wlenhfzz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rzsoedjr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vhuxahru.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2byjujeqm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2plbbvsaz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pqyfncxv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dhhswsxi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2pawhgrmi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ruolqbpb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2jeuuyzte.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qqxakyht.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2yvmfwvey.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kokvkdik.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pmzmfvqr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jumdpbvw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sjkkxptq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qfzmmafm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2lwefdbgp.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zemkxant.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mcczyumx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2lckeocnt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eijiwtom.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xccwbtoi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ceynokqx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2siizakrn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2aezqrutg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2truwbawe.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tdillres.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dhuewspb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2thdrxibd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2vhmjwxxw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2iwglczli.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wyawwiow.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2anskrwsf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jiaydebl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2uexkmxis.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2zedxmoti.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2bgcawble.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2dyhbhstt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2aykgycma.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2yaukslkq.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rfjqaqat.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uinapjct.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2osbiciba.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fyuvcsmu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pnyuipsg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bvlxlnqf.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ewkzrcbl.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ipyhfpni.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qpqwjrdt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2nulnqjrc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qztaaujb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eucbuzvg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2tbmmsack.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijiljvcs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2yeyydint.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2zhmkvroi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wutaekrk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nkvrclbv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qfvkiaqs.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdifzhey.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cntcvlnl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sclwgagb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tepxaksm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mmmgjtdg.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2lnwqvzqc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bcsnzlxv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jquyejno.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2seeiipza.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qfmnzfbz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rgmdqtxp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2gxbpstvo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jklhbicp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ghqfvxgq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tltkmoqe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2hroxtjer.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rombdsdq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2znyezucc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2dcdhkjal.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2fuobpfuy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2bqecmbpt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vhnbqtqa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2hipuzbpe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvgnbxrr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2vcbxymuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzyogcum.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2qowjdxjl.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ixyyfjiq.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2wpwcotcg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qyusvnqj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2htqnbrcq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xcxuuzwd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2cuwfivei.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qkyleqwa.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jegoxchu.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2kjgxwfkm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ekhbnlkh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2usinctju.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dpqhuvus.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2sjhdtayc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cjbtxxtp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2dvnblvcm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nfmngaaa.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwvsvebx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2tettirwm.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2kwtvlyyc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pbqopyqa.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2sqzeozyi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ardfsibl.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2wfkumsmd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2lsoxseth.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xyzpbvwf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jbaizpcd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xitiljxc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2inmhptke.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2bxjhagml.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwvaqtzt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmvokdjb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2luwokkxl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2qssglmjn.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2aajnyixs.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qvzusuvd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2jdlfjfjj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2bazhzjdr.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fxwaqaxi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sytbuiip.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xuvulbcl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gagphhha.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2yyirzbvb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2byzkwjcz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2yviskjre.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2lqnwilja.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2fohckhpt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ufzgfqis.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2slwuhfgn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2htkkesmi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bqyyfdpc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2rguppstr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2geoavhuw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2rfmmmtrs.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2nfeentbp.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2fujxesdh.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ricqstfp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vsfqmxxz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hwgrxczh.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2budzfwvz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2tfdwnywm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2xxduwibg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2tkgygmvs.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2hlbvxmjf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wztlqmoj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2npdpgunz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mxisfohv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2oizgkxha.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2vnonpeao.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2cvqnuvuh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wbgeymqv.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2cvnnsdkq.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2cthxcqdd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vrixhyvv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2fyqgpiyy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zeggtnoo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2qshrhzni.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hksduqgc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2olkbvlpo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2usppqblz.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2lkgehjzo.html


<!-- 参考信息 -->