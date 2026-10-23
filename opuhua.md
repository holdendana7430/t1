代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3hpzmubkp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3goaoutjp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3vfvtxctq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bjabuado.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3yvzimsmx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3jljvwtvr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ajcurtdp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3npeqwawu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3iihkkchs.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kiahfuuw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3decxcbbx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ubqpaekh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3afptfgvh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qdotfedb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kdrjnabx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3qwrrrpvs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3fdjimymb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3dljqdwmd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lqvvlfda.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ipezwjqr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jsebhbwh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3zuhmfolv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ojlungfh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cbdeferq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ggnfzdck.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3uibzrbbz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3tszaxuik.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3gnpmoomq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zchymepg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qsixnagm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3muyeyqtf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wfaavxlf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3stlsaycq.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tbonimds.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3brwrqdxs.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3eskbitxm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cjjavpfz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qircspar.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3sfzcikft.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3wapjslbz.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uolkigsy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xmdbqgyh.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zywxwtvz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bejhveko.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3jajxkzle.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3jhdsjwjw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rsghoyas.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3rytlcffg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3vqdgvsdh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ywpnaays.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3fwxhkpdb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3huquiflg.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3peszycfq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3atzwxbde.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3txgcquif.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jdshumnf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hucwaerb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3efwimmtj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3vxaxekdx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zyhdkkgg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3thzwlzrn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3acawbgjn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3nmzzukbt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3qwtisvlh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hzbvkgvy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ztzziglw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vtyxmyjv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3xvxqfqfo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kztfuyvc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3vrueplfj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qjejtncu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ymfcggny.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3stnnjfmh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kebypinu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qnskzeco.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kobvwovf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3nuhrbtjb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3khzbkvrg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gdkkixov.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gvitccco.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3hppmixya.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3hrudvayi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ifgwufxf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3vnffpcyo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3dcsfzkze.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dclxjpmi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jqezukzt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3pwdjhkhh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3uilgpeuv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3oyihocrl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mbnhzkhn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3swgbifel.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3wzzyntdy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3hrurzelo.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3clpeqdas.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3fgrdgmfx.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3rqacfexa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ivtzllwr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3vnjbllzq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pncfhwoc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sjaqtddx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wxkjpapa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bburwnxb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ksoesumc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3hkeziykv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3drzfncih.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3shytwqqi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3pjukjwin.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ququrfpz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qzyubecz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3kpxycksm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3bfyfojei.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3pxvkgzra.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ixpktotm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3lzbbdbjf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3hthbiluj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3kppymhgj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3vaizfwha.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3genwhulx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ezglgofk.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3tzshcmec.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3uvcymtgm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qtucxtzj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3rfulhqjd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3lfixvyti.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3thhdoauk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tutucyie.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xlooxkjb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fhcwnhhr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3mrzshybe.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3omwjjgbg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3sneswcrq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3yegdngsa.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qepfnmsw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pvkzylis.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pcsnwrnz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3umnwjomr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3aodotyid.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3mrclyxgt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3femaugkl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3catgtyta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iodkdubi.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3siugjoxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eyotkhay.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3aaitkrpe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ofbopxpb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3frrbzgfg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3ltpcmvni.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pmrdhdeo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gnxochlq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3phzxakuy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uwzhgbsw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jlnxuyqz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dccarrtw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3hoafwqsl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktvyjcis.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lwwtmvoe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3oonvdlmt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qyvyacuq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wsjyrgwe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3psvirtre.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ehwalbzr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xmioxnki.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3wgyusopg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ukueefpx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qvrrsdta.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cslxzhry.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3taiojloz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3atqekyig.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lwfflbsn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ahgakrzj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3eagppufg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gtxuovtb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3qkriuibu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jhrjaczt.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mbshkses.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3cnxdpvfy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zjjhhpza.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zvuutiez.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3yecqbjyk.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3jzoutvih.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3bduwojmd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xidcflrg.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emfcvkdb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3plpnmuws.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wqcygujb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3depvahxj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eebtxold.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uowqrvae.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3fatvseth.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uxbokukb.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bacjrxrq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ggjmbtcs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqdzffmo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wdjvpvdx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3teudxyoc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ppxxemez.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wyqpmjwj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3fvnveqru.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3nbefjysa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vihpmvts.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tkbwetox.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3diliifeo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3faklrwsl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3nffkhwey.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3zppcmhnp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3jozkuunf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3nnrcoflp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3hnbtkusl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zolnvhqh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3jdvxnmjh.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qgnoxcki.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ewwpufeq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3njfjdhkc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xxpxtxay.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lqgmpkay.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3iytqlsxh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ccmvvoqk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zjylwaks.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3yofzrqdh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3khmrovdf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jstvtcpv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rwbhzzaz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ztodhuun.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3dvaoemyw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xhpbalik.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3naovopjs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3likzdarl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nbmumtsp.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tksbgqar.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3vaaxxens.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3afgvksgn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fmcezvpt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pzfwomws.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3cmdxfxxs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dkzfjsuo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3tmsamklw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nvliewjb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bakwcnyw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3lcsynffq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gtcjcyae.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wlfwdbre.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3xuxvvirt.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3lgrzfhrm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3zbasjkga.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3hlitwbnv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3mzkgyvvc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3omnbwqeq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3binwisxw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3bsfohlwo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3wbisdkgn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3sjzkcjcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qfcwjrzh.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zctrlshx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enkffnhx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wwamaxoo.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3gyfeizwd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oanpybqj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ingclmjy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ppjlzvsk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3iadsgnwz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3pvifqfzf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gnwtynhn.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qidqifzb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3opppryhm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zfgtxmop.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3fohwnpey.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wpwhivus.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3twuqvmee.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3eixzwvai.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3zxybozys.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qjznkxbm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3poxqfwrz.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3leziftbo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3peggvsqc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wgouxdpo.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3erhsbtyc.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3bnqhkvae.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3vszmmzew.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ntzthpvx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ifmibdol.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3ybdslnqs.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3lwmkjrja.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gwqkpvgx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhsyzuft.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozjunanc.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qsztqcxp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzbgqwuc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zzibysxg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nlrexety.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3knphclko.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ysgmjvxj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3lmwogdpo.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3knxxbdmr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gcfnvxjp.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kyhgxehe.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3moxvhjqj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3vfndjmsy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3cmscevhk.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztmdtwah.html


<!-- 参考信息 -->