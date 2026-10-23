代发 wailian999

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jtugldwe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3guntspyd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ehivfdsd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ecafmrcp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nnnkyejb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3riyrlqhp.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3brnjtndx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3pytiewnz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3zglfxoix.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lfazpynf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3xpylqowg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3sgzrgife.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ctchjfkg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ldwqmlir.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3fejxbyww.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rzmutpio.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3okdbmqwr.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gtjnryva.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lkdkkyta.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rumcqnrq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cmorladl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3alnejnnq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zbpxyngo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3nmabxnhn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3olnutuvu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kxelxska.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3itedgwqm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3htahezja.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3npwlxhmn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3frcxojtf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3hhnzsjib.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3zvhjeybf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zialtjki.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3quqaqfbw.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3uskkzdto.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3meeiaebf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jaslzdiw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ccrvnmnm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pkwfyhcv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lodzkpcr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hhnryhxu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sfbgfavz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3edixtnbl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gwdxohkz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3dxarfxuq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3nktogpsl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3tdzcudnm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3edacuthq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3kbuddpoj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dhqwlupj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3bsxywfvp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3aexqyzbu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vcvmmqau.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3npukjwla.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3cpfmptfn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3wrbhtgmg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uaylphyh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3pniumkyo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xonxyxtg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3cvbrivlp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wvevekgw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3dopigqpd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3yginwygx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3plsmaxpb.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3njflrxcq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wsmqlzbr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3loecghak.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ghtiosbc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ryblhjuy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3mgldyvjt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wmsjavnt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3warkhjck.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3cqskufex.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bdikbcxz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lnxbicez.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lruvmjoj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fbwduhtn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jjmhelgx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3cyeejoyw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3dcawipek.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ofczxeze.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3cecinlme.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3gbwzbnnl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zkimtoxy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xayflebo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ugikpgkz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3htholytw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ceupahes.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fvadofyk.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ieczzjza.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rrahatas.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3edbffbhy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qnizpdaa.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dhhulrft.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3jwuhnkbl.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3grllzzni.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3bfvcoowi.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3kyspxkdx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3bvqrhvqs.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3fvervdex.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3romyzdps.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lpowqevo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3sxyuqipp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3przreccj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3btwfgbot.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3anujpxio.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wpyfxdpp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3hwflbudu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3clccdnre.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fxrkvcqz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xoyofpmr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3buimhkbg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sboggwls.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3afyjaidd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jwnfoxbx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yqycuchz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3kfvurpup.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pbuolhqs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hjxezwbw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3abkbjuwy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3enoqmnzi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3umfmjlqn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3vxwnsihp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ofqqfcgw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ekhzezbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hbunhzga.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3dnbaocdg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jkaukspg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ggjdwnyb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3haunmxgx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ycrwezvl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3awbiqmgg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wmgemfec.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zhuigvtm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3jmmpctfs.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wxturukj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yaguosft.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3zddwgdut.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3btnzkqfq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3tkiwqlyv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hadpugts.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lyrqobxw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qaufpzyd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3aknfmbvx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3mebwmeao.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ydnaihrf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3zjlfdrcl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mmzdikoj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zxngvual.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jxbmlszp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3cmoueufp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pzwoudkb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fwhsewcq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tehgeopm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pmrgcprh.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3plvxidjg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zalbubjq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zwxqljgk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ijwrxomx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dgghbauj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3bcxedbmk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tvkhirzp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3rgfidtlr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3tujbayrl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3utdnnoyz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xasixywp.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dyeyglvk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zsfimlmr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjujhjcl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jezjajqi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3uixnyynw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3juwfpyzg.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yukqnvac.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3digvjroi.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohmvlnjj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rmshdylv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iunaaksb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lcivdvwt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bhzdxrce.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gcimvhum.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nnnnnmlp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jyoauegm.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3tjsszmhq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cjvmogtz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jllmwrqo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qbggjyqt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zvgbieae.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3nnfykcqk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3meqkzyss.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3plasxsqn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3mohrorzt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vqcveysn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ixnmnpnq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3uduvbvui.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fffaxwpc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kqvsdxbt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pacgeaew.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oudasvju.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rxmelepg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jxkjavck.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3tacpljtk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ivfjtyjz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ouckrhoj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3irmtjfoy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3fmxkkpjd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fbxuoosw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3nkwermlt.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydyipodq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3peuofibn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3khsworkx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fmmlkvif.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gdwcomkq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3opabdwfy.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nwuonyyc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3dbomdkco.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qwkgzkhe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3opyjbdyh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3izxyibwe.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3kpzagvfh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ipiyjauk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3zjocjjpq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uovtjjdd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xjdshqsk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rtlahegn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3gttqhgdb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yoomzmwz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3cxxoqbjl.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3wugtswtq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3pdfjbhro.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3byqlwtnz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3noyhjsco.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3yftluyeg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3oduvizfk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3tzbptvzg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hmeatnfe.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3onxuypxr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htrsqojz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3dbmgqnmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3olhxiouh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3jxnizmsb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3cuaellrb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nhbpbjxy.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zfmnwysx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynjdkqyn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3lfofmsca.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ninalmup.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jcwdiekt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3qajjszlf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3ypzlrrhu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3iumlybsr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qmfxeqgr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bwpvxvoe.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ehvacyrm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ubijqzkr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3czguehhw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uyawkeac.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ebtnqcxm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3nmvvaoor.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3qqbnbnxc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3indinshq.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kciwkias.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3symtzusd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3kmvtkdkb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3icfiwyqe.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3euusrpor.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3tgjnyuck.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3xzkfrbdq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3sdomxdju.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zeztxldh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qasirzzw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ytwzwwxh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hthxgemw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dcxzqqik.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pkmzdjjk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3albyceiz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3wuxihgyq.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3vndcksuu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pdvvyflx.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlbpdwea.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cspnvxnn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3brmysmzs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3qhgttnvn.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3uqogcwbz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3euqxsrin.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3sftgwfam.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3tdgicxio.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xbhskrdx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3iveyggha.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3krctfugh.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3uutceagw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3zglhocyd.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3mzxyrpzm.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3olalndnt.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3iudvzlap.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3pwbufnyd.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3fmqdlzxx.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ewiknmeq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mnzhqtro.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hbcyahai.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ibpsraxk.html


<!-- 参考信息 -->