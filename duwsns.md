代发 wailian999

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jfzipvwr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wszagdzp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3egnpvsju.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ewszcksz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3vtnktsul.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3pcprofcu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bmwtrdps.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pjpjpixs.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3natbhgrt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cajwkpuf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3jgdzvlzb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gtyqnkes.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rokguunz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kvzflykg.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mptkqntv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3znnufwby.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3fbasotzx.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fucdahrr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gfsftpzm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ppvqscia.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3znauvijs.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ixgpcoqj.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3exuefbfi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ijrfvfny.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3qseogdoi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3kifariep.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjtquevx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dveazved.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tlfvntti.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ogfopdfw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wyjejmth.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xxqwqwcb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3iseqqvjg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3cgkzwzac.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3welwnxbf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3itfgcluq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3utzmzlyh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qlbijtyp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3agtttfvx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3hieacomh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3zdhbrxqz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3avlqcfxl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3gszowxxc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3gshlxish.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jffszvbf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ngelxayy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3acsaaqwc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3tgafbzaz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aleobmek.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3rtzocleh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ihxrchsw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ervtmazh.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3okymsdfa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kpmmyjni.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lzownvvt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fsdhmfzy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3xykjubcj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3cxceoykm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ubrpnppv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3dfxabrdy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3wynhcbat.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bzcsfzlp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqkhdxxo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hottgvri.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ykklmzxm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3vevjlynb.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ogjsbsnz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3grxozznt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3btceogui.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3udvkaadp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3xsbjmhxy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3knbhujhf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kxmfpsvm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fhowffsw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3avvkqizp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3gdqsdief.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3mvqrdvxy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3oxbcyjhv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3dqdowdml.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nofayybt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3agmczfky.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3eyymkgsl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3qmqoghky.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3hgpssurx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wmnmmhgs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3awkgpjjf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3fkeegbuy.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3cuqiuzyu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dlxpozir.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3barfminp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbcjmexo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bzyfovur.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3novoozuk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ccpnygbn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nuijtgzk.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3rmwdzmyl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3lffjpedi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cxloksmt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3awtjspvl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qpdagmpv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hgalfrma.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3xrkchove.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rdfskcpy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vybkqbgb.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3wedmzisa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nhkywrvo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pybnydlj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3rksclbgd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cqpxwsde.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3yejhbucm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kshndfqq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zwfvpsnz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hxjnkxag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvssdjvr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3qcetdyot.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvmldumq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3lgsrjdls.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3hsrxwdie.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eyqslccg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3cpjgvahr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mtenmxcb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jkwcmtaf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ixhtgkop.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cqelmnwo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tizmzaak.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xixjxzbk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3twjfziit.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3uyjnftdo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pirpdqcn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uwcxmezi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sikbdhms.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3sabztgis.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3qsyxlmur.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyporxyj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vyoopptq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3aggogjxl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uogijexm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hfmntxgh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3psctgwkg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3menvmwbm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3fiqanhrz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3cjulkdzp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wqdhwtmn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3wtizphta.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ovnqteqa.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3vvomtzig.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nvqoqjrk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lpirpwod.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3gyotkbay.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3owggkgwc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3kdmzivul.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zmdeyjhf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eldvxpdu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3nmbscwnb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3obsquqhe.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ucwgfcar.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zplyocfs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vilxsqme.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3wtopxxlo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wwceklba.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dcqxmdee.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3usnjdshj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qdxfronu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bmcyutwu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zckmuydp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ypsifxnw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rgdtsnop.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aopwovot.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3csmlqprv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uvtsnoms.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ghgfnedw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cfjemvij.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3codftlcj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rbiafbmh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cqdmjqfa.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3aziarrpy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ttoxxznk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3rmkitthi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ltodagse.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3kmukmhvy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ogtmmejr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsbtghyz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vfhlfsva.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kplixjht.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3kphwjtdp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dceadivh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3cgjegvzw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3szstrrco.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3vdlgslcp.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjytubba.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3unisjpja.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3uyvdbier.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vuxjqnkb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vczywzro.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3arppmagq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3znhhdpxs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ibimqxqx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3aujnikpa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nserjnxx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rtbveltd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohmidevp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jtfzqmsc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gerergtc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rlhukmzk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jzgfzuuv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yqkvttbt.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3blojnhan.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jvmdfrtl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3uurirnok.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3poudzktc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hzockejz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tpqjdmfl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3iiymaeco.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lnulujgp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3oqwkgwrf.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3kskfujya.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3zcyvjqhs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vfpyzizw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mhenbqtr.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3xqewkpbe.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3bllnvryx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ltlfrikd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3wueiyzhx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3eyythvff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aesqrenk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mfhkcavq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvocqopw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3thhnxlos.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3gvohhsup.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xjtdmjft.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cxozxxqo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrxlqpst.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xdgykopc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3dyezwqyd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pmsashgt.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lcstnyqk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3zxmgtygs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3hihigzhi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gztqcwph.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cxsgsvbn.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3btfitcre.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jcqmfheb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3giqymwrg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3aevgovhj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3promlmkb.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3hcjfrisd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3huqrzsmz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ghfvddud.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rdsqlobd.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3moqidsqj.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3yxdwhdrv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3wcoaovyx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3obyajcvl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3mcliovif.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3osmnryvs.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3iwgdqycd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3qjqymabu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbcsuaov.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3leowocdf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3eimsrady.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3asayayey.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yleyqrzo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3yheivbpl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3gkgyqane.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3csdkrbhk.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bmkhttcy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rbckczlu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cskciewl.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wczagjes.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3porujqgs.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3qxvkzbua.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3xvoiiefx.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3tztpitax.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3jhkywxwl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lptnzxiw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dsksnevb.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yonnxwnl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cifulgqc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rqcjdekq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3aygzmrwu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3htzucmfv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3goustkqm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3qliigdqx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3uiytpxkt.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3omgykcwr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rzdrpdhd.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wmqssrfo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3vkmjhobm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3yrxgfzys.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3mwlwwpbu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3nfmcsesl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3lvmlgjtk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3jcpxowfd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cbvekzbk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vhgctqoe.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3osggyxfb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3tgrwpcuc.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3nphgpjgu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3kdydkrsr.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3exmqmhsb.html


<!-- 参考信息 -->