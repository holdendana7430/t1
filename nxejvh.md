代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3boxhggeq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lvjehvfc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tsuhrzdx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ehmzntsc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3fzloybsq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kaunyywd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vjhlagan.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3peqnckai.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3cppxbwbp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3quwgktup.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3tuauxplp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qfndsavf.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wgepojln.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3sttfrrnf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3boqwcprm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lfkidnet.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ubsrfflx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kznfcxag.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3byuvjxih.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3iniuhfqr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3awqnwkdc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cwsurmhy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wpunebsj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fwonsxwq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3gggwnzcl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3pnhjlvwk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jewqitoj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3tgdhcaat.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cvzzvqqu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tdhpwbqc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eaakpbmb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gjuwfjyv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3tbcghkfg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ixuysyng.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zphjfqhu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ulxnjoup.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ziptnbsb.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ltnylkew.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3abjmksbn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3oahcdlop.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3prwxwvev.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3svtuepxy.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hbqzrsyv.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qgsaaxci.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3vvwotvug.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3pnbhrcsb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqsgcfxk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bjsgfuhh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ajvbquxz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3thdamnvb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3dyklrhxs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dldqymkk.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3jktygrgp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3dbpaqpme.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3leghzoqt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3hswibfnn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3hnynbpdy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3csarmciz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3qqqvefsr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3qltjiyrg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3iacdsldn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3skeisanu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cymjewtl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3gnolwdxb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ytdaktfd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3hjwavcdq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3rfdxvnby.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xihqmioy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3pixhktrr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jmbjpjcb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ooacgand.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ztyvszoa.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3hxvnfhfh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gerqxcsd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jwrniifs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wsztcfut.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3jtowirzs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3aueojhtp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3vcydbomd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jrmtskup.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3jvyulthz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fuiexswt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hfoamyoh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3idrbpxnn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3joyyttap.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3dgvvfypo.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vhjmwfjp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3qtvudqzw.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3sjxfludq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3kbajqivg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3yfrmtqex.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wmdmgcst.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ubsolhbz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qvzbupme.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tcgnlaek.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3ryjidtpj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3acixizzm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ujqmonth.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3jheuqjgc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cdzywdgs.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vcvgajab.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3icatnahc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qjhhrhyn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3dxftycdi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3iyjipena.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3yvpbglmu.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ngfmiefc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3yisqpfrm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3uksjpwoj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ptymxwvw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3urvbrkkj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvoszgld.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmfutzjv.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3szuvwyxz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3epqxjaok.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3vqxzyjav.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3msjefeoc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qvmviqnq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wxdxyvnn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zndzvxek.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kdkazcwt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3fuueilet.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dnevteje.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ngypjubj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3zystfytp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ngzryfhe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3iaranitq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jrfgbfel.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3npyhplke.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3yrurlqit.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ncvujrsj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3schvtady.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3bolhqrni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gfxvoaqr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ypiybumw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clteaobz.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3jgkvwuzq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3unyglqot.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wjifxkiv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3fwbbvnla.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rjtfusba.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sjqgzxyv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3lmksfmvd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lhbstemo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pkomagxj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3hnafxsel.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xszhyojl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3sclnjbrn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ymheybgy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxihjxca.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dbhxwkta.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3dntrqqlg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3hmynucqj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3hwmfusps.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3cvkwvnep.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iznrgrdm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qnnhzqjl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qgihzxqq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sfpmscvc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ybnqvpey.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3uayraszo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3dikoezab.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fhbmeqqx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3urgobzke.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yicvjlaz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3qrzczgzw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tgncexwk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ybockiof.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3lnxqnacf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rolyacuq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3zfkrtxpm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3wcoeciia.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3awmjlayb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3pwliyrru.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oeycbkzg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3stezrcvw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tmqcasbu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cbwoehpn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3mpwpebna.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dezozjru.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xjttawge.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3njegbmvc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lshzrgft.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nnwyefvx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3enkfdqhc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jljjaqmm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3blphqxci.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fmwuleqs.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vaqxywas.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3chhmhcle.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qsnzwvzt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3viqcmrkm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3paxetqnh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xyjyzkwe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dghknaby.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ncasolmz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3kabyvuzo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3lftrooma.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3pssxxdie.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3olmfveqy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3afhroodc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3xbtljgml.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bbbkykmc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hmencqgk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3jlftxazc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3fojgpwlp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yegshopl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3demkotqc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3oltggtqt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3umikmzvu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ojiloevc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3npmsabcz.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3pznitpcl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ogxmuwfl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3jphctrlg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uvxfwgfs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3uzogqkwb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3tjsrbqto.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3grsobuyy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tqxmqrku.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uivrclbo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hetosfvi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ckdjcqtu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqbejxar.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rtstijnt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jaxeikzb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3gecnjuyb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhkeqlax.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3tcepdyyx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3icouwkaa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ixgjkkrn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vxwlsytx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3hidmcxdk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ojvovdks.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3tpxbtlbt.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3bomhnwvy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3zmmeeaiw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3yculjpea.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3lzknuifq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3aburwxcm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3etgmcrgj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3spdainkf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3tkubgghl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3pjusvaqz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zgxfobaq.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hhnthgff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzbnqlrw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3bxmorpqw.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3nbfkbbed.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wivkwdsd.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fahjzqyd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjwnztsn.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmbcbyga.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3vkmajikq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ydhctgiu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjavzryu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ppsierjr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3bzwvahbg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3jbuwxhdc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3kfwqzukt.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ojxcxakr.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ragmiyzi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3qrecgeaw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vrvanlzv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ehsrcmvn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qtbknsva.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vfztqfoc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ldtjxjfd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jyszeiqz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3karniuyb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ttycyjmz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mdcrpwyx.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qntiahpt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3biqcseli.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3kqleghsc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ndfeezcc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyavewko.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3kbhpbufz.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gazbezvx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uktggquu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3joztuzzz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lkfhqcaa.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3rbzddftq.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3lzdjbiyb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mwfkvqck.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cfjeltme.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eknxlhou.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3stypgfui.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xkfvlrzx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fgiztpxx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3gziqdolp.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3hyxhxryi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3cwirdjxw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3umndpqtt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zoqmqeyg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lihszpfe.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3srlhkxen.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3skkidhyr.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jwveyvmx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3iiqrazhh.html


<!-- 参考信息 -->