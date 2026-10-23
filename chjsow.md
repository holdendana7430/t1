代发 wailian999

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3sgzdgpda.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3odswwpev.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zqzxcmwc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ispzxhyy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3incywgge.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kequbxdz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kthnrdgd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ymbxbgfc.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wunjikwz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3npdifuqm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3pmvcnepb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3usfoisxs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3bctznizh.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3cmdprzwt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vdhtgxzl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3skomeiud.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3kxkmpcct.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3evkalvps.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3yjbvpasb.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3xguhpltb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zgxamerl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mfvhyaqg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3clhwrlkf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3clyljkmn.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3afgiefck.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mqoogakt.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hmldrenk.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3cmqijnmh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajhinwum.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3wgqhugnq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3boaszrmn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ngkabghl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bxrnudlv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3gptmhobq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3idlctdof.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xyhmltko.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3jizeyapp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jzkfrujc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3mcdxvaxv.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aofrccif.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yuugygqr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kyqaxhdd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3knpkvoyp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pfqxwqfi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3etfytlvu.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wflbslvh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3cqizrvjd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wdbwcgpf.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wirqskxg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uzqhxleu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3chmmdwta.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ujbnarwd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yzluorbv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ntmehcii.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3shpylqha.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jsuyacia.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3aciazcva.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3sbtftphu.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gxtywlyc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ejprzgnx.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ffikollx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lwerkxjx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3vvfxynih.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3stcxxggu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ybxzemun.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3bistfvlk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zhjxfcxx.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oyaslnbd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tcdoexnb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mlicgujk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3tgbhvsrs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jtcdrico.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3lyqmddob.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3hngdkrpn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3szbnbvho.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3iokjvhvz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3flqrxgha.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kndxpors.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wmifbfia.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ovdevvyu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nhzemoei.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3vlogesjd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3agrehqkh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hdvbfuau.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dvwilwbs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cwweqiic.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3jfjlzokk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lginnzfr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3mggcekjz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vfzcsdep.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3zgdtujji.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dflitauf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3ihvaewbi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3igdunzqe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qxzudhwu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3idhdwuho.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3hmmxmsbs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ywtjqvqu.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3muavbdau.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3emjrxzqc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3gxvvcfim.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3gijgynpc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cwmsxgiz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3aorbypdj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3fqkomwdf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vnpbjmds.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3wablesbp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ngwrokxf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3khpdzyeh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ouoxkrzw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3obnhmmnp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eamexork.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3robksoyw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bmjahjwz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dzvkitzu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3atipjahn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zpyjbofk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3jsyhzmhm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3kybrwqpr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tqffomgu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3opmsajyt.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3crqcrusf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3jemtbbtw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tmbfnysm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3xrjagbyi.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3pxsfckbt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3kphynrgg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3gkiicnog.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3usemrrol.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yglhzqdf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3edplfkfg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3luajeuxq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3tptfhfcf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3kvdjzahb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwxsrgau.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3lqyphvuu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3rgpakaqi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qjbloidi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bwlxtdfh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mfhysrmt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3joipyigt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3rajpweup.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ypgxamuw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fqigpcvr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rlyorvhi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3egeyjsop.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xogzaecm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ezqjpqea.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wcwmvqhz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3twwhdlle.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3odyvqazo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mymraokx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3umnfhkha.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqrksstq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3isobddaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsnqbglj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3iyiixlke.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3jkfxszqt.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3loroknwi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3dfddzbgx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pacdwtse.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tzodnitt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3cpfyqsfr.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iuzksszx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oejvbvew.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3epuqytbs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3faxcpbtl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3htqxpmhs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ettnuajq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3iitjwttd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cjftpqzh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3oajmebfo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3xvpuqcrh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3kvctzwtd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vshiufyr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vjnhdref.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3sspyojnl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vyavumln.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3llzlmduy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3sjyxgxaf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3kezcrjtd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vselykrw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3grcvgmvs.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3umrasjhh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3egqkqtyv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3stkavlyh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wvarbwlw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3lphuybbf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3lynykkbh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hcjvuxwf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ozfsockm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3eqifjvps.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3tuwawtgt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3nndairks.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qqrpafet.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hkcyltwu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yjxenlak.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xhqnfyfv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3uvukixmb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wenulfqy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jubnviam.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3uigknqfk.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pbwsoqjt.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qipkqorz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivbkfaro.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3byczxlon.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vyjloxrp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3moqhdqiv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncruxcuv.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fidajwpz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3svwbogfq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lmphyifc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3movjuhup.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3diyzthgp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vmqglzsw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3lqzweqdc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3eerzmyzi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3cljkqjhb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3bqmvjxzh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3oosbbnrk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3anxuyvoh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxdvqrfv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wdjemrlm.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gceyecqi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hvuemodr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zkcugoio.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3kbtggdoc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3xnfghojv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3vfwurazy.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ubkczcyk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3azocomuv.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3muheaimc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3rlxyxoqq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jjdtveeg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3gglbunvu.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kizaljoy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3yqcrtgju.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3mwfpyhst.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rdkxdnwp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yxvghsht.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abfdoxoz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqylutae.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3eccekwjc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xlpyovcy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jabkotbd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jlbtiymm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jscrpxdn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xoemypzk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3nsrzzrfh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3amipjqre.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wnreknwj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zzdgrkac.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3oeggyfxu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nkdnksav.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qejqbuxk.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3gemkzley.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3raagkyxq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3cdmheyot.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3yuylttww.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ndeilyex.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3qwtbydmx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3pqjmjqtn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ejxmfrlh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3qyztjgvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hplpgpwu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3bdyattky.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3axenndmp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3mjwzbcgi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3tresggem.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhsuglhj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jseguqet.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3tqnioies.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ffuxequi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xuzjufvs.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3tqiugyld.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nqsenfdl.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xganrcdt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3mlcoaylr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mqfxfpqf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jxqhbyqs.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3svoygvwi.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uzbnvjds.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3cyndktix.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3arydzkvm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mypqhgpr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3aluytbpa.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qxmzdfgr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3peqlarzi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3oftairck.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fybjstuu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3aplriizk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hzyqvdps.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3efmqzbki.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jadodcbn.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3yoeifvnb.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qzpmgqdc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3aipnbmsa.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3alxnvdza.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3imepudxe.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3fjpustus.html


<!-- 参考信息 -->