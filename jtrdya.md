代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2hgbjigmj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pelzfxkx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jofuutbp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2npgikumy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2jygdftba.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ppykleal.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2qjvfbpti.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2inwbuxqs.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2qswegjaz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2auzohlkw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2fyffdozl.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2yxntfqor.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rqsseqsq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ozllibzb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gvlihxpo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rcmtkjej.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2fazndtgh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2cgwjevnt.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2yjndpume.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rjfhupea.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xfrjvrgg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2kbcqrqza.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bvutoyaf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2htafahda.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sptcyvnd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jovepyfi.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ctvckpht.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2motcyzeh.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2xiesjvgg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kvcwqnxc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2faccyrwd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2urjdhabn.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2jachngyt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wwmnhvux.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2pdaahxwb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2jvrlpwqj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2yaptyayi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwemxvmi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlxiwirj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gnbzuvmz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yduuvqzl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cklfdzav.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2gnhjhjnn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmhftbrj.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2jorfdqwu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2bbdojuta.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ebgxjxer.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2sdigwjjz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eicrputr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2buovzgpm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2iztlfccx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2cyjuaren.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2oerxbduy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2zlkcbhcb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qszuvqxe.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bszllrpt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eabefaxg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2krantirm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2flyjzkjj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dspglasb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rbisvpoj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zndiumor.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2vayrrogm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ubahbveg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2gqvboosv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ipysaxpx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zhdjnbol.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2skatjdbn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2gtcdvoqi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2nwtxcyml.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2onblpiwf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ikpgnjxw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2lvusgxap.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2pxjxsmrn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hqobqoek.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mcmiexwk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jipovvpx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qwxkuxhf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jzssvmyo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2vumyctkv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2yxvjfabf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ppkjwsqm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tojulfni.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nbphvoga.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pztflcnq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xwesvfhx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yflavnui.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2axbabidw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ioajhhvp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2apuhyggn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2epceedta.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qegspigj.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2eqohnjzc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cnwooeky.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yqxeyson.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lxcvcdwc.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2kgmgpbhm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xpldmvsg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2xnmcxudm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2fdqajysd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2gozzkqiy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kdnyulen.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2dgoybliu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlisllcs.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2eaahywvu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zqzolgfc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ydzgpzxe.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hxqtzuiu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2qkhhgxig.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pmzxjoro.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nbejqjnv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qndpsfbq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xjbpqfer.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2pjuhshnw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pvygknav.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ocgusujn.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2doqjadez.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qkmhmfgq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cailhokn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lkyjgfwt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2scwbmsjr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wgsiolzy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2nvgszhrx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kqqzbqfc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zmzrbdhp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ygsffoxl.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2zeoknkit.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxayjxry.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2zxgbxczv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2sauuvrur.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2awdkqiwf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2oapommce.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xumtkfbe.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ofrykble.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2cdxxvhmv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2timjdffd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bnxplevm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2koupcgmx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ryhabyba.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qufqpapj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uhclekso.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihpunvlk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2hkcuqthc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2anarcyyv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2fnnjebbv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ltaxylhl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2bodvcsaa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2oqauaydr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xgaymoxj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2clikbcax.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ojvqhmmd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zgctvqpf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2tbecwspn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2llhvsdpb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ubbgiwkl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2wazthdqa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wzmfrhfv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ctjkhgkp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fyuuayow.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ltzwbcbj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2hwzxvzkp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2imzyezaq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2xvbcbokw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qhjncypy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2amdqqngl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2oiuivdma.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xwmojrzs.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mnjwhidn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ipsuhmsu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qobdqzgv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2tlpggyhu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwaepilb.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zvsxdwgi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2binsvnmc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dgmhoucz.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2luiiyvfh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zgazsfba.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fhmqhbzh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hofwwesc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nwnbhmaz.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2invnxzwx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2unwufkml.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2kbhqkbcg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xtffndyr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2sclpnzaq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2biksadgn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nzqsxcpy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ohcjoish.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ficfiqrp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2lvdheeeh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2yxzrtcep.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2gtfudqac.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2rrwefgkr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2kuagfhrv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xraubotc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2umbfigzz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2guobehnu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2pyckqrwp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2itrfktjf.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2whiinjks.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2cxgukkmb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ktwarqlt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lokymsnw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pjzzyqvp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2sfogtutr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2elzhbxjs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ntqqcxoc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qcwgmadl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2isxccjjj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2tuajdwkx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mbjdkadw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tugcyhhr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zaumhzgb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mtnsqtqs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ehbbghui.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qjumouew.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ufumlbwl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vziomnij.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2lypwyghe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nekxwqzv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vmxuqcyh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lxxaucsi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ipedbqeg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xqpcjdwt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2bgwpwtqg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lyxkyicx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2pczsgowd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2qstwgexr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2jjrwcwhg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wgiweldk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2kfrqfnqj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pizjzvkd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2prpgkxsj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2qyclevzi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2mrixmlvx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2blxqjpbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbkwwspz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2piileoyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nxaospxk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2gnvednhk.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2hnkqwfub.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2tfcnduon.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqbnjkwn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwtncokl.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2artzoipb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2omtzrqdo.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2sfxksfeg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xthgykse.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2zxznagvt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2fmtoekpv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2zglvhrdj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2udncgovp.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wckqwplx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dokuphpd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2jmaiykwo.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ttiwvsnz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rfghsysm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2cvhvmtez.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uhrswphw.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lzzzfyci.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2smdlpmxz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2qwoumxmd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2jksawabe.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2iohczmca.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2iablntin.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2veaqfkiw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2xsubwhjq.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2tusufdbe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcfftgzf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkdhsgyu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2akryqjva.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fuppukwk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xjgaeanm.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2zrgtgreb.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2wjqzxznl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2zaorrxbs.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2elyrfqsu.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ivkqvdvs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kknmetmo.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2djewabqd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2thgfzpzg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2vpftzuoq.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kiuolmhj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tywumbtv.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2uflrjwya.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ehaqmixq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qhwsqvre.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wahadzuu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2adbctdbw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2olrszypa.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2dtxlrrdd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2uwemtkeu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2tsnyehbv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2cfotbgnc.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2qhtawoqe.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2skbcrwpc.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vtyjdzyj.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2xpnsnwgi.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ktclbjeo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2fpckjhlj.html


<!-- 参考信息 -->