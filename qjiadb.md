代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zajqlqkj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3wihjlmlx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wrsfipwc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3eljtjktb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ieadcncx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rqljlicd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3bistilqe.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tvdtkhdc.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rsewrvbh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3yvvduxjl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mgvchgvt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lbkwhmfe.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tiragigp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pztlsgqs.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3qqcwymdw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3eooqcqny.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zqtiwagp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3cpmayfbi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3oyucjesh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zwwsabcp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ltgupchp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3nwfvxyba.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3artmlvzd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3jemlqxps.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3nkgwzjxt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gfdzatax.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rngvbzod.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gvmtjkhy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3znkoeiur.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ugadiqhd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qxrprooq.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3dquykjiv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3nbejjtua.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rwaaeftm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kpncealm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rtmwaacq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3dscfhagj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ojzngjbr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zpfzbbqk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kunjfcjd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3wzvhomef.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rtxrzixc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3hasbntst.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3agindjvt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vreyojlg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ihpxjlpz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vrfhpazm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3kywkyqwv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3rmsqjzkg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3axhjxruq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3lfhtdquc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jzwfqvrp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lxdguvnf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3astqrlxj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3lrkwoxpb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bjwwpefk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sxzrhnma.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kbeleggn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dwtxxrzt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3krbgwynn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3uklizmuw.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gnsslcdp.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bjcdlefa.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3txsdjzzc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3okukfdbu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zzqnggis.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3cwhcujyn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3yvnfwepa.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3pfrbquso.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ioydutvx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xvzxcjuh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3waocfbgt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gueeiiof.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3wygdulls.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3woweysol.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kafntozs.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3aicoyoeg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ufdlwvhu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3finizlkm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3soxlllkz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nkvyjgrn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fdadehud.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gwhhcoxq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3zedbcnhl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qynjusdj.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3bdfkglcz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yzuvcoie.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3ujgmsnxq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nsralqvy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3mdfualab.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3dnydtgcq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3egbclgst.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jwygfxop.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zrimnfzi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3tjrspfxl.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3nvnscbbz.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3hweztxda.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lrvfbnjp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3sznsghon.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jzeneyvy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3vwehjzgs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3quaphedh.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qylqmwgy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3lpkzrjhu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ohhrdyrb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3puvfxrwr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hmoscprt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ozgcsxtr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nznfprvm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nrsvdlih.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3orxhfwgv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3vzagcpdv.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3nmzioxtp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3nccofzjn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3gehnlxpv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cwdlmooe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ntxiwxkc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qinuamvt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lkzyahyg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3xyzwgehj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3jvdfsiel.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3fitfsbkl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ffajvdbl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hrkpaujl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3txnlgjfy.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3namruwbn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3pyljueoc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3zdajzylf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3vvoxfxbq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3mgvpjlnp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3nvnhrvvd.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3jelhrblq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3hslhgler.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ouopqnal.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3drvgrwlz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xruzqkig.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3twadzcxg.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3menzwnko.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3gddfxyst.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3uspeipgn.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3cmegtxzu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xmmtngnk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nnjmbgwv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sznkoxih.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bzmthyoa.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3twiqnxcf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jhwbsbfr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mbmojvhx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3yvnzyfii.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3iuscudtk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zqsqigsg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bmlmfznu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3brcuedrh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3cwzdmaoi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3htfopktc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rywlmjwn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lrqmsncy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rqesoyxi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3psvusfdc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grqwsfxw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3xbqiinee.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3itmimggo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qhmrsang.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3hgetzusz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3iqddupbp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xdlabziw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3gyjlrvjl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oqxootjw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hqyuywod.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3abbpxefq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3dqhqvqjb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3lltcgxtt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3urpeiaru.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3khjedxaq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3blttxmdq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3zlmrzfld.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3dcyzmhod.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgwphukc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3eocunwmi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pbypfbnz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kxifswjf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3elwnzero.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ezfktgiz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3wlcatufm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3hnsqkeda.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jafiiomd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3getrxmfg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3hpvnazqh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mqsfwhsn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3syroacgt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3frifusof.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3rgsoigra.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3kxmczqmq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3scwhvubl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3uadhazyh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3zsqdtabo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3nwcnygor.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3nmsbtvgf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3maraidat.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dgohlaaf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eczxltpi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qpbziqyu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ejznkqaw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnasiyos.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uxitzmip.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3isdzglsw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nailtkxm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ddsutgfp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ylwmgutr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mirpayfj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hefhbrgm.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nplqaokc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ftbmqmrz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yqxgfrwn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3nnsdjtgp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3lkzrvijn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3dpujyyxa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gnxonixs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dcbmkibc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ndfgjodo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jencndwq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3nbtmtltl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3iysyoanx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3xugxuwsp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ynopvsrm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3myvhglud.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rhzkehyr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rmoxlnry.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lfhkhsll.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3rvggzulr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3suwrpgla.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3fnrcywly.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3yfjkwbai.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3glgzzerr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gchqaktu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vyeekfmc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kbxkbtaw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3malaeeky.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3bkishlse.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jowzidnp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3aaosxvrj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ypdoxssg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xywefqjo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3iqcgbell.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pgjmcyey.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oibmppgx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gqtefnsf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3exncavsr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gtkzfspt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sbngtktc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3vglkhawv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ughekitb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3kxwvnuer.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzlibmgt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ykgrgqts.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cwbneteu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3lmszinqx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jsanewvg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3gjfgdeka.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3vluajyhf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qkkqwpbm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wljeuqag.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3xjnkdkap.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3neulefcd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ikiltmcl.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nxezsnvm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3wjzrsnmq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3qmiybeby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rkuklamg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3lwjghuxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mznbyybl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jbqcypep.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3iacnklmp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3jalhxtbx.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jcrsxbel.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3shmrlflt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3gwszchdi.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3hwknmtob.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3vmqajtdo.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3epzdblne.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fooxjiai.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3rlqovzgl.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3dnpdofni.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ajaynqnr.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubhememk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzsipwle.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3crvfctdr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3lezwhkvq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kskmcybm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3tmlnrwto.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3bouerdtq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pqwakidb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rorinqsl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3bsxgqjfp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3bzcscqqk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3vhqppzsb.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tmfwcolx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3juduvgne.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3mhyhzamz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cygwvoqf.html


<!-- 参考信息 -->