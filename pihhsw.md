代发 wailian999

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bpsjnugn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2fwdkpmvx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2omyackdb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2eiigfltn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2xkdyxmoz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hhfoxcgx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hqgqpugo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vjhuyaqv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2eoathfsy.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rfnjzwyv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zoojxfup.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yngopuus.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2eyqvoiqu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2hvdigdmr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2knourani.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ssaswtgu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mgraagms.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qhyrqohd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2bnwhwbhn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2eknojzcl.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2izgfecue.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nlpwujnc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2mislrhuc.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wsiqqirg.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2recylufh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mxxazlax.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rglodikr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2kgkxzfhe.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2xhtyshot.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ojszupao.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2fgyuobjp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2uiksqjaq.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2dlimadpq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2lrrrdggv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uzlwmgcf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bzhqccqh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vaadnbhm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ciqiloav.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2bjynfvmq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cibbjpps.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2audpxano.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2jbjfxnxp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kwjtgknk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ijtysptb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2tilbuwpz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zgbalwnc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2unjpdvnw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2rdqayaww.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lgrcivlv.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2jkliyufa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2xabivbyc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2gydpwzrz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2buyjylqv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2qgpmexyb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2bdupyjsf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hmhjghsh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2zgbmthlu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pdlnhqsg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rsmnyzop.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2zhpspedi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2joktfmhd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hnzxaiqh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fivkkddx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2edshylej.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ikuhfwpm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2pqrexyke.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2lbjngtas.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2lbrzlqum.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2gznrepdq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qhszjjth.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qquyzpel.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cncuohru.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2bgbjbmtn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2glyylvir.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ytyelwgk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2eqnatgnu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2smhavoyj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2iiycjkwp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ieetohrr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mddvhsun.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ytcikhkv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zutdaimb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nmqadogg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uzmvvrkm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2jhnkrdbn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2fuswjyap.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2uyiwbvtb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mxuqqvns.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2pivjoohl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2oqjgdbqa.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2pvrypkrq.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jmkvsjgs.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xoiwjzvb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2naehkhng.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2gwsewyoe.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2vulhsaac.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2nxaniacc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpqratql.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2dgnfesxg.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2khednzld.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2lvxuhmig.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2nqeqlwaq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2blrjqbvh.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2wkdfsvcq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2llsnypwi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xcbpqpdd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hcrrjphs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yarpahgq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qlmccwvq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gccarbvl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tkmpznus.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2juvprqio.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2axyiqzyd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ymuczhec.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rgmsozol.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hchcnnkz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fyjotsgq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2yqiyxgwd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2vqktoyop.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vvgolmps.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2xxtsyzme.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zxrpkhna.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2tqmngnfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mphsbbnj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ojsusrdr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2wmunvrnp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fotryshm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2uyynignl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lnceytnl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2azdfvhic.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2tcaqvurd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2edahachw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hqreajqz.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2nvhagplu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2oiwoiwge.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2alpzvvao.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xaxycavk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ibsndlqq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vgohxiqo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2sslcupaa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ygzhqkur.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2azaouzff.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2zfnfuhld.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2yodjgpem.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vftrpycd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dvxcomcz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wpjdltjn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2kdkqybhb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2jdgsceux.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2twhdrmau.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kmeranau.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ggwxahwv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2drrekkua.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2nqvxkoxe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2aodpxgvm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kdhhcdto.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2zikqinin.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wkpdshry.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2trqpgxxf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2rwcvhljw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2zqmbtabk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kakapogm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zmuwisyd.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mgxeqive.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2slyirbsj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qzcnlnqv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2mthuiwna.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iceikaht.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pxmfpueb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2admxkgoi.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwdqdicj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dmrdckwx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2prkdtvvi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwqqgaxo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wrjaqdwk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bwiqhysp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vsxbljhj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hcyxmsxa.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qhxpuyxj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2fcqrlujb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2awpupslo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2wuogdyvg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nfnozrfv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fvdwaqqg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2svkyskqx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2fawdqjgu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2kaqsgmti.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2yarwypuj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2fkpdtezg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffxpzeel.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2qahabeim.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rcywvigy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qawbeqzm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2nexdkybd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vlpvrofk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2cicfokyb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2dazmnbhe.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kvlwbfaj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gfmagpxx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lzbwsuwo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fufmhgvd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cpzgmhua.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2iepdbsmv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zolitefd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2uiizqnys.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ligblgtd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yykocesk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ekpoyagu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hcgurtcu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwbwokzi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2tqioxchx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hpdjodnl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mtwyeyfs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vqpsruze.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ndhertoy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wgiwvdov.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sfbamqzh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kmuwykxv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pjbtalaz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cfdfprcz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kycsoyiy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2weromzvp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2veevylry.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2dyzkvxde.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2yrdzxyca.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2xkrpsvsw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2fipkhenp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2hpogpjiu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2jnfdcttr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2bdsqmfon.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2srjdsgpy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2bojojhju.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gywrkuvm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2czrbrhdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bszbsclz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2sofetdeh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2lzikawqt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2wpwcexan.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsjnijru.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2xddimqlr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlmierpg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2pfjaizbt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hyyanwkq.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2qviljakg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ovzceazx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2mdpnitrc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2qbovcskj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jcajzrsu.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2urweyugp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dfflvrqz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2llzdwtfr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vuhpskwv.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2agwivijh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rllakvjr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zdmqjogu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2jmruncfe.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hviyxllg.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2eabututg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2qmnxzrhm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2yvuxvinn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ovkwamyc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aablsyyo.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2wkadgiul.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cdlpfgeh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2fbvvdnax.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yteebolc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxhxfcnx.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wcttzplj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2knxraymp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2knjhjnnv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ykkqtypx.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2dyyqvsdd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2fxhwahvo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2britvodj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2bcenxswr.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wzdnoasj.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ptljhufs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2sgidyrcz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2mdsoalpr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tnfdawnv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2gkcmmhao.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2wopsyhhl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nhnwbwbs.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mxrpyhta.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nisbhfri.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cjgjkfyo.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2yjpvzrhe.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2wanderaf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2vammfbqv.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2umqgzixf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2arpgdwfl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2frgjpznx.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xrjrxkip.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2iesvzbin.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2puambfcm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2hvwozeay.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2eeksbogq.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2sezaocns.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2oqftwuoq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jgnrhafd.html


<!-- 参考信息 -->