代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2itgpdomb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2mzaljrsm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2psnubtqb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2etoiytnf.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vdyrptrf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ateilwcy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2xkdkjxby.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2wlwqpmtn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2qbxylkkf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qjhkyrpt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2bwsvxgid.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fheycuhd.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2iclknccn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2lvvbtfvw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2gilayire.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2vslhrjti.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2hwbtuozx.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sgaakjkd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gyckkpty.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2tsowezth.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2levticec.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2oclfkhxq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2txyzbdph.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2qhzjyetl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2figxyski.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vnphswma.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mbhxyvsj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qtqnaeio.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gdetqxmd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2japvbqam.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vpkowvrt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2crpbfurp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2duapzkcw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kvmzpgcs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2rcstsbid.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dhapsobw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zppjdxlh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vyhtlhrf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lhdnqozy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xwjdblvn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2mcnmbwtl.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tsziqnft.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2uvbxjnqs.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2skmcudmv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hgsscrmu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vumojcpx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2hwqckwfa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hhhbvhwc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vluuppdv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2anhvpmmj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fooadssu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ivfwdlxk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2gtdfxlpd.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jbyjrekn.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2drhjwlzw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2tyolwtal.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2oerggndo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2znfobrls.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2cfvjxrwx.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ndgkuaok.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2vbngaika.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2eubrbyen.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cuhxmlqs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iiwfojfk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rrhamain.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wmgbjzux.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nufiizfl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fuzksxnt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2tnumhksy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ixqihpiu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rsakvedw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2fuidcngg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jouvezja.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hrtjmmxr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rtbyicsl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2rhooxfiv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ndvyjmvw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2eitoggra.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2afjwyoyn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2mwhvstyc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fpwpwqay.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fvcxfpqx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2jdnjhhib.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2skvynlah.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pkxfojom.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2tylyjtzq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xhvmqwsj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2sxfkgath.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nqgzdrre.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dizevabb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cnlgbqji.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xgfrdivf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2mhvgatzx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2twwsvfzn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2jvpzxcec.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2phujjlam.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zybcftbn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2opghywal.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wvefglkl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ldkdwxpt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2zuxobcyf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qfjiwizl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2scrikwtt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2tzvjdohx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2eixcnnjx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ivgclnva.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2etunmdqs.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tbaojxqj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pltvjkvl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ihqqrnvw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ctbujana.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lgfxkpiv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uysaobbl.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ccxwvhpu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2ypfpflux.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ltmbbjtd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ymlgfhha.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fntymbgc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2lrkkqlhy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2yuvzxsqx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ytndxfop.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tfwvpjuh.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2loouqxko.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2thuxktjz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2juchsrdu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eleqpqeq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2blyalwid.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jwyhaqkf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2hfpeszel.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2iyfuhacc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2harmigwx.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2wkbitnzp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2exwdjmsi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cldlxsfk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gcchzfls.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2odilazpv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gpuygqyw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2npuqlzaw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2okgyjygm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ksuwjmll.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2kjyoxqhi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2crnaoijq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pegjgadp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ssnfyrqe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2skbttgoe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2naqbqxhs.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ottcppsx.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nkywomve.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wlhilxxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2asdlqqkw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2zkxttnze.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vycfyiiw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nskuacbm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2dvezgrun.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cmaazwwo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2xotliruh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2iovchvrz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wjmhocym.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2sjlnwgqt.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2puiffyvx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hzxygwtu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2icireokn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2hzsvsvjr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2kryvadso.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlhhnfdi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dmdtygew.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2yqoovlwb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2seefxsco.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ihvyvass.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2fpgzxkmp.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2douymarg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lcnuvmhm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xzqjeftn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hwtpscem.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tirsgewi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mcwasjhp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2kjmrtktt.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2wmpocwoj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wigltzpk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2lyrtdmqr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kpwxpmqg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2dyzmfysw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jfzzkghs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hwhgakra.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ttuayymb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vhgedetv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2kndavvyy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2shmogppn.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2voebxika.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2cyzbuswf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lwmhdjgb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jzelymtq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2psvnnckj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fraeennx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2nvbegfzl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bcsaqhkm.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvyrvmdp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2nawrmpup.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xaguiylj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hbmfmalm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dtkobzpl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrgxdlrd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2isrzklpz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajxrpves.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2olxbabqc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ufdcypzl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2oczyaqst.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2etwdnnyx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2jxzxwdba.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gwajxcne.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fnmwojib.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2icmcidth.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2abzqeugn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bwihhewo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2aslxotxh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2fmolpzwv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2oqopnugs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2zmbfdmmp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2umxkqhqo.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2piqbzryq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tswwbgsj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gvjolulh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2bfbpkdrb.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fmwaymky.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ttdfrzpw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uetoylfx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rxdodzra.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2xdjjicqm.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wdixdoty.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fldyvufz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2daxbveps.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yvueimfr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2ujvxgsuo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2itbpwljj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wzihjdrz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hpkoftlu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bcqzfzwh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pziuswed.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xmbzbdmz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mwjoonxz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yoeehbsl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qjglovfs.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vykndfef.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwjdleml.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2iklcrnim.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ulklejkw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zktvnjew.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bwlppxhq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2mdxssnjr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2bbqumtdu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2boggbmco.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2nkrhgypy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2lfpuemeu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2goattjij.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2iunmjeag.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2lfztnpoq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2wgyegvdg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2skemjxyv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2awbjwdle.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2wvwjshci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nyepmost.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2thfyldfg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2saxnxfvd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2nlqmogof.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2dlmzyuah.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2owkilvoh.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ltxejswv.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2oenbntpj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2bhdumgdv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2scwahshy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2fukstcpc.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rfgvizxe.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2dhubndoq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zpibzvld.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ifcttqvq.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2melbtqsi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gokfrzwc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydtmtebn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2dnlgdxjb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jonbrgou.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdcqvqqh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rixjrymr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qcyvdcsn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2vzocwtgs.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pkzyvmtb.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rprxnkez.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2vegxnhsq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2croxgsex.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2hpgqnvbr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vpunhylq.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ibtbpmgp.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2iolarupd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2tndroamt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ekypeyxu.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpbukmrg.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2oexjjdfp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2jmwghban.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2yvwgpwlo.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nvtfqyvb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qmeusiol.html


<!-- 参考信息 -->