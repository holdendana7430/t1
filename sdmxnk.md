代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3joihidhl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3iaqhfali.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3shuecqfd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cjdbsxkg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wmksejhl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bbshwspx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3yufkujxy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3vipgvcqo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3usauezsu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lwtafyim.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ksarnamt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ytoscrea.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3jvumsddv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3eukdheja.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pduhiukj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3iicquscs.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3swaqmebr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3obgthigj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3jmjovrau.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jeytctqa.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3uekbduqo.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ivjsxcmw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zjjlomam.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ujsuhvyn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3gdrmoqww.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zidbbtau.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ikmskkxm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3yfnnkjbz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3zqyxewud.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3zvqnzwuj.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lzssgvap.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xileayzz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3hvtxqgcv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3agkfbhuw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ilnrkaox.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3plwwxkrf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aiqkagql.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aynkaybm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3qewudper.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nylsnbyf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3azrgrxza.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3psybvvpg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tdgjgkio.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3mlvrxmxs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ydjvdnzq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qocqhngx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3puwzgnnw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3abxngmfe.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3qxlnodyc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3qgnmmhal.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3swsuqzqo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hontbmwq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3vobocjcw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rqvemnka.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vbptesjc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fhchqkpl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3axmrdzoj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zgiikiva.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3zmdzvyov.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3wdcdvdvh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3mcgtqxhd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bhdfmooq.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dlfjiavi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rmrruydy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3wgxwobvz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uavhslxp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ozdmvmzw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vmkzvdiu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ohuoawzv.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3myzaolwz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3epurelhl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cswyderf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nmfxgbba.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3bzkcaimz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pncequdm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3djxcwhfq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3pfzqxrbp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3qrdpfvfq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qgdnxmvt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nrpzhfzz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wpkxciqr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3sbglsmxn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xxqgyien.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bxpvczpt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3tqsqsjge.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mnuzbxdd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3insrgjkr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fidzfhwa.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ctewavxu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fjukaddd.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ingpgegs.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3szxekrhn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3yhjosvhw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3bzwlxaoz.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ttmjkhjh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3usrhrrxo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3zvkvxqai.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjyxosdo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwfribmo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eodzihqr.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrshdnvn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3paoetxbq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jxtndeor.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3sktrubcr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3wclupteu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3czspbzyp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rkwxddjk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aiadkmzv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zqtrwkzf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3mlhetdtr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dgelenbv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uobeztco.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3qzyxnaub.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3tvtvrpkb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jxmibcam.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ttgmsyrj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xobpuvkh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3abtaihyx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3fbfutefw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xspyguqj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3avithyri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hxbucaqr.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3hehrxxob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ajpkiohs.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zmynlbqq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3zvrdohmh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3finabjdy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3sluozotl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3emdsqvsg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3sbtmfowg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3tcboinlb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rsmxjvvh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nmcdngdr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3lnzdtfyj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3npmiadpd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktbmomva.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tuffepir.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rodigulc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ccgjkijh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3lmbdhkar.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3pbkkkmhy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3wswoairr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3mutvydam.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dgbbqkoz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3cegrqyhy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jslsnrlz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3uxlnceni.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3pdyvvupe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3wgmxefwy.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rdvirqbz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fadyavss.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3vgcghwex.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zsczygxv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3livrqwjo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3flwounub.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uhzuzyif.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3rymkunvg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3keagobyr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rrflkylb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lffbjkdv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3jxglsops.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3qpjdlocq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dxzvuqbv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oolsirrw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tqovokiv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ikiesmgq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3gklynlao.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3exipohkd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dlxxxtpe.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3icqgjpll.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3idlymssh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3txikbzda.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nfrnkdlh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qocyehqq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3naqvhhdj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pmgsjyfv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ewjltzjk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fhhipfxn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ilvwinad.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3irwqlhqj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fficajwt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mgmhywwe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kgionnrf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mnntrhgp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3gpeayqgn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ncatoygz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3khrxfszp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3trhvhyqr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3fuonmcjd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqyskjys.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tpusyuqy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gapvzmxc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3aehltvwo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3fzixflpl.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ojotgpsw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3kidcszir.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bxbmtlmi.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fhwdcjwb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3odxdnaqc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3rqvgfqem.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jzsckrjm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3utfvscps.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3plxjibyr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fntftxdu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3emkceebt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3injnbavn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3thenamnk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3awtenzgj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3brccxlzt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zpovqqlb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ogskooui.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3unudfqog.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pppypuvz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gywbshzs.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3rdfakycb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3myscvmsp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rvatpfii.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hdfdsnlb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fzgfduuy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3khonvdpo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3igmssetm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dbxmyhvf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3fyapknuo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zeyhonke.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3cwwlozbw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ttugixio.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3azwtcbea.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gznucrip.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3raykwwpb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3puzvhezu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vtrjpxre.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3mplhhmhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgfegmjp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3rbytkafc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gdtmnnwb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3negjdmik.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ulymnyxz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnzujzfz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3svbkyvis.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymxvqrsq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gdebcjlc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ltsvcknm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3sjpfnxow.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3liyikijw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tjndbhrk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3jlcjrklz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xsrmmxdp.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wxjuvkyk.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tiqrrmvb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3arlzzbjr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rcklwzzv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ncytfyeg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rfckoseg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jalayodz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gqqnmvpz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jqpksbbi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ijouelam.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3dyudfebd.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3fmbxdzli.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3dhxokpjt.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hxglnewo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3dgukrqvs.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3dzuzaewm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mskhmtbd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhocpiwl.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jphrjbfz.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3vmplvneg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vmdvsyoo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rflsgxvv.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ccjweybt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3psqgexyl.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3uegmcebd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3bfqicgqo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jubwmwnw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3mgrorsej.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mqdikfmh.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ujddihoa.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3hgnklsbt.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3cydaksoe.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tiyzyyas.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3utoqwxml.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3vkthceww.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ytnkbccc.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3djqzwbuy.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wizwwqvn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmkuugqc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3odybxbwf.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3kazkrlho.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3qvhsulsj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3tzmjafiz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rpsvgfka.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ajxkrcvl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3waamunep.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3geuijryv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3tgorwnjb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3thfnqdzd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3dtmjpvtf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3obtsxxaz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3gjttcgyv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3ythdxezp.html


<!-- 参考信息 -->