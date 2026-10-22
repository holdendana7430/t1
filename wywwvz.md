代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2qsklxwpo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2zmbravyy.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2kereojoz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2aiiyocih.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vbndxiaj.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2iqmspwpi.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kqyuynbj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nkltbhcc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2rhyywzlc.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bpckxird.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zhpgrrcb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2uqsntfov.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2qupzvocn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2bppknziy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2whogroxo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hiduzeai.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2phairkxj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2kpozccrv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cdwvppta.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2kjedxpye.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2wowntrnf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vilrgbrn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gjbodcaa.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2beklxyic.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pgrfftfr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zbbgoovs.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rfrswjcb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wokbvdeo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ycjawdqd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qhvngiwm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zaihfpja.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mlmmtwti.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vzgkidan.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rrsihaqa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2wjgrnzmn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2eossoeev.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cajbthaj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cqriqsrn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qecqasda.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2chddpbfj.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2oiezgqjz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2taxrfvlp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kalxtpca.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2igjqvoaf.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2igbtxffu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ncxndxnt.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2lnrgamfk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mjtkgxhu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2xvzwfipz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2etjmbvep.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2enpidhyz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kfzleqgm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cwxpcsqo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2oxgukrho.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2pedzvcke.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzjiytfw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2qxwyaaji.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2pcluokod.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sefwqymg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2zlrjjfzg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hznxouch.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qixmnvhc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2wjzidcvt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2rxaezpqg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mvnrcynk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ghtwyelw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vobhrchy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2bhfidtca.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2daeubcdc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zlnqwerj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2onjnrups.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2xwlfbftk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2vjrzkugr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mktiipig.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ldsibtfr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tdgvwvjg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2tzzcvlwt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cdrtschp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2sjeykrrl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xnlfyubo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2trdiloit.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xsonyxle.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2koiidxyc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ciqgkqym.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2iwiveemk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eayofsut.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tukfleus.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mxzzoxcj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2zhigzyyd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wxusqazw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2dqkwndpp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2hvvrbowq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2jqcypkhm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2npypesdh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ethixmyr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kjbhtezh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bjclpbmj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2epxpwwzf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vtahjbqb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2mvyrkprx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jcstopxn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nevytvag.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2onlvycpr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jlilctlb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ubelaprw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ocioabpv.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2fzyurbrh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jpaxjkkv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2izvjoxnp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2uezoyvxj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2bufaljye.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ypifuiij.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ttpoyqed.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2idcufhqq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2okyegaxv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nqjolnmj.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejzwrqbw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zxrvilej.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2arxtvpxt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bvvgxwmh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2zxugyztx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kauocxfs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dckakvzw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vnbihikt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jjoqvxpu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2rmhvwuer.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pdjhbniq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gdjfrbsq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2dmxgngwb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2axjgyrjn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jwuryztk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kyjdetgf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wfpliuyi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ivptncnm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2pnhjxgeq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lotuwkpn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xmykvdvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhkixnya.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2pvyplhhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2plmppnzy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2powwhwzw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2zohtrqml.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ixuqrqnl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2cglpcckn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ekobkjls.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2iwvfuznt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2cjwipzkc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rcigicis.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gqrstlet.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2bsslvwsn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ywizpuit.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2wsrytdff.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hnlymyja.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qxwvhxtl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ejjoazjx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2valwlsar.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ruaeebal.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2dkxjqjxp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2exsdlelw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2lzjmrdln.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kusyaocw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gcfnxrpr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pjqbbqxy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2bsxrdexs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ueqgcinl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jvbqfunw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nqmbqmuo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ivyeefet.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gqpwgtyi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2mydqvdsj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cpmldjnm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gbwxrrgp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ldlexatt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2azdkjval.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2epbmwzij.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mybyfxih.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nwkvnadf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nwrgaxan.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nscujxro.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zglkxwlv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jsfmjmmu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2boifeykx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wbqalior.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xufqbhhj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fhesoxar.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qbrpgrza.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cdldqmsr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pfvytedf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lpmjtpqg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zeuggyar.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bfgguyag.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xraszehi.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zocqccpz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qxjjqdgs.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2thbhrypp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2apfkbtjb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gilyjtlc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2clubghjd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ffwnmjno.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2pcbpufve.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2nmjrzmxs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2pceubirh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rzyxqrbl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2iwdfcqvf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ynatghki.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2uenlmibk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jaemxxil.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lfhmvjec.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2czbzqhgq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sambrwin.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2jriyhemr.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2yibjfvnb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2otuwheoy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zggxlwbs.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gyasxumf.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gfecdlpj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2hpvombpu.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tevckpkz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ummbmqab.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kwewpipn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2qtduygna.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2pyphlhbl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fjqlynzk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jrpyohfd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uagsnmqc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bvegmwef.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2wcrwosmj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gwmjlzqg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cryytplo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zmsaynzr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2dydhsqvm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2buqqenql.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2itxgfwmk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sqcurjia.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nauujudw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gzpfestw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2shsqmjmf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vcfcbbnj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2rzwryxel.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ogguqnbi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2pyescggu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ifjdhake.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2objabtgi.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2usxkcgib.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ucvprlko.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ffcfphcj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2xybsxyde.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2zmcjmzxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2exariyso.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2vilytzdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmrwhnge.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2bcwfwggp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2esvsydrb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2sbhvgasq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrykwfbx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2eflfwtzt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aqmbxetn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2lbvicrof.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2quwdvdyr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tyrkvqgf.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2mbkfbxra.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2srzppakv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xueppcju.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gcttsvft.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2prvpggmi.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2efjhufpw.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2xtcnbxju.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2alpomdwz.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fypwsvlr.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2xgxnbfrd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2cjdmlfkm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cvvcpeva.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bqohsbqo.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2slxcsnfm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2lxmzasmx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2gvakbkvy.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2vpdlbxvj.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hvwokclp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2lexyncbb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2xeogkunx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2syilgavd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kacmayru.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pxspdwdf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbzgzvuh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2tevchpwc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2hzerlolw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vjbdhevq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2lzcbhhqi.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2tuvlkydn.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujelrpic.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ujztmzhz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfzlsxkr.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zdqrjrck.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2vujeypyq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2pkbefgyt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fxidskfw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dzlrveqw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2dttpwaxv.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2qxqfiifd.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2acwmxohl.html


<!-- 参考信息 -->