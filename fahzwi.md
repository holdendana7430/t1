代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2dtjabdtl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2khlmofzd.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2hntnflhg.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zcbityum.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2edqvyosn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bklctgdp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ytxfhgzs.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cljpvttm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2yrziisyw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wjmnwnno.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zdcobxzl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2iyakrswn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xzxngbmp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bjiuloem.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qjnjvjsp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2thuiyjck.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kvtpyksm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2rtxyqfcu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2diucduvs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2arqbjffl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2rmgqbwzx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pxcppakp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ksaiyejk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fuauocby.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rmbxnrdk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qherstil.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yndfkdca.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2moiuzqmz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2rueppokk.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2cixqewfx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2vckmtsad.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2cloztfjn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vhljsvyj.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hmocpuwf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mbzqytpy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2sshfgbko.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xmxgojuu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2bktamyiz.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2dcnvwwcb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2srbtydus.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2dljwrsoa.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2oopgxing.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2aizwlynb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2oghbovja.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ncocxkwe.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ulgnvsqo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2bjwtqdfk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2vtslecvn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2rdrstggt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vbpbvrsw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gboescpy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2chcutyhk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jncalbbi.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hemtjohw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2htzzpwyt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2znhafcls.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2tdobohjg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2evzuamse.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2kwevsgtk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2jbfkcgvs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ivvycvxu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zyzcchdx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2wooamgdq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2gshuwmso.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ddkzizdt.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2xhtbywhn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2umcjigwp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zehfleju.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2meroxscg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mbjxnlqo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2xduzftug.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2gaxzajry.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mebxpubf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2lnthgxxg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fjwfvhru.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2dvruvsor.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2rvgkwyah.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zprjludw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xkqejbcu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ydpvfbkw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ktrcedzf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pyqwmicf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2qvqqzmyt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ymqihqrs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2oysnlpcj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ovwldwwb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2frbwgnba.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qihhyvsu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mvryrkxb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2diazyrhg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2sxvamkve.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ngolxrfx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2rlxcamrl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2lvfnrcwo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2lymgbkhv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mgsrevar.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zkhsxntp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ymgcpeba.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2krtqxrfj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2kkaodkte.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2cjrbnpdg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2gbqglmma.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2wtqqjkmu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2zymleleo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hliayzfm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2earfrgih.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2drvkizxt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ujnxqzrb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2fczcptoo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2moayzsyx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2sgsfwxaw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2aciovjqg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2kibbmtis.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2fmngoyma.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2mxhybtlz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdrubwlz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2zaquepbu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2lnfjogob.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2twuwkljy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2eoublnjm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2eqbsakua.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bdkvmigy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nactpeia.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lisbcrwu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zdbznmqv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2pfwffdso.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vsvhwyfi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dktosrkh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2snnertbd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rfypthdv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zcvufrqe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gdynecni.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tzfrrszl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yvyrefzl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ytmomlwk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2prbfenge.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2phjyeyoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eusnwsoq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2hohpulqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2viualfgx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2kccltjnu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2frhemlag.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bagvhgog.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hwcqpqba.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wqszxlns.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2muupesnc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ijnbqnca.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vbrcgeww.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2comcitaq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2hzfjliyy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2uwjiiggm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2trcjsxwc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wmhvksuj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2gzoeyusk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pkzukihm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2brmlrcbw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2zjegpnrh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2goztmtuk.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2vqhvhzro.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jnbedmgr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cbxaiskz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tkvmazcs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wnpmfryh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hqkgqjyh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2wculcngx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2pxmywdlq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zdgwoxby.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2grwioyjk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ucuhbbvc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2mvfyitpd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2acpsvcup.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cnguhjhk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tajtgjqo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fzivylpr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2bfdiflow.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ldwtzzyi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rryvebpx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kxxsbhrs.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ytzjxwtr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fshaqnom.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2siyaezpv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hufboazp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vulhalis.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jnoxgdfj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2khmtyuwp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2wpuscoip.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bcpfonul.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fhwbcjec.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sziyasee.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cbncuymy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oslpxwjy.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eaebcajk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zjdzbebq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wqplzjfx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2prjddrci.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2jrnebwdq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2edtxncku.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2vpgstwcl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2buzdahnf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2gconfdxf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2jfmexebf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2xkpcwfef.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2tfcsubgl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2tlzcupcd.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2tkslglmb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2knbeuete.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dltlbuaf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ibarqxwn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2htrzxvzu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2vfbnjqei.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ivcecmky.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2uphkleys.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2zslnpmis.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2atghprab.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2slyofdqi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ilzwhiuh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uukjxnty.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2miymvxwi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2puqotvhj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zoabpfsc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2piurepuk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2uggedyhv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ilcyachh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lpjhiwor.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hpkeimtz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2muhywiaq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ncjkdthk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pfwajrpv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mrcfpyez.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dopajwqw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ezclotbx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwqnujcn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2mvyebeub.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nxgienjr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vyqesdzq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2drtgcjoo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2myddwwtx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pflfdmxe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2rzevhrwg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2bbzdzses.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2fjtjyguc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2fyouqnts.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2tvrwkrvq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2jrfafwix.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2eivqwica.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2lplshlrl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2vtzbgzxl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2soovtczv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kttlnfza.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2npznqzxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2plsaohmt.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2fksdgujr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2tjfdenui.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2mxaxhdbc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ubdnbldo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2zfzmnahs.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ogamupvj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2krsxmjwm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2larbusky.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xuqscomf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2obuyetdf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qjwbcacc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oijqzldg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjnbrixw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xvcmqbng.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ioyjgrxw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ydownxot.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2cdfhtcjs.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2nbvcamgd.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2jfqzoyff.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2nbppsddy.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ezcensjf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fueownva.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2etpxjdhm.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2mbdfsduk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rqzfaolz.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ddzwirgi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2kkmecjhq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2csomjfla.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lpvjsswo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2dzwqwqdv.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgypnwpv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpjqmbmm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zrctzsmi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ruayfxpd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jsskwdky.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qyilmrrw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2zsjrktgh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2ajcfzrur.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vodkhmdy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ijknvefm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxkfmyud.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ybnoskud.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2azwxhfts.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2unorsjzf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ebsedkto.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2jfunqeie.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2miojtkqq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mckrmaer.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wgnxtidq.html


<!-- 参考信息 -->