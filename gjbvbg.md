代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zthebfct.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vbpxlrat.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3zocrruum.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3dsylklyf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3lqnznsas.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3jbprpfdp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3adllkqqc.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ogrljkid.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3oylnykkl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3focbrzfm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ltzwvbrz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nvjuftxb.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iviaxvwt.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3disafyit.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3idmsdsny.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3kyrppbvn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3kltyuevx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3vcphpzzj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sjdohink.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fxbahnjz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wgbbmssu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3kaiuuoez.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3chytiibi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ytqrjwph.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3wftmbaaq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oguiwtnf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3vuaixjoi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yhhdtmwl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3utdxfnhb.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mwajjsbp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3hjtwpeiy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uytovfqe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3rdqvmmzm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3qwoedkpa.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kpxkwxqm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wwdcbizq.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hfvfaqls.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ohogocov.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dbksrdsk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ckmzryve.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3glgjdjpc.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rftxfbye.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3qnlstewm.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qxpfksrr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3mynghdui.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rpeqjhgy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3eilrdihk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3zvkovgyd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3becitqci.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vrcarypi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3dowgvyis.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uxnzkqeg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3djlctbrm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkktociq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mqpssnvm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xpvedmlh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hdevmxtg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kakztypx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zktomqbe.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rjguwfnx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3syguxiab.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3gxnxakqe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wjucroei.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3fydcrygt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bohxnsiq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qzqrjixn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3kcergbfs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3yjhcyekx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ivlytmtc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3tjnmdlaf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zowuvwrk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3autyirnc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vqengvdy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3lojvnjsu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3qwbojidp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3vgiwgljh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oqywixzr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3woentrgq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3eeaenzqs.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ihsxjlzn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3porjmdbe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xtbqlipx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fptpiqun.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3hoafyuau.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3bjitkylf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3wvtdstxm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3fvmnvjhy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3zfmiugcn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ficcykmu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zljspvzm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wdidyiwl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rmcrvwqc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ojmqazvn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3vmdqyrhn.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3kgdnhged.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ydwlgraz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3teiabnup.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3yeimccff.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3oazfybtf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lasbfzja.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3okjztirk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cbdchbaa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tfrqlhle.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jglsglrw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zppzqtlj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3lxpmmvyz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3xbsibzra.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yginlwgb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cyatugst.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3kztyqscy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3epnvoiuu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lqgcmlfw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3qxzlhkap.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3hoztfwxf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3eazdivdy.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xxylwplk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3hlgimgsj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3huwjqtnh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3tznzhgqw.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3burnslhy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3jrpdavdz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3bberusyq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgtkwjxl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3yfuufwce.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3hcoujszo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gsygudqh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3plvwcxzg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3syoojrhu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yjxjqsbb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qefiquna.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eljdmqsz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3brhickcf.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nargrrzx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3svwxpolg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xdipjnxw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3eaveaycf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nvbhkwtq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3gvonckbe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3vqvexpwr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pckkmrmm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jknojyuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3evwfzxac.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3gnmzzafy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxpveega.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3eolguhkh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ganpecqo.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zhovpfpd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3bfwryjhv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uvrjvowv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tvgcxvvm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3fpxdsibq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jjwphhmr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fbvnpujg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3rejqbjxn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3fmcldjke.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3mpckrpku.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3bzjnjkon.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tilblqva.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3enzwpuhz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3cdqjnorz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3xyfsiysu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3xufdejqw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ovjjhlma.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3rdhbucje.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dnnixxwl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3csuewgua.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ugrqhrsp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3zbdhohoy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3yimpwnbo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tflqahrx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kpsltnmv.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3stcnhipe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3oqrfyaet.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gdlbtanb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3prjvakov.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hvwycufk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3zxysbqxu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ctchtbxv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3myvnelgr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ytaqqqiu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3wjszvasr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3didzeizq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3setxtruq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nvegjyum.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tjnxyfwr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wvrfiqkz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3issqpbgo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vvhyghpq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pdivhrbp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ihskqbxc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3viemfgkx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ztbvckie.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3slxptszy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3isozmuav.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jijebffn.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rpwbchcf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xgwmwrxi.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lkyhvngr.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ttljfofy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cyjgmawx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ahlubhen.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dhjgxjyl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bcitvcqd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3yyibgidv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3edmxxcmt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3llgalqam.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vhxuuxzc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3cmongkpp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3vbitgdja.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3yfpoluqm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pehhqfit.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hwrasqqt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xjbpmyun.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ifjihdex.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3epldhoey.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kotxeuoc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wawphbfb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3urmurrce.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jsuaoguv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dryhrnyr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hegzovlb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xecacfgw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3uaqtryuf.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dbakxkvu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3gjaqvjec.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3whffuxzd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vznkigia.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3seqkqwlk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zraiptxw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tfqqxvdl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3hvyhkhxl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3koaxsrop.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rybtpmuf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eekkznbl.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3jzdbtvqi.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ewqaxadh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3bftsmilm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xndpbvdq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rmzwbqrv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vwhmlzxm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3kdbjmmoa.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3teqcpfvs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xfvukmgn.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3sezhmvji.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3cxkrbqcv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ubhtsesl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3kquphmfi.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ovqvykda.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3mozqnmmf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3pgpevlgu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3xkuajcug.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3rpajkavm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3owtvsgbu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ibcxqizo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uwcjurav.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3drpvccci.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3klpykhyc.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rgyfzlvp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpnrzubx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3gczjckod.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3sxzkaqgf.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xxaauosc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3hjgdigwl.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3vcuckjqm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3qtpdkyps.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3cpxxsldc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3utptdaja.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkfgitel.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zlhgldes.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bfosjeyd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dztbipnl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ecmejwur.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqauapcf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3tzpugagz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3odereare.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3imztyxgl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fasdyasm.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wdunwryz.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3rpmsselc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ubyzxsji.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3fqptdmbt.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3muwrwlvm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3tuiymlmx.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ldqlrabv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cwbofusc.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eudhsztm.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uydoasmx.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eivbieqd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pnvrvdef.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rrsqoavt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cgzdomhu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3wsungupr.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3vwoulqkn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xfyrpwwi.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eiatnsbn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ynqcibsf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dkornvxn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3wlyqkmsw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kvrlaqzx.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zsgndmrw.html


<!-- 参考信息 -->