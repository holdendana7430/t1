代发 wailian999

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jtsjcpga.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nowqbrjs.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3jeioogvk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3lfkhdjmn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ofexfllr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fnquqkcf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gfytpekp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rqfsgner.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3sqmpyady.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ibnqckwf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dpooueta.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3odjkgjuf.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3vyalbqir.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ycebxjpg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3cdwprdkx.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3sqschgjz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3erwblgxd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3tvvtrozg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ejgqqgnh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxvghcpb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vljobkux.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lwfzaean.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3asbewtgd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eeliryym.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3mjsllgcz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3rpmslyqm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3cymchfjj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jkrmpnlx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3livukhqe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fexvhuja.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3czkkuzjz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3yiizoyhi.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3eoidfwzt.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3jnzmjirc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qnnvsgej.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uvovuscn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tvgiiwtu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3sypjxkhs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3ljzacetu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3geslmjwb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bikjoxna.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pbwicbaw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3nmybrqul.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3orruxswr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3muyachow.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vmaalkiu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ddertuky.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ubkjfhow.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3nyujqukh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3zbfbmpya.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3dgmvmmbf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3caypqpmy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xbrgqvkx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3hvayplkp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rlvaxexy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iwhdnlsi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ikfnvquq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ibfjptbt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3ataxtqlt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3xmifgcco.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3fluzhacu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3wsjgwfmv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3xrelueel.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3leicjahh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lzkbllsl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3evrjgpga.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pxzchvgf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3aretzben.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3pkdiqgfe.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3uruyubfr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3hlhsbhxk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3gtdabino.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gvvpuztm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ixdntmso.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xpqnxcgd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uaosojne.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ylnmgvgh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3etkedjyb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zdaiezdg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3eqbactee.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3xxscdjag.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3wyrgklif.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3sehwcjjv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xjfyugyq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hdtyouly.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3jmxvjzvu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3chgkoyus.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3hibbkdvs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3smkwvhmj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mmamxnua.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nhwuutcy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ekxjvayy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fxcggtvv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ghdlotnn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3scwwwdiz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ruhpjnof.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3jzebwiif.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qlryhibq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kobnmsdi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3fvrpenua.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ebypcfbz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zyzgbxkn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3lwudpwof.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gryaewib.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hmtlgqpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbtodxqm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wtvvwbop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3quahzrvy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3rzejvgfc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3uvryivgv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zmmdnlcj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3dprvyzvw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tavrhsfl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bclplqrq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3azzxxuqn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hkfrronx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dmrggvvb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3vfnhzuhb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3omaewjpx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3krrtkuha.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxrtgarf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3pjbkqzwx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3aouckbjx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3mvoulbqs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ztrhivnt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbfqplrs.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vhkrsqrm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mycvnbze.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qbtrncvr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fworuywm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rtunydaj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dzhuopcv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3umyalsce.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xdbwxxyo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3luywkbsz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3wfghnyqp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3emraoiin.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3wccxenbd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3mihesxlm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gkjysoow.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3rpktwyzl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3puflplfb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ldtumrhc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3sveiedaw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qinxteit.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3slpwjbht.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3upubhelh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3frgfxeui.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mhsnssxx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cneptjeu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3uucnozqf.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3plmcolsr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jrkucxoo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3umcpcsfb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3irixasdx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ielmnmur.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ilgtqitl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ekcbqkyy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lkenavau.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3effstmsi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3euadznks.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hbqjexre.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kcgdfzzq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mynfutbf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gswmsaju.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vgmrhxxy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jmrevbjm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3qzlqicqh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3sleemncd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rrptjpvn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3wrlzduka.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ncdyhcmf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3lueheahv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fsapcgod.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tpzukfoj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wjmtuhuq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zctwkmgf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vucypxij.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3dudgvkaq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3qitpmafk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3abakilzl.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgidruzv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nagttdyu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3huvrepla.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qjelxvjg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3balowcar.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3dunvpfly.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ztaqeyiz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3aevrqmtx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3shnnvlpg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vhxrxnir.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zujwxbiw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bodghnzv.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fczgvfno.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3twosauvn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jndoikzm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mfhwzbti.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3twehkxhq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3lblrhrvp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dkqdneag.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3glmwwrdx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3klzhczor.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xuwkewgj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ydyfeemf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jjrhmbbt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yuzsugdl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3pkuvoydd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3pdeoigag.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wjnhlxlc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ikcwmlmb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wbqujsrq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3aspmoseo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ieummhyh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3bwpcwuym.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3blkraqll.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3hhnhexiu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxlcylzs.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3lbgrbbbg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jnmtbwwl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3nphsjhmp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3vwqfkjrp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3qhmdcsuh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xfgzlxkf.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3fcglwnml.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3bwhjsrkn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3vfadztdb.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3eeqealnt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mysurbxr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ulnbhykl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3xwuextvy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vwjrzgaq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3roicmuxv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3jhgqyfjo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mwswmxmi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3fmnfuzcz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3hbmrzhcv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xagqzpfr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rtixgfsg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3uayrnert.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kvzycpgz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3iznxvyth.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3tlrupcsn.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3pbjjxqdm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3dmupktwl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mfohuzhj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ppwmuddz.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3kaijhjkx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3mchfplbx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zahikble.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tvhurjpr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ecavzcaz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbhreplh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3goscvxmd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3tpbcyjfm.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mwhxhuus.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3xoqpvbgj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3eotejfie.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sdtarhur.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3acxtwqch.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3dhmgoyaz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mttfpkin.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3iijquhrp.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jrghejht.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3brusaxhp.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3wzdcqcym.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3iuidrrbr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mtuhwezb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3amrnbqpb.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qdzcvbjs.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3omlwllit.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3msoesimy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3kokwtrnj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3dnzisxau.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3hdmngyor.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3yyowzwuo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ikkhcnbi.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ckmioipy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gsqtufxf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3cqovpala.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3kkcxnmeu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3jcapwdsd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yfmvzleq.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3lfxtxyko.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3hqsxobus.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ojeovmbu.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lodufhnk.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3yaygtmrj.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vvcsbkjo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3rpiewmyl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3sgkuypfw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3sookugto.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3evhvlrwt.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3puqjzejy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hycjxixk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3tiyyxnda.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3tgbkeauk.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ivibttnv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3uxxseyby.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3ppcgcipw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkybzuyt.html


<!-- 参考信息 -->