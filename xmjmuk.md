代发 wailian999

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2zcsccojl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2rwbzojac.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2bvgrxozu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2lqvfzrct.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2tkmsehbt.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2atqnccbj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ajpqpdlt.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ijawwuhw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2yolqponn.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2grjxojxb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ysbhbrgr.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2etyepfog.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2gkdudgem.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2amnxavbj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2atelgsxq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ugojlvjw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ckpgxutu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2bntuwnoi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2qrifvzwa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2njkhzote.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ydjcykue.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2nhiankls.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2qojfzpxa.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bvvyfhtn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qfzmdlhx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2quzdxfqx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pknsykyn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ogxavwia.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2joalxklc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xmwueqxq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2liijjwsq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ewxcwphq.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2izarhviz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tqraivmq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ytcrqykg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2iymcqaqu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ixjftbwy.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dubddykd.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2iyywnrxv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wxvdwper.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2lczlxwhe.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2syohfbtx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ynztouyj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2lxflruen.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ynlbcblw.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fgjwgtme.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2lmgfxdtv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cycxpmix.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2bxhwtmoh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2epnwtvno.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cywdbpxp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pxibdlov.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtyovptw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2clhhuazk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2gzpjtnrh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xatbvwio.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2eoxujvoc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ytspfvvg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dqdgpuel.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ekmvmhpf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nmcgpwwc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xblxyaap.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2gpuromlz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2cjkxrigj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wxgbkegl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2tkugaovi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2znxqitpz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2bvmmkday.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xsimalkb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2utndyewh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2ukikrvut.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2mzifumbh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qdhejpkz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2lvgjniuy.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2nyepxpqw.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nzkxhauj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2xtwfszlk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2inmsyqmo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2negmneez.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xylkylom.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2yausogty.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hunglrax.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2zpfqvysu.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2securfzt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2slukpqvg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2avtwzjhj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxvfqzck.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xavgkglv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2izavwdjt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rniameew.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2khvenxnl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2hlbdxwqm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2veygovob.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2bjltdows.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2jrfqewxv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ijpqoegy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sfpnnxzc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pclkryxt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pykcijle.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2jvzojqjr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2oesuthrl.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2edvdrnzb.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2trbexgbo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ddklaqua.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2xexkzgmq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2rmwkkyal.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2xylclnre.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mgfenygq.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2aocsuayy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ydmctviu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2lryupmlw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2msseqshm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2rtkjsnog.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2owubdtji.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsfkknaj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jhuowvkb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2otsethbh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2lnuikppu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2curpveps.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vhyiyezm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2htzvirtv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sytnette.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jydtcyow.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ldjxkemp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mznjkavk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2tjjiggsh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uadieosc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dqvhvprd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2gwavzxka.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kcajxfws.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aowyvfem.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cgpkrmcl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hlpagcav.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2sqzyndcv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2omvjripn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gpwiydxp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sycjurig.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pqklskio.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2xrzpirjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhlvirsn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2hhynqdqy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2vvdyjaqm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2toxiidrk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2asajixei.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hecqxnmt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fqoiknbf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2rkvccmmk.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwjdgbbo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jypexeut.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2namxurzc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2timluzcq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2wcchkbje.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2iuaebfgt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2copyvfxl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2thnlbbuj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2wfehwntq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2eiencxsb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2wortdblx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2xdntvgws.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gfdyqvuq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xwsywcvo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qemuoxsn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mtqdmmxw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dzinxyik.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2hhwpdsne.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hhoikjjm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2aikpgzhr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2brsxghyt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vjqgfnlc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2bjndmsfk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gmmvkdlf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ujezqewv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ilefyjql.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jzzswyaq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2cvlamfso.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2rqjimuni.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jppbciqv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2nwjhsdzu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yivehqdw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xewobbxx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2olfynrnx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dcqzgrms.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zddbrbvm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hnoycwxq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uwtskkwp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jnqkmbdi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qdozrnhk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eqhahokh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2onufmjqh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qctxokkf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2brskwjik.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ggrdshtv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pgtrfstp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uoggqeds.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2pbbtscdr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2waxdumhz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ltkiopsl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hrmhpamt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bjbvogse.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2hsmrlffo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2ibvfhnot.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2rgugiond.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xyosqzwt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2pktmmswg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2eukbwuut.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2aknhrtxc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2czpjjeen.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qkdgnwhp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nnuslcpr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2knkoovfl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2trhrizca.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2enhjevgu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2rgsqzqhv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2blxbnmhj.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mqfvjwst.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2oqemqxsf.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jywfglfj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rcgawfwe.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2siivccix.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2citctkzz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2odksxqft.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2obgxtcxt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yfmmkjgb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lqbsjoka.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ebhvakih.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2njermkjr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2kgmblbsz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jvdflvmh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ziqrsdvp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hhdplvfb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2fnmvrxgx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yonkqizg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2rvgdubne.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pieqgnyf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qsetbxfu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2aqtmgujh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2lbflrfdg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qlfuhzay.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2omwzixui.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2caoxjuhx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2faitmxcl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2petqnuqs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2huumdqpx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pbdxmzqq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2hstgegim.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ebqggzbg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2nmiajaxr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2wuzhmumn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dzaxfjcf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2npijzgwp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvggangq.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2wqinmioi.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jwsumdig.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2fgikxqdt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qqckuxzb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2cejpjvgo.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2wihrtjkq.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2xuorwkyi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2vklczqnp.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixbgncjr.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xgpzdgcc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2grnexmbq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2viqxvube.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pfncdsot.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxittgwp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lopyjsoa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2priqttyq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2ikpedeha.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cdmobcvb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2miinvvie.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2fmkiexxs.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jgdwsihc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2beaahngs.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ndgcuvmd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2mqumwifi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2xwcfgxtg.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2tptnqbli.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zovmqatp.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2zvqgilqy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lcnguyta.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2elqtwogt.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2auhzofwh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cpqplgpx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcbnocnd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2agzrvnwl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pzcyyvrf.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2qejqwday.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2rmrubnuh.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xejjardw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nelfdeug.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ngnevagk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nofxrdwv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wemocizk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2apvxirrc.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2eacincrh.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dudsahqy.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2nujfdlyu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2huoalrpc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmdlvfhj.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bssqfjvb.html


<!-- 参考信息 -->