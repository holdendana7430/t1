代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ajeivces.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3izpvuvea.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tkxezknu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3avmbjnhb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3unalkcsn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fmhjquyw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3cajvwelf.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3mpnmkfsf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pwaosrpc.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yvhacekq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nvlfrvsg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ynkmhbkh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ifyveaac.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3njqkvhdu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3whsmzbud.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ulnkwnrz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3eytlcybj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zdqpgvqa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mvilyndu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ieapbhbb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3nrrsyatc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3puswraue.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3pfsbwlny.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lywwhvrh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3vfgpkxgx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xeymeqnk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nbuutojf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3utadvghz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ljjrwjxt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3olqzsjow.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3kjawfhyn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hpszxdgd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jgbwnhvs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlxpyfnm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgitlltp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dzskmzdq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3imomdqtq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3mkfsgnao.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3alnnyzwl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xmhreeds.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3joblfbub.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3gvmdskou.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dgmddbgb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3agswiwsf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3euxudwsq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hdnhjdwy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3pjnyqsrm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3rhmqzuwm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3quqewqpq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3ylwrfuct.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ykdpzfpb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jkijiklm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gavhzvjs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jxbjazqk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3uoksfnoe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcimyull.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fchxbjna.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ugpefxgd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xdkvimwt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3thglwaet.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3pjpderyl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3huljcefu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kmqdirgs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3mgzfqykg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3fszrfbse.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jtpuzpud.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3qcybqnnj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ruqxdcdo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3tfcibqox.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lxtzfvgs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dltjkibp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nbbtrcjh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3bwfmupym.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3njyiwudw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3unyylhra.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3fmbqsuul.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3fqztxurt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vhimiuuz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3nddknlel.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hesfukjc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fmehayni.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dkiklchi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zivhfwon.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3miwyizjz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kkpdgoyb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ilcbzuek.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ydeslvdf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rixpdgnu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dfjrltdz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ychbkdbn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xgampjld.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cljloapp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3kampeyll.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3jnsecqcv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3yaosovsp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qygzhfup.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ywkofbov.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3crqhgqgl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ybeltzle.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3hlcyyzqb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zzuikdrf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3qxwretvh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3okdvgvri.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3vznnnubc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3dcvsgrxj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wgzapdju.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rmrynmhm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qteiqooq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3edmodogp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3xcieozty.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gfqzlfwz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ghyioklh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3pcmrccok.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ddwzzkmr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lhfeqjxi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wbjakdef.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3yxfkzwsd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tfhcsrqt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3lqcqllvg.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3oolznvlk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ecuuscuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebimlewu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3kqhxdecg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zulqhljp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fjiyvgww.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3equawwwh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ygvpukte.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3febyqcpt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zvrnisyy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ieozdoxs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3kdpsbpef.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3chplfxdc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jurkcuve.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3sfjapjga.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xafhfzlm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3kgqvsbqj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ydxdtbto.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3skfxkjmb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3bvivhxhn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qkedhqvb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3tkxawcdo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3kdwcgiug.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zurvifbp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qfizmuzn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mfpqnkfm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ixllxbbj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hruytuvi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3khengcqf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3leryqlrz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3olcldnuy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ufrqmfnh.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hgmbdetf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wekkqura.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3gwyssprt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wfmzyipf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kqpfpmjw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3deopjhnl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3vlseqayb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ifaghuba.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3srftqshf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3clzchwwv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3dzsynrka.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gywdqvka.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ulkshwty.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xucvnzdu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zezhshkd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3rwxtzrjz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uhojeebs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3scqmsyxy.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3apwbbwrj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mxdpfnbh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dkaifait.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zxdhebbh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pvwcbltr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cdcwxbfl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eqxtodrk.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sdbyrjax.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3heffrjvt.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rbhmxobi.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rkurqxno.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3kwyusjqm.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pzmqaawg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gnklfnde.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3flteiwbm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3oypirmwb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3oshatuei.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3uifvykwm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3gmkkuxwx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3bzzhzyqo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3gtweukcv.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gvhkxzpd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3sobmdzco.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3aereaawb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tchsidvn.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xmuxltfd.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3srhblvsv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ycfkgedg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cinuvxht.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3trrmxkog.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tsmgvslx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bhsttxav.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vqlexfun.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3jbooypaf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wcadeoab.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3przozpii.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3zvpmthqa.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3slucnjyi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jwfjcunt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wdbclyee.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tgkcodaw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ibyufwta.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gypwidyd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ptpqtmus.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mcbtdyyd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3nbhdflki.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwqtbdoi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3aapzyrjh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3umkrihpr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lreqrqhr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3eqyrhdpn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3erqoszhj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3utwrcaft.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3jecppcol.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ukkduyak.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qqalykyc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3lpjrcqfs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3nbwtctds.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3mxbskxra.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3nwtclnit.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3hlhidtox.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ytzfmwom.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3blimmzgl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nsskywvl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3evtwjdoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iklerfly.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3ikojzwyp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3jssdxmpe.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqkofotq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3chigytpg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3tdihwcan.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytchbypm.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3pecguyrc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3lyremcou.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xuqkzbpt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cnzodptj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3yajifevt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3eyzcknjb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wwkwlrhr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ermdszwk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3endfgocp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3yulcjcwc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ldxyuyvq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3niqcizzv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3wdmaohtt.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pdqbsyyg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3srzncfva.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3dynvbwol.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iicwwjbg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3mnhloeyn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3omatikhj.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3yyjrmzws.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3vcdnnlhm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3jhmcsbql.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ugucnzyg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3htoaoqvw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3coneuxmz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zazwoteh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hmhacsqa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qfdtahrr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pcigmzqv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3obalaivl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3sghcjvcy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3odupwjdn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogudbxvz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjtpwfll.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vvwjhybh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wcxvrmge.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3zspjvgnu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3nzqzvmqz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3mpyeaziq.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3zwjjzgeq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3feaqaelj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uaqebwnq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nbetqdoa.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qgelyqzt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ivcnbjqc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3uwsrmrby.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3aypgixin.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3btdupspu.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ynxzbcjq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3gagrxbmr.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wdszsnob.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mcezzzpm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zajxskme.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kyozsgda.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3iiqkgfdc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3kwxzffol.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3hcryvuvc.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3dfmieiqr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hqwlrapq.html


<!-- 参考信息 -->