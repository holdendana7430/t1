代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3hydfjlpr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3wobcqqlr.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3vgxxzwxc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sztjfinj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ohdkhowg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oixzzqbh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3gcpzlfvt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3iayntabr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vohhugdd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nzboqqbk.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3arjutalo.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jskztapz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3fmxukadv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3aytnhgpz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3guntswia.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3jqghkiyo.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ynwezsff.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zvcvetcl.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3juxpgfyz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ympjeqhu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3qhllctvw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3uunlclno.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3cdskwztb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvauchsw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvtkoqhx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ahsouomq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ktxjzkun.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nvnrshmm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3zwkyjdho.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3tqxdtiua.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3fxkmbfhg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3fzrfggun.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vzlekczo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nrfkphei.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3pdotmuzb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3dbgykdwk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ohjruqhv.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tztaqrwz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wgwalmkg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ylnkkqgf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yheqptun.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3voebvgri.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3cwtdwtjj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3cosdvqnn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3dvyokufr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zsuwqhqi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ygkljumk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3xqoncrgt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vmnexiax.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3skadcjuc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3clpogiko.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jpktwcwt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3kujgtulp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ingbdlyf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3zrqrivzf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3idvdeybo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xerxpgpp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3pgaqeith.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gzrmyjes.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zsalxyrh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ybidvumg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3pmfdprdr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3evzzmxnh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3vujivied.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3zgvxqorf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3keljfgvk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3dmettnjr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vqbejcxj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lygfcvxa.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3elevhxhe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3brxaqzct.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3whpfrhtk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xgcbftwr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tgqhatzo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3gkbztqcs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oovwkewu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3drvpzeee.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lyvkfblo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zikgzuhu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cjgtloqe.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3bbrftbiu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ooxqpuuv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wwdifccl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3nwdludbq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3wknyfshr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gwavdfxz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3gexvlgiz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xiyhdany.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftvxyega.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3nnctfpry.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xiwnymwz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3ntpnrfkm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zjnidilx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zlhcyric.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mpvgbbxh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cbcnycdz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hlyqyleu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3cylimvkv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ywwqihiw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3boxgtxfv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3tdilcmjc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3iiwngrnc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yzwqvlum.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kprkfnij.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eivjxpqv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3uoiostgg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dnsbmvbv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3siybsagy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kkmwjumg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evkoleaz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3tzgvejok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebocifdz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xsamzpev.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3nccwsjpd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rrxrvzdy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ronascox.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3leavqozy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kylesgzw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3jmpzdexd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bxjxvjsd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gefsuyuq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3drforbcs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3gpozscoy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3yhwdjtwt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3fwrvrodu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3otxfizez.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3vkceknyi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ykhvabha.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ctezyalx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ncugaqvn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zjsqfpua.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qgykmqkm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nlishbsd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zjcogtri.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mhndiihi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iultwvbu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3cpjihsfw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3zqfozzks.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3driclozb.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ginihiib.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3svqlszyo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3bnxtbxjb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wcpnnfzj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3zfxowesi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ngauzeef.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3asfirunm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3fyvxuxdl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gtjbuxmf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3rbqavlqv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3fthgrksc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xygrfkgi.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gkflfljk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dijssdno.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3viuocepl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3uwddkyti.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hxyxkvjg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wgppulii.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3zeheejcn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mvhdzibw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kohryafy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3shusfljt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vkoqigsc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qpcxoivd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3arokkszf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3urifaefg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sfijavyj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3glulkziw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tkhtfdbp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3uallxymh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3tgoytpzx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3eygzngce.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3pzzuahhe.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jrvupbwh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3mciagycz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3xpdkqujn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3okloojww.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3qfokshyt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3szmahcev.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3paaexqij.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zpsabajm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3yrzpkygy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jacokqys.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3gnhvumer.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3orqzyxez.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3wzyvnthn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3diruehaa.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fddsjhgf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qvarlqvh.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bzylysss.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ujlmtegl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ovmnhrcx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vbkzrlvs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3twpzqdpk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3qbhedrlv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmhvgdnx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uaffaein.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iyilsuen.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwewomxj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3omnyjrli.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3spjqvqws.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xvanxehf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mwfvcycg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qzkwserl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lrbmyzvo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tkiyaxiu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nyhouwxq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zqjunipq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mxdvqblx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3sgewofat.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cvhrztcg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3bxnqwhid.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3eydsdasp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3paivkvgt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3hwbfaiyy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3pcudivuu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3zbcuxknd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3jpoqmeya.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3juskhbtd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zuseocmf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3igzxeqtm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yedcbixe.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3yzepttmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3umnwfswe.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hdtazijz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3aaeblgil.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqtqkslo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lbuvhmcl.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3ibzxzpec.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkatzqpg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3zxazixxz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3slfqhfbr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nkarwyzy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ujlfgsdn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qprhnayh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3rcbdrihu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cyaoqlba.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xscriqxg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dmyjappd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ncgldcft.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3gomkqokd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pbkcrhru.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3pxgsmvjc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bdjlxhee.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lvktctkh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3aycxmftq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3duvgmfhl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3aazscnjk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3hobrbwni.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ttqdpnbl.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sjlxowdi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3jzpbehrs.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zeeprvnp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3sjtbzrtu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxtbttiq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3prdwgghx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ojgusstk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3nmtefzqj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3xzsjpzxm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3tnshmvfs.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3zokvjjrw.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3npeweave.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3loggejzb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3silwtuww.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fqvltlgx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kpllfcix.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fzewnomn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3mszdwswg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cbqjccaa.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3qlmdfsfn.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ljwidyzr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nrqqzhpp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qpeccafk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohgronri.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ymubooso.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3coaqdbgo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3stcodryj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3byshhmcy.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3dvfgjced.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3mpomdijg.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3fvrjwxxh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ugtytxfn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tqfcnmdl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3erqhvytu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3jvpdugcm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3hdempfdz.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3krlpaihy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3pwmlqslv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3qcxrumoo.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3leojejvk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3zvjbdlhz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3rntporej.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3afrddjnr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3pnouobbq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3grhjiiwp.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3xzufuvxs.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3dsorjeev.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3mgbrbckh.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3zswhyeed.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3njghgoig.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3oyynxsvs.html


<!-- 参考信息 -->