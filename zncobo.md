代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2duxlazun.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2zjouljbj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2vriqqewt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2izpswpvp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tdmuqnkm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2hyufoobh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ojtuskha.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pthcnlwc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2xvohwpbd.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2sweykwyv.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ddsnbbus.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ewixoqic.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2abmmndzi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2oqbpraob.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rtqxxewu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ylvfnlfg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2lywqwkil.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hhdknrgg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vahkalmf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2iarfphgl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tedrdkik.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2anmvkwzc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2oedmnttj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ekpyplwy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2edqptthe.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2ngoiikzu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2somsydbm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ovnzhipd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ekmmkzlp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rrakfhas.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2rvmbhwgh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jeehnhda.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2wpvcowgw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gmjbqpvj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2trhuoafl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ovgffeoq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2qkcfnqhm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2odzyfxyw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jjedoqdm.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2tuuuifct.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fpzmxsqa.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xuwapjoa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ejrbwgmu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2rffjygkw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kqselpls.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2erbjiepd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2pzieagwt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jmiewosl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2koyruhhf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2lmmygzpf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2lsolvjsg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2imloqrfn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2okdoddma.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2majapxig.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2nendiuxk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2dpduonew.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2auswdmmt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2yajkvaoo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yixmgfbh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2aqgaeahs.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mafohkvp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qzgefxzf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2obfxbtca.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wbrcrjhv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hlouhgjs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2fupkpfrq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cswhdiqx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ebluwkzm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pamyngbn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xogkpkge.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jjnwpmdj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2fduxsetu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dhfjgrlw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2kaxfprzy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2grzohhyi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2vxxwfars.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2elkqjrgg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gybrlwjr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2kaeuxlpt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sixugzmj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ovvszxfy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rlgtxnox.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2yduewftc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tnkdsniq.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ygcfjcfg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2uyqsqnxf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2itwkzatx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2iqshnbfx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2hwebasan.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2bstudwch.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2hbcikugk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2iuqfjooi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2hkbbfyah.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aapieuah.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qdrmfdhl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2uavwjfit.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2nqxmxukn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2bjscfsov.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2roicnmwc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2nppdndka.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2kbwxxqxy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2kfoxbvom.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2lnenaxtm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kbbrbmyg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rhhlvpww.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xpghtjvy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lcgyfioh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2withwcpo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rcxiejtf.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wshijwji.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2blaqttjn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2obgrguwu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nxjtrndf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2cozyzwtc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2gjfbguoz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qhalyfri.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ingvmneg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2kjbrykop.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2vllqgnee.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2pjkzhayg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2xryrinpe.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cztyuqjp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2srogolwj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uqmmwyae.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdnytsmo.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zgneckhw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvtetdqt.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2iqssupcw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2eqwclaxh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2klmkclbh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2itvlrrtd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bqwgfqdn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fdlpducm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ykopcprf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2byufnynt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oykeiuxp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2pvkzhkjb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ecsnstbl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2minkrrxy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ktwtcfxw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rsgvdttk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jojqaylj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2nrnsiptj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wfxfbmau.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bhjfrgop.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqcxznlv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ztyigqbv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nupbcggz.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2czpawrdm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2tuyrvgbh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ohqybwfp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ajrjtntl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ocdwbptg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hejogeag.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2lxqjqzxe.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2olwfdbdp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2artysxeu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqnhokbu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ejgkzrro.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2uttjxepe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ujbfbgbv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzoqyxcm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ddegxzfn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2jpyjhcct.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2aazyjucb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2uqzezurp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2ikdarkqy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zvztycxd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2igrfptnq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ciemdwrx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vhokcjtx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2pbwgfaxk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2lffhuuzz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wpjjhtmq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qjemveqg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2flrjwagr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fmdokjtm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2gshtwdsh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2spwxqqix.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ylbihmnd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2dqxtowzz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2eskfpnev.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2profjhhy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tlptkngy.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2gypocpqp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ycqqukyz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dwwvsvry.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dhudwrjd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jcpqwqdg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fiwepubq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2lirihbeh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tgvlrwmx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2seiascdd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2duxdqaja.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eqtaiefh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2savylbul.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cumyiubu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2twempwkl.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qticdurs.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asgrknbg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ysqpczdp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fhnaseck.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2nvmzortu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ztijimwx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2sqqnthkq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mhukwtot.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jyomdsbg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2mrphjcua.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gkxeaddz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2fiemdgib.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2jabhixfj.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2nzosypfo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2sswiliel.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhxfejjo.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2linvejcq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jmaxrhku.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2nlycyibu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2usxqmbal.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ogeybmgv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ypgkspln.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2lnecunui.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nalmmucq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lazglieh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kkfnebgg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wswpqngb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eoprchty.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2bvzhvjel.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aabfgqck.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2duhqhkgi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2yxfwmtdd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ccorfyee.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hupobzpm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yegjxcxb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdvyuiec.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2azbxscoq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zhyrpwst.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ydctugsu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lrakkzip.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2jsprtycw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cptxgnuo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qhhpxqir.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fpyosfuy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ksmyjpsf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2fogcgemn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2bqdzktba.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xlyocprq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ijzolfuh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2sakxoshe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mxgglrcj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2waidycwj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2zkjqlryu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2oqkbetwk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2aejqfkwo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2dtynntbt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2djnsvbzu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2yoltiwga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrjuovdt.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2qdeupvhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mskkwnzf.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ehwzswku.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2dbytbzmj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmojlszq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xqpcpcmz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpiitjng.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vteqruuh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2frfgccvf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2rfmxhkor.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2czewjemm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2ufbkwuxv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2tkqapwkh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ixtwzdui.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnudfkwb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2sbwlorlh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mwbnukxv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2aeysycub.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2laktnbaf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvxnicni.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2fudjanze.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2oopzewjs.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ftccjogc.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tavlnads.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ffeqgaog.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2jgtpgbwb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2budbzpvo.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2srwnllue.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ijagdfbl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2hpbqddcn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2jggsrcvg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwenljkt.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipqeggqh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cferzjju.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2shbfqtjz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fpkitsij.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xqetzhkh.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fgbriqop.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2qmusnsrn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xotnvwin.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wjyrllac.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2toobfgcy.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uyzsijfb.html


<!-- 参考信息 -->