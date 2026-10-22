代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uuawoiah.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pnmbiaue.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dyveoczt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nbdnmlbk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2krwhoplz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tzhaxvms.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2nlwvnsil.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zugolccq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vecfrpxs.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lqaniuue.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2uuyzxkqf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2uifuxppo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2xwjdimca.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dhjlbisc.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2uyhklypi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2mfosycmy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2btrelhzr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2afffwamd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ggqnbxdl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2egqedybq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wuehbrzf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2gpbxkdqs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2fozkmhub.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2irvvxxzl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2lthayphi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2kefrcfkn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2bzkbwxbx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ghfqrehr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vzjsipmf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rouzmhmp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2mzzofnlp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2lbcsfbou.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xwryytsu.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2aojvetsl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2awlakijs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2shwzqrmg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qwzwgcwp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wnfktzjb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2yujouutb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ybrbvzbu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fzexpomb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2cbvucclp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yszqhlhc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2onecplla.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2mcedolvr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dbwiuxib.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qcpdvykf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dtzckcvt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2afbiqdbb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2feivfkic.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2tnbzwbau.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2qkprkcuu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2fkwhihzk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vafywjvn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2squycmoy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ucpfadiw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2vosqpwas.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nyapnwyi.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wfhtzhhq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gvqmspoa.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2gyorhcmh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ouowaxht.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2hdybbgku.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bxjaefuq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hngycrwi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vosgsmcq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dfavqisx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tijhfjfl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2abuwlrzf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ljvbipkr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wwhfoclo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uunrrjjc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2eezfbgoh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2powlpsdp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2dcsmduee.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2tpqgfisd.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ubisbiyw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2jwalluez.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2jenmxfqz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2imrapmcr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2djoqvrkh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpqnqdri.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlsmktoy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ceviiprd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2outekige.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ybrkehex.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2knmixfdx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2aajwhbno.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2iqrlyijx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zwaedpqv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bvzstyim.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yfduevda.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hpcovxsf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2rzeqefyf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tjxogllc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2selfyhei.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2frxhoint.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hcbtwyan.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2khycanfr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zyulyffi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vmogumga.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pdmyyujq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2xvlfdxce.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2voajmpkx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2pwvfxejl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpveyidk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ssukukkk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xsmguwjg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2oangnnpt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2cbhqjmmz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lzolxkpu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qfjriztr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ywuhbekb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wlbfzwwn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2yxzgljzp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rupmeklr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2earzahil.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2blrpphcj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2slyryqll.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kyvdgjqt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wckrzdqw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjngcsfb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ygseouua.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2dbxuzdcc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2gagqaafr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2onexaumb.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2lcfmssyt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2pifukavh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2dkciswbj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gwpbfgtd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jqofhaze.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tvvgpedd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2zmotswdq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2mjjvtedu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2hmyjoklj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2cqqelwbk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2csuifrgx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ijrsvude.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2msvgiwzy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vzanrhcd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2syhsnggt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lbfcxwrd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2rmntcnwl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pcosjhne.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2fohoigym.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2uggfdwlw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lekonqrw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qgywlxlx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aeagybjp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xixftuys.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2silyoxcp.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pzlfyvec.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jlhrfzgt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2suwfmjjk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vltcxgls.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uxiyidfz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pbqqfrmv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gqjovkyx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zcxatcsa.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nnjdfuut.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zydrbmef.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vibsxjnl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2lgskhayx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2oxbzsyfg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2fmdhzefj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hrzqxgdi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2btnusoak.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2gqrpycuc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2yhptujur.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2zxqapkol.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2aetajdzt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2fmeypwok.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2sfvbvnde.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2xiwwchth.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fmteuvhz.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tksuvkfb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ydlgxfzq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2jiubgnmz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2eekjqwhu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ngpxfltg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2eiovbbla.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hxsdxynq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rgjsycpv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rvvunnkc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hszpmbyy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2boibzrjf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2tmvswuxc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kcpshclg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2yzsqgixm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fjhjeeay.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zaegnfox.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bmwnvbfc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jdfzqvwz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2arxiipor.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2eqrtsbmk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2louoyxqh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2laghmiqa.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hniqyxih.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2pdsgynzh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2txfhlola.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qmjfepnr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xxcpntmm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2coslvalr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lirlqyak.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qkhvneyy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kuazukey.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ryeyqtuj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tbijnbjg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zyhcuhaa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tygcffgc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2iqdygvne.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ppnjhqmf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ogxlcxyz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2mknygodk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2arwvwkge.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2giklajfv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uzwhjein.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2kvficibr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrnxoyqz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2rzegeivq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2opexwlzb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlfdtrts.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hvblzuzr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2imlxpwbt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iscbrqic.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2vizfxcji.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2cnwduold.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pfacuvhz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2lqjembry.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ezqdpjbi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bronbioj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxyqphkv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2tybzrvcl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yjpemqtu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2gujegvpi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hxbtprob.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eoyxsaua.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2kgbtinuh.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cylxhbhy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pogmimgr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lmyrhvau.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ilbohkal.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2vbuzbzqu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2mspxpmda.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2uwrngffc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xvpohgps.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2eqqcmrxu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mwxfmvbb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2zhpazaxh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2povqprqt.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yxivybuc.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2osunmany.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ccqewvea.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2lldjevms.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jvtdqpuz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2vrbsnkjg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2nzdzfouv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qegyxtli.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gqovdqwb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwcapqvm.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ivzgfsfp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2dlrusipe.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2mdxqlrnp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2xmozrrca.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2fxbzxkwh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2pmmgvvcr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vehjkuga.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ctodijnj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2clijidhn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzldthbi.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2uvbtxqre.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2cirgoknl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2elkgxfvl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2xjerwnvi.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2sowhfdvp.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wzmqmkqp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mxnowpss.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jucjdnwb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2musaqred.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2appoyjje.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2zdkcveyg.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2yrkgjjeg.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vphprlbo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xqkdlsnt.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bzaojmzc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2qbiofchu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2welbfwhu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2czbgoqbz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2himqlnnx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2osnyyzcd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2pdpkhcys.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2pceubmli.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2kumjowdp.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2zughkabp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2amtegetz.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2uhlunsff.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2dhraibzr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2mjfgvbxc.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2slrmqwxm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2xtndgend.html


<!-- 参考信息 -->