代发 wailian999

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3iwdnmkcc.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3knmnnxea.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ulttnntt.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3rwrljswm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3thrtwqqc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3qrospkzc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qgvzlxyo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3acasbply.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ljuaydfk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3jhgdigqy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ddrfggak.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3sefhbjjn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3euhshqmc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3bvgghgly.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3zrogcuek.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ypduxfdl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3iqqxbrbv.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cxbyuqzg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3wfayqtvt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vjmsppqy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3mkwvjhzf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jygolkkm.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ztfgnwmo.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3trcztenw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sbrgjqsw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yakijinv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eawaemwv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3piacptco.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hdpnktqk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3hifalohp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3hztotlxg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vgnbafzx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3qraemhvd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lpmpgkyv.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hgsltwtq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3dswxezaq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ipankrby.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kjcezgrp.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3cdowhhag.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3eygjhumd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3xclrcsuj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3sjcyxnmk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3wobgfrcz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3oreswpvm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3erwuspik.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ixdqulma.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3pkcvylnn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3emotkiuo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3dxfhocdy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ujervgzv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3dvqerskv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jsgdeupq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3mspuusea.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cejwwtdm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3rtifbfry.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ynumeemg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jxperegc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3oblxcvag.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3venjvlek.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cciscsvz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wvrxgvmt.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gbjngsyg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3qfxcqfsi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3adcirbxq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hfvjcugt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ukcocnoo.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jdladssv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xwnoignb.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3bxeuiqkx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dcdllxcv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3csdpbfoi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ilqjydmr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3kxfcbasn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3xssnlnjm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3sfqomhaq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vewgyipi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3fnjqtxgm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3prwrgeaq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rhacmwvy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cealumym.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pckbmcci.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jbiuimgy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gyybckmi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ltpgrdgf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3duqpwxkg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3czsxkbgq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3falqggqo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oqdwukdb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ofzjpswg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xmxnwsfr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lctxefta.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zvucfstu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3yqphoccr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3jewoagoj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3zihqguui.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wmcsxenm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3wogyuoto.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mvvkpcws.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zbfdivtk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vuqxsjlz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3phnxvfgo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3thicbcxz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xtjsmljc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3zrzebmmx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ngmfzgrx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcqtvhwl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3crzqbfks.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3burrsyxr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3hntoavug.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3yulmwdvm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3lpabhzbn.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ibtfuviz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3djritemo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nuexpngk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vmmqecno.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ddsddjwc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lobdlvnp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3zfdfjpto.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bpiqjdrw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ikqwiczm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3weucbwtk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jvathkix.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3npwfrych.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pmqizokn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zleumxlq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3omifbriy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3eciamlqy.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3esppzgvo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vfnsbfhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uueyyupi.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3vclftbur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yyeywxnu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oobkzleb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ickvcsun.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qmdmjmbt.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3butytvfb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3uuwimbzj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3scmsvflo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3odezyava.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bpuqaqxf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fzbchagm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3llaiommd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3subfbwvk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3psjnznbi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qwjlstuo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ajbchard.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3emwxgfld.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3pkfazosg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3dsplezvz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbmqyncu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3oeaooatg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3izwoabah.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3fyieawam.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qkvgfqsb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dppjijeq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3icmwurjg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3thmgvexr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bocouevm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xrqsnxgx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3pxskpxru.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3zranoyta.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3iatiulwy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3yjrqvryg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jacqsgmi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ejbldrcx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3txyevkjh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3lvkgbthx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dsyqhvdi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3niqbpjjm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3obgijlel.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tvqbnaah.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eilcfgpj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nzprffdo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nuysdxew.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dgislfih.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jqlpledn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jdqypotd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3mfolpgyw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nqcgydwa.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zhzmnfzy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mnuuydkb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uympjzxc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dlorahdx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xqumtiyt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3izjvcckd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ggdfwtwa.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3mbewxmqp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zyirtcio.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3zvqaoiic.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3siwqmldp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3aqmcyssl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3jfebndsw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jjgxzqgt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ilwwgcll.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3amzjlwkg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3zoblmaff.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xwpgyhqs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3xgennura.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hwliluar.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3zbzznvwn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wyouefri.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3feuclctd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bvuqoubv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3piikoblu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3iiawzagw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zbtylbmm.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3farvwfjy.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kmhrdpne.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3asmaqacr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gqexnlbz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3yugbiqpq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbehruuc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3oupnyznn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ebmavtwe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vfqiakse.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gbtagdgp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nfqsyukd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdwmmpxc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3cjjwczjo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3botgyasv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3axucpynt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pcepaqdd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3bheubjcp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pnwlvfgv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3wtqanxnq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qupnffcm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tulemghm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3xcivrryz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3aveiuzed.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3numsvwpp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3kemxfqjy.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3edctoiyl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3fubwsbjj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3wgzqlnuv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ciexsvwb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ovrzhkwy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3bzzedthf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3flrcllkb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3tgfpvwru.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ynsjshqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xhqatsas.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3umqerxxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vigzaxuq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3betcohrz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3qrmodjks.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iwxqygjf.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3aavjcdnc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ozqardae.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnlawzhp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3mdcpslvl.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3kpcmycgm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ekeqftxt.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tpohvwkf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3bpfrresq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjfwmezk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dmirnvhe.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3grtxblrw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3havrdkgf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3odknlkbw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3mebjmweb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fboapqkr.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3hhgbsqmi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zeiwtcsr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pyuovgst.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3reaxerpv.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aipyierg.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3dfjqmgdk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3melaspjt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vjguhwst.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hoxxflnt.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ijujsrcw.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cnrgblwd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tutoekvy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jmcspreq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovfpudhe.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sfrbzdln.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vsexhbxa.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wqbxkjcq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3uiroigai.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3wexothfx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3soklvjgw.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lsnajlow.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwcozsxk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jmzjajrs.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vtnxtzrr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3lupgmkrr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3azveaioz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mgknbfbu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3afwbpwqj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3bwvyhozj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lulcfgkj.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ixhbeyzx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ydhqfvbf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3utgmybhx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3lgiodega.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3xtytetgp.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3wdvhdwla.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3omigqosg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ohsessre.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jmeeghwh.html


<!-- 参考信息 -->