代发 wailian999

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3vxfrxmqz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3weeullmt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oxixujch.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bqnugeoq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wiygsxqj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ngmmhkjk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qyxoqphv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fszlsvhj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3makhodnf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3dmtficcp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3hhrkjtkh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pqpfclfa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3popgtruy.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3smeulset.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3qnijbzaz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3luheulka.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3wqmmxkox.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ayqvktxt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ifsqdbxd.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3tgnbcolg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3axtryvli.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3govbztcf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3nyobugrg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xyirucua.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3esasxuag.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rccpceov.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xienywpi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3dylnlury.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xbwnpfez.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3kkcmeoiz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bmzjtwdg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3oiroowub.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zpeghlgj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ejuhmmwa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3txflsnhq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3yfmgeadk.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3gpuqgjgq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dcldxejn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3svvzzxkm.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wgntccef.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sntufvzu.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jxolscdj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3snfrdhpr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qdgjrmmm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3ukwjfdvd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vuqmxefc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3difnxxbk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3upuoiism.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xhcojrjc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bfpwagnk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ugxjtvvh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3helhjvow.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tvagkxgv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rfshoeyf.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3xqhnpxht.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ltrcolnk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ilqkyfdq.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3dyxqnqgz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bnzecbxu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3plgzjlih.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3faknkegi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nsrzwfeu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3irrqvrax.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qmalbrlc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3plfyajxj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3eirvsfzt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhxgowuj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3necdazmm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gmhxkapf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yuwxjgdi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3dwshfegm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3znrboyed.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3pnbkcugu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3aodpjzdx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bgumebhu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3uyssaddg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wdhgvvyo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jqtesdij.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wtacxvyf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3yuekqhkm.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zqoeztye.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3sqscphhz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ejsvxckw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qddwshtp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3bqiryrrn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3xgjgzran.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3aaswhgiw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bropqsoz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ocrphpyr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dcygajzo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3sdvvipxs.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ivyhjeek.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ftwjahfk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fowensmx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rrytmrje.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3yobqchxb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3izkmzkry.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ucoslluw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3czkliben.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3bxjghoiq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hmekhrwf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cemsumna.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iatrjblx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zexkisiv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3retjikdg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kjomzdxc.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fdvrhbvg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3mlvyckjw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3mxahymrk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3skaksijm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ablcdkla.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jbdolkwy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3odghyfaz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3atlpgzbs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kdykhjjh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zerowpau.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3qjlxmpnb.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3naunutif.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3xgdnllrx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bmaehiig.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3idifdfwh.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3bgunkcms.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3sgkppyyr.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wtrfheaw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ujpntghs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3mbyllkom.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3qjvamxxt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3iygxgqok.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3upcmtgff.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3wiklqnlw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3cogclxku.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3phmutioc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3enwxdsxs.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3pyrcykwr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3aofadhae.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3hroptnzu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3iuycdozh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wcisohyo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xldzlgzv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3omxlhtll.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vklsajvo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qivewnhq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ecuigsnd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eaqhgryt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vnejzqyf.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3arrbjljg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zyqvdbno.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zgjqlrwk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vwexbfhi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3kbobqloe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bjkinnxy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qqsmjqtd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3uwgmftrg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oxbmmgik.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3rgcosnch.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wyemkxfu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3molaomil.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mwdgskcl.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3duehqiqh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3pzienjkw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zwsodccd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cpdrpnct.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3zvjgsewr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nzujozya.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pdykcmso.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3jfuqwdcp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ywkeehei.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3bnxsdcuo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kidovymz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbpoqvql.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ojnfkcdk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3kefaxxsv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3tbahkruj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3frezcjdr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wbacfazp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ywkidbvc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yqnuhxbs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3eitmwafb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rohxpyvs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3btezkxqs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3dseorqbn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3msdvbqpm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fbefscrn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ximijuvk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yjrbcaap.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zharrkym.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nvtpxuhk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qrwqcbns.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3lbdqnmnv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3khddympg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3pdxvvcsv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bmhnbqzw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zticnxrh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3oqiwafqq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qfftpgep.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jkntmgql.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3alltgzjn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rhkhkmkk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3wywwvhft.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dejpbqxd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jsqudhwt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xvjkfjlj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ltmltaec.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vzdobztu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbzpimie.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kkcodyld.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rswgvpxh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xyboiiqu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jffphrgx.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fhrxvkim.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bzxuveds.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3udiefiit.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3bfaqrtbf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gwzvdlru.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tozrbrlz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ibmrbicm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3nmeezisv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3xhxcnejo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mdpffzdm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3fcuwwoqt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3lxwmvwye.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3btwpmwef.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zpirotpt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3abpejtqb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gbettwmk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ipcwmzfu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3pnnnrefe.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3deqaulwr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3yqbcverk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wiuvxbnv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3amesyduf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cqmowuxl.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hpcdurkj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yhuenail.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3lpwsdnjt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ckcxxnku.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3bfkcwshw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3mqyxnjme.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qozhkjqj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zmxvynbc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfjdvesj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cgjdgezb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3molrovjd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xtsyvhzm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lyylbach.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgadlare.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3cevhycsi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3atuthkqh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ekessgtm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rwnxtwnh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vtqigpfa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xdivsleb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3dnzghoma.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uidxgtcq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3qjvlolrp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3vswvfhxk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3lsggzqzn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3cgdqdqvj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3wpcbrgfh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qwaknvcf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3syhoeoor.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3snmeypkh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3yyhuqtyx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3fqveoiby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dilazmal.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3skyorxih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wktfuxms.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rclpuqib.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3gejmnkmf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vlivimio.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fcwcvwpi.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldccvhlj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cjfsglub.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3psxjtgug.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3yybhimuz.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nkxwcdqx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3glbqwysk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3stqwvesw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqxavaxf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ohvaynlo.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vczcabql.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xozwmzqa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3uqpyskoy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3prthyumi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrqiilof.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rnztykqq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3suifdqnv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3trcjgpca.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jyjbdgfb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wpjurtwf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3evmmqwvm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3chgvwitw.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3iwophbzg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3lprqmtlb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3llljonkj.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fomftifd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdjsfiff.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eqltvpha.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vynmelqj.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rsylsiad.html


<!-- 参考信息 -->