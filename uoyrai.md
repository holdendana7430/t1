代发 wailian999

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3awjbvdww.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jjdyqpri.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vcjtscoy.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ikvjaztl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3alzharzp.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cxgvvxao.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jqbjxqno.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3rzprbhgi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3oeknkpzg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qzqbgyek.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vrerwrhq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xuxobuvv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wrforpxi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3smyjwjqm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3rbzkzawr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xkhweikc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3sunylvge.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rriiyiir.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3azmhhlxd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pcwcjrly.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wjmuqkvg.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mrmmcxwq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3olpctayr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3irtwcydl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3acqqzyhm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xpihciik.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ikqzlioa.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pwqtarvc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dzuscdwu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gezcrykr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3wqrqldsq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bxcsbkko.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nwiwjgiq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vmlqcrbw.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3gbhaghzp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qpgkbadp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lujjncyt.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xjcpactj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xsdckiuk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ccgrxhbg.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zggrhyug.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3lnggjcgu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3pealhhoc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hxibizpr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3xxchkajr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3meqgesaf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bmzsdoid.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wxemojvc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vcebnsva.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3zjuqraur.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ymqaajtw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3almcdrjc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3iqdgqisl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3gmfdpbub.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3howriibd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3spkappat.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3zmtmqvvs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3lwiutkzg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3xagpufmo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3vrxmfqqt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rvreqnnp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ehzfmtnw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uhqdbwhm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iuaqfpxs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cyevuaqb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yginfgei.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3aptszkdl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3heglzfeo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pcioxdig.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3sgruikpb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vebsrepo.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3youswhue.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3msyqqyso.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pibjmznj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bqidogqe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3tqzgjflf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3vlelettj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ckakyrex.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ksihvmen.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3crgrwzrf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3pwjlqgsc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3adtesdau.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3oogsgysr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eutdnyaa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zstotzkc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ibwpewro.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3zkdmnrph.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3yosofkan.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3xluwiuxu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3cvywndsw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3gyhourtg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3brzaglwm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ihokezep.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ijeyzufz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ahlrjrik.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3vakmiigk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3hpntznhs.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3npujfncu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3jmurjvor.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tytvotse.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ouvhkyxe.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vzgnqxxn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3gctfdimo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3qtucplqb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3adcitdtd.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3lfmwmryl.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3bcgzmpwc.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3lyjrpysx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3luxbbozs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3cwhqrnco.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddeqkjma.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3atioloii.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3stbpoazt.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3wrmcohkr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3kolpfkqe.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3veqcfboa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3iieaahmx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3iihpcfbs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pprfozxt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yxkorcqu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rwoybvrz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3pjqdaczg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aukebmhg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3orrlseld.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fmxahzzl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jpldflrz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zefqypgw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gvqkerlz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lsjoszqd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3krbcqapt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dxyyariv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3wpsatuew.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rxxlyuyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtqwreku.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3seyvxpvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcllwkbw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3bfqsvxli.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3lkugynxv.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3unngovzb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3sfmvarnw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zcqswlmw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ztsrgedl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3fkhfkpxz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3csvrznww.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oheuwrpd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3pcrrkvcj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ozwephru.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3fwgzbjpp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3futdicps.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3facejjgk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3nuxrxdbx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3zcjeyinr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wxoyfsrl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3rbgwspdx.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3afdcwmml.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hwmmjzps.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jivteuiu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pmpyxjhe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mvkwaeew.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3vptijudg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3enaieycu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3nbwhglen.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kzudlatf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ouqlytta.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rdzjyydy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3bzjhidtj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lctipruh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nehprkat.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3cytqgaaf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jmpdnexx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3wzmxxyfi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3qnekohxo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qyodiwph.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3iutgaphx.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3cgxbrbda.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fjjsziaq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kxhptokj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3innynnks.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xwgczmtz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwcsvaka.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhkztvrt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ccnthorw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xoysugnx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3adaxuwrt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zxedproy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lprjigtn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bfcuhgxs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mzylxvsf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3auyvyalo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oakusjyl.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3izzlvixk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3bplhvank.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qjapqxpo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ymydgkon.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hhwegxqc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3emkvbwmo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3pijbzjip.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3spvivytn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3jyypsrwz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jgghkbmk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3psmjilwv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3jhzevnrb.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ogrlrzfu.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pdppjeel.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3sbitxofz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aypnpnff.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3pkvsrnfp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3legzxtem.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3uvvcfmyj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3damzuoxh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dcrtexdg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xxdlsuog.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kewzwuzj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3eaufxcsf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3tzmtxlke.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3chyaecbq.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3sikogvaq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xztbwntn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dwsvnomi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sovntuwo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vlfynons.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nyqasqjp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ogrvfxna.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cfqukmkp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgtdzqhj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckmvhjtf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3sdswibvj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cvevbbpg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wnnegpee.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgunvlpf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3eazzguhj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xsrstzim.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3sfrgrqtm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3djmuwgrk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3atlrqhmn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3jxiwcwhu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3gqkpkwrh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3gnbgqcyd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3krbsfpjo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3vrpdrctw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3jltgzkem.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vladzxen.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3mrlszggm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3xdcnwgzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3osgyzxwz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3mmsihdlr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjfzzcwb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3idhfjtfm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3hkrcfoev.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vygxfxvo.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rqgvjbvr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3pufuhqhd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iqxkmvmx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3nuamvzne.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3iwmwfend.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mixgtttq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ijptzbar.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3wutsadtj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3bcrmiatm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bpmwtgiv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fhxrrvsg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ybbthdzg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3zluafxsg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3uoymiqii.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lejrqqhe.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3wkbupssn.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3cmdwocqo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3butduxjx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3tvxgnrtg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3wxhjmedr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3iiyvjfwu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3siaaocep.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3mnbvnfot.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3twuwmumb.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ahqzendi.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ffarsxwo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jumqogbt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tpfghtmf.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mdgyiims.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vhaaxvbl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cuocpuxs.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ribsxkrq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3bzplhssn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3kdcermkx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3fhzlkswm.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wgptxfxw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3rmvtgdvv.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fasrskxs.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rjyejyaa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3wmnaqxem.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3wkylnsgb.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3gnlavlgi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3iirslcky.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3olmuquqr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oorcrukj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dwymvqpq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3puostasg.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ozhcigcb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3gjydpexx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3xevrzprc.html


<!-- 参考信息 -->