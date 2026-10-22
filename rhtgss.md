代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2mybzrdhp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lajoytkr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hkzpctvg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2ingceqfb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tzpbglft.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2hdcuxskx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ryfdsfwi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ziinzaui.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2xqooejjx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2iraofwzw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jtbsqmmo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ynkjkypb.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2xcswybbv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rqajdruv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2iahdqreo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lzubmcii.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2bpzpycje.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rdrsyxhv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ahhkvryq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vlcbaajp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2vxeayxnl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wvdnzqsf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pfhdworz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2apajwsev.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tyvolycv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nukaemty.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2scnsjkfk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vgjgxfyk.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qasfjozr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rveyjxib.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2xdedqtun.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ndnmseny.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ajwuvjas.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gmuaeekr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kqldozec.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2owugykys.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2jfzsixnj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rxelnwqa.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2zkieynna.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2lnaesgay.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2wnkcccvq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zwtwvgim.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2idpqlkzi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ehlvdroo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2easdyghy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zcxuwufk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2anaamrxe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vmuupsow.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2fjpizslw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2tdgqbajt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2owyswdfw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hsgjryyt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2wogieisg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ybxambop.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2fiosnemb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2vwmltyxa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2psimoyfl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2giniwyqb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2dnlygpvq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vlpvegjj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kfwnifij.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ywjgnmst.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2rikjwuon.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2leksxwaq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2fhsmyuce.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pvtajwpg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2eiadtztk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qhdiumoh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2cruckkfy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ysmzuqrl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bmehatqm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2njxmzdac.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2eeywsjrm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wemlosww.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2zdezamzi.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2nuakklbh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2rcniricc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2uirawxpc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fwjoqxxm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mfdlzvoo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2dmafbghi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zwlqsyrt.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ndihosln.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2yfjusfem.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2fhxczgri.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2zajtxrrh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2vrxriect.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rneboggd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zlbceerh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wckryljc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jhhppyay.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2foboqpau.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2awyswtaz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2zxmwfgvr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2rpwgvfzp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2stqyadnf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ckkxvqhr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bhvpqcqi.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2yicirsbp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ktayzwfz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2oeuclkql.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ykdrrdbt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2kglduyik.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2cnbzxzgp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2pifclpqh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2tetqaifx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2zsknffxi.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2aqtrmrse.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2zhubqxqn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jdlacpuw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2mdteotpu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2hbbpucnq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2foplvstw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uqpekxxt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2huelsvly.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2etmynktg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jkwehmxf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2xdxjdgjw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nkhqsmle.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zvcpssua.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2nckyyrps.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2arjbwxmg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kgtepdgc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2huvjcwxc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uohlfbcm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2pqrjluhj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ksortczi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zxelnwcu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2soaymebj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2stgwllfb.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ciuikprz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2afjlxzoy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2nexofznf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2llsqbfuz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qvmrrauf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2xbasbddp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fznavfoy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sgptnyjm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2idtasbje.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2huvifuxm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vkzhdshm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wxmngfmf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2xigubuuq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2lwlzgzes.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2psaifytt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2pntubauo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2uapkilwd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2sqsftvhh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2iiccbgnf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2whjrrjex.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2xnjsspnr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2yltbdule.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2iemqmeqs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2klzbttzy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gqvlvmjo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zbghcdxi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2btkscppo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2upnefxmc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2teacbdjn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2bsirsvlq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vlupofbm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vrkmnrxm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pebsprqo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vdkxwkxn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2lqcbevhc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mxbfbokd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2udelsdcp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2oxadiigx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2omnmqmyw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2aghbfmap.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ydvqihfj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pwwfhchw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ljgynrqn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ldtwkeah.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2rjxqnqnm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mbohwscr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wuvezryh.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dijmyfor.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qntfbham.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iajkyfhc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhdoskuo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wcgsymzg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cqqomhoz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lroednln.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lwweipbg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2raqddfcd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2bmcfiigt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mraecgxl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2vzozqytb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2velxllru.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tgobzbto.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2uhoutbzl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2rrffgosy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2exbqzxgq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qquqvexq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2zjeroiww.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2vldyhecw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2uyfsnlmk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ocklnzsv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dvumhpjd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cjndsewk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qyppezyb.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2jmxceofz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2bqbjofju.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2zbxqndlu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2twryiyjh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xtepugus.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qxqtgusj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hfozmret.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hetsseok.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2eijtluqn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yqdzajgt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2fizfzerk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2iazbvkgo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yyobnipg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lskkyupz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ubqjhnjq.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axgpfylz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2joyzfcbm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2odhhllrv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xsbbjxbx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mryiulwm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2aqswfcwj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhfjwiur.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2slgargvl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rleehykd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2idoabfml.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2blpsumwh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zvtlhkgq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xfrdiafq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2mmpzxucq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fumqicqp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2uuwtgpby.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2mqytzfud.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2fsddpgfq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2oznhdpnr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2gugqyqmd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2mwuaibmo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2xcgwqhyf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2nchvydyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aefckkha.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2brlvsllm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdccbtup.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2lmjcyoex.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2iphmnmbg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vshasasz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ujxwwkmo.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbywzhla.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmsnokfa.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2gtfifshp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2sksqqtks.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tvsthhbr.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2scbkbzqm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2aszflhwv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfciuhge.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2odfuahwa.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nfvhuktw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2iopmvxwl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2buqjxove.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zufhnrjl.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqkakudb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2mglnklxl.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vxagyyfn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zzmgwajc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2shkoarnn.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mmcjchrh.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2bhlngibk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2wustosfh.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mhiufxrr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hpyegxbv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2rhjoudbn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wosgiold.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ogzlffka.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2cikxouui.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qegxulhq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpidevfd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2demevhzx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dfshkkhl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2jkzxgtbo.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2voqrswuo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2imcqcema.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2etjknxjk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2cmkghqyj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ydqzuvkj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfapxnvb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2sdjzxucd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2mittvqgu.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tgaoxtsd.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wshgsymc.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2zqodmfvr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnygqcvu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxkfapep.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghlqbrgu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zxgdorzx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2kgodjbqw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2fpidslpq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2wynmpuqr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qiyczkwf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2dtvblkyq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nuizmnpx.html


<!-- 参考信息 -->