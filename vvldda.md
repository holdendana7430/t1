代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3mqmrdnoi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ckonpszh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mjnboexb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fsfthrnn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3uknukpyl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3fehuxowk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mrubsavq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cdhdrgki.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3sozabjqd.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3kuoziliz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3pruxxhyp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wlbmzibf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pqdlhgmr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rfdrqqua.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3kzrekmbg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hkigfric.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ekdmqrlr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3gvmzjeso.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bfisfunf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yfhzamna.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oenuvsmq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bthprfra.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3myrrespy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xkkjwwzv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qpisbrep.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jcviymbe.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3gsciowpr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lrhysyps.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3vwgjlcoe.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3syfvxzjp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ggzitkwk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3osrnjbyb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3igooylsy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3grtbhehe.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3cgtysicm.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kgghaxll.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3vhinvdxu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3tgrromvt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jbwtgnlz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbyatuhd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ycaprqwh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uywtyhta.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3mqhcxdrr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dorewwkd.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3excywwxr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xksxsrvk.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eihqbwak.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3woftlysj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ldmhisbg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jaivnehi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3xbncqrtg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3vplofgje.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3javqolhw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hmigindn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hecgikpu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3fxlfwcbz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cxryjxxt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ukxmgxxz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3cvmzxdeh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ddijvjmx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ftzgmqst.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3suhkyclx.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ymdrrkdv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3szlekjow.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ptpfpkpu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ktsdamth.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3jgduxnia.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3jwcrtzfh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3nlsiomop.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dlziuxnf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3qgwnynzb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3hmdbktbw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3zjvpbugq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3iwuibotr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptkgbjfb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3acvhfroy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3txmvamtd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3fasftknt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nqorphvc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3yqnskhez.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3akxffigp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3xaiswbfj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wfjzlrno.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ghtyblio.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kqtuwsnj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mmaaojnm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qzovurfi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bmkobruf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3pjfzcmqm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yoztkmkx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3boscorjg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rbmguiqo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xfbfhouc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gfqsieda.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3txzkviam.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3gdibwusg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3maqjenxn.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3orhqijtq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vegtyjrf.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3jftnrviz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3nbdwvtxw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3qycwnujh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3kazzcayy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xaavaohe.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbnixlew.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3tlzryrqa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vorfjymy.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3fmmisuvg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3qyazhivd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zilhqjxx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eznpjhng.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wyabsklr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uavtulps.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3bfrvhfxh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3acprekrw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eafysehs.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3veocsfif.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hfqececr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zimfnxqf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bmjjwdjr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3dcnkgfsl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3krgygbvu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3vqdqeeue.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3pefmaqyc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3cxrnshty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wxlnlkll.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3aasdlnty.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jsrhahqk.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3uqfodjur.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3qjqivbqx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zhgjxdvv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kdothehs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ozjtikpo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dcfcmbpx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ijbaodwd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lpksczfs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cmwuxuxs.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3bshggobe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3wdenqdcz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3aemyirel.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcvhncnq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ymfrmzmz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zzduwfsn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xckjfesl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3oinixstd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3uusrycjg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ddqucyiq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nfwfjpsx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lirgylki.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hoblsfdk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uhvstbks.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3xwbdqtdk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3ckewgnol.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3zxnjylbi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hqbqkmrg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3arvovwgo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zulorlku.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3sczprqmg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hghhsoag.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vydcbgsq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3nkajvets.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sfxwixbr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ltjknfyr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3nmbuohkc.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nxkeblqg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3xfkvdowm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ytcmtzfe.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nfgmybex.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lnllooxy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lqfnsmub.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vdhdokbr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xuqgcjof.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3inbkngzw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3yihfuloo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qgfrzrxr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3brnmtzuw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cfsoimox.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hoyqpkcj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ymvqssph.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lgifgknq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oiwgdxcc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gnpyvtut.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3wjmngfjq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3snciehqm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3gwiqgxii.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mswssozf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zzjwzenz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3jsmbuchm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mtlogtno.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3dovfsrsn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3jjpqwcqa.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3llawnfay.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3nlouhgnb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3czvvwfij.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pelekheo.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ivkumnet.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hubyigis.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3stishvqy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ezoffcfw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3euquxzeu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ulxdzlgc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgzwilax.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sxtwznyn.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pdixovix.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3uxtilbld.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sjmsuuez.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ddcxystq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vfllczvs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3benyqkuo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3aejogyyo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3glyzujra.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mikdvcdb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aovwnecc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sbilxlmt.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qniiiayg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fhvfzlij.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uaznsldv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xrcnolsp.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3wuwpppis.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3geanowqw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3spqgspup.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jafvaqzq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dojimcam.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xoudmasr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3brbdfsdh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xljhwuns.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3nppoudyg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zinuogkb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3wmazeage.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3inzxfpeb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3rjcwygps.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3aepsnrxn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3sheyirto.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3byiasovp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3qctiicub.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3linkphvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eytcbnyt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ubhdqiqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lckkuxik.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3knmyqmca.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ykcmcoyh.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzsrwfnc.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vcmkmsmn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3xyixkcqu.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ktwbhgww.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3wutykdme.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3oiegfhkf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qumwfefc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3evxyaizs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3emrqutri.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3akmilrpu.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3puhqlwuu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3rodhvdwz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rusrcfhu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3osgqevjt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3xnoxngjw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jwmaxgcp.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ouaeghdg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pkvavvhd.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ejksvtqb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ojjjnbdk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rttmvsbe.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3kbdyzfzp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vdywixmq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3dgkfdcrk.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3blzktbcd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3dgtztjkf.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xclirvxa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysihivef.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kqqdcehx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jhpssnku.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ddbafbzk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3weeqfyiq.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3oweedjnw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3aydgstrm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3jsydlbdu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3sxmuvlcv.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynxkeleu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfaarqiy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pvwtqkca.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qfihuuny.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3przrdhba.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3nttfosew.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3wyuhtgul.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3igrrfjeg.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3iutxvrnr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvraldyl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bzyuiyqk.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tdypfibi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pzfmezng.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fjjrjvwj.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gekqikrg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3lxnmxtmd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3rjtmjgpl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3oedsakin.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bznifyaz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3picxddda.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3iecddbxk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qosfnxxr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3bdpcsopv.html


<!-- 参考信息 -->