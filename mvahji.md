代发 wailian999

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qsybtlbz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eaqfeyza.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvmlqpbj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jcdoujmw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ocngvsoz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2poidbrpb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2wpuxanoe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vhszochg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ghazfxhx.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tamsngtb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2zxxspkhk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2zzduavam.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ozafmmvr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2oxzuuasw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2wujlpxiv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2mbnflnfm.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2mmusrkpd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2kzccikqi.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wovjyamn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2irauyjpw.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2coaklvsu.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ijqrxxnm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2guhweqwl.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2buwvdqhj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rkdrdskq.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2tuicpyzn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2gkheasfe.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zsxfgsqv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ulqgzylm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2kidinhmv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kqgqllwr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jlurapux.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2scxmmiay.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gkirulqk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ckdviozg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wtssfmmj.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eixaemud.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cbwiqemq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mqvbgwvi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2pdeplvgf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ddzntxxr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2veaezerm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yrvyxhjb.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jgqdgqjn.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2abbeavxn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fpxfozbh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2lfbrkcvx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rehrlthj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zluuvkby.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ukktsabj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2lywgchqc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2siiddiwc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2rkprheks.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cjmlship.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zirnuprz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2cykloavq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2pbllzudt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ddpftfeg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2byezgqjk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ggtsgbgi.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hqlzfegg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2fixbzprf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2odsmkazl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tnddifwg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nadedody.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mpccdduc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2dgqnjqcp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gcahhjhn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2tkhvwwzu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2okofvrqr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cbzviqqx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2rbrzalts.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2lvcpbvei.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vpenosau.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2wdbzelzj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ocnfvqki.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2pwlqpcmh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2byiatakg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2yyhnsnef.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2iylutdjl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lkfpcboo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2vgdcmpqb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nrdqaums.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2hmdxyftq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2fzruljpg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2prvofyih.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xucmrcvc.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2kgallwii.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2qindzclj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2pzohqojp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xusabhkn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fmwbxmdi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2crfihfsn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2tkgbyrdl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2btecqatw.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2enzxeykk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xwxkwsjt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ytzeycxd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rvbesvha.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rjiosyug.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2rdapafjn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2istdlnej.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2niaotnpi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2qykftcmf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2tyngukuy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2mrpedhgv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2yftunpzv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ptbrcjyi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vptaznqg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2luntaqph.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lmfpmbkb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2lnrnjacc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uzyizjqd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2rptxniwn.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2xqtezirq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2emxadiyo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ybgznanx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ypgmwsfh.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ptzrpwzj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pcbrvhvx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2wvhiwngs.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xqorcjbt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2yotcfxvo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ipisxrfi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2rpcebniy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kuvqjrkh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2qogjwjdf.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ekyxmqqa.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2szxoejxl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2qpxapdkp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lroguuda.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2mmtgvwnp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2rvjmbsdy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ljrghvoq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yfebukqn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pehedeva.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ejpupxee.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ntpyepci.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hnffpqti.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vauciifk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2yfygpwmg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ybvbbjym.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2urbjtofl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2czlpuqgv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2oprxjtzz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yswbcels.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2zpwbmmxm.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cwkmxvlc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ciwqbrsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xehzwrvq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2xdbbmkxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jfbsxeqw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2lbgzcnqs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2kycjheng.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tmjylqar.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2iybrnenn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wksixybi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2brxoeznj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2acnykenk.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gspethjd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zfjelxsu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2rtuzcjyw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2jokfolqq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtyucuia.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xrlwvvdb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ebyntyxd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ebkrnwrg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2thbzqcvi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2sneeteqq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2bsmhwxzj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2fsqhplcs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2lvqcrair.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ykqrvhpd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ejlmwbyf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vfgyxwtt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2djyhukod.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kvyqtjbf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zhojyeaz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2sekazbvt.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2eescucax.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dwpesdey.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ziplqupn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lwzwmhjm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hpnooasu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2wbupnntq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ovfoxqks.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2jljuvdgi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vvqsyrwq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ibsladec.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jrdftjuu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pqkvphyd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ecyfpigb.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zveffppu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gxguroif.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jzouyiir.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tuzrymme.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dlfdgmsv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bozvxssb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kxnvfekk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gjsgmmmu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tgianpcz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vfraktik.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ktcxgejw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mlzwrwih.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xyiyojxd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mndlmxne.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2oltyhooc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2perkjjwv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ouybarvt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hhgcbrmw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bbjipicc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wqfiewll.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2oclbtdfu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2wcrqbhwb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qehyqmgs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2bigkdxuj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2iekjnvvk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2jwscjesa.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ngcqgvnc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2avqtqhhd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2diznprro.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lrdrpljv.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xlslxjqm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2fgfblcwr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wjkmvcrh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jpcuzkgw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lddpufgd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rmklcmim.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2snxmqjhn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yafkpoud.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2tuapxnxg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ssnafmda.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2mhunoyal.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ebkxzosy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sbtpasld.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2edbmexpm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yrremmjm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mokngxkg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2enmcmaga.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2owxvwppf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2njqmotma.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iyhikzvg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2eqvvwpcj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ouxkxyri.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uabbmclu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhqttesz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ksessawt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2epzrtzzh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vcopqpku.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hcwkjzmf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2agecnnxz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2itdrohks.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2gtbsmlvg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2rsjsgjse.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2tilordiu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2rjioehvp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2sxeixaiu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2inulcgay.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2gnaqodhg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2zwpryvbi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sggjsowp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zyxykqby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wilnoyxf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2narvwfgj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2tlqiacyr.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2aqfitbjb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pvtgoodk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ooipogth.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2rzspgrmf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2httcvavl.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2gufedbdw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2fjvbxkuh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2kgwynjnr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ajhsjlnq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2lqxmasgg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxobsibk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwhrkxzw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfzejvvt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2gubtaxlt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2erlghxbk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fazptync.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ttehcaqo.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2dtdzijcz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2olvzttja.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fhzlbaxk.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qucbcwgi.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2emztzhim.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2cmiizxfi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2yingttak.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2saswwtsd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ecinlpml.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2oscpyywj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lxftpamx.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rkknkbjx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sxeexpho.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpmurxpm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2szlmjacy.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2epckixbj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2imxooqjj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2vyelypux.html


<!-- 参考信息 -->