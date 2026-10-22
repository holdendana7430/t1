代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2mvyxyksc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2kjyrqdvj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2rjrwvcsx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pkcjlbjp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nfsttlmx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2niwffdxo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qyibdccf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2hbzhywlw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ftrybpjj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2aycvhtmr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2lgeubbvp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fbvesykg.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2hfjsrejo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gvsgxqjf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2xeqmklsh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mpyzhkzq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2uzfdesqn.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xnsjwmpg.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2vnmozsdt.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fifylmxb.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2imvintur.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2noyxwmoi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bbadniif.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qqeocybg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qfukfkqr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dhxeozce.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2geuigylz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kvslrfbq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2bnywvvyb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2xtlvqltx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mevphhtn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hgosyggt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2bbrmverw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2miwyakct.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2uvmvcoae.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2yjvbzavy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qxicjnow.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2umlesqks.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2aqzjjybj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2kpgyvsen.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rvzgmlee.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zkqsycwg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2gluhmacs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2udngsqdh.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2cuatfsxp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2csazrujg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2mmpnacuh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2eapqkplp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2stvvrmuv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2nkcnxxda.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hbyebokv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2fwfibjlb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2unduhmdv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2bfccclbt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2camyiexq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ejusqneu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2cyipdcks.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2skamgzth.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2siwnissx.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cairnqwe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rmjphilb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2vwanzpcf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dltxignk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2xmoobtjp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ydhibjxo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2qccnebbm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2bbgvvvnd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fcyjtifm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2smdcsqzq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zexrzjwo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xiewuahx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zbfrizcw.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fuekbzxy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2mndgqmnc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2nfdbhlqf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hhikveaw.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pzfzswlq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2yaydlbzu.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2jqmfjdqk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sragwnlg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xmbhabib.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2hpyhrjud.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zxsqdztx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2vrknnmkc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2coffmlxi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2jclumbpz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2pwspdtvr.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfprrjvn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ihlkzbht.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2dlzjyfwb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgxltbtp.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ymbpiijh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2uvfiusba.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uodfeddq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2luwvalrl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2nrupbrpo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cgnktpcv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2jznqqqck.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pubcnikx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qkrylxdw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2gbyvvrsv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2nzldriyf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sdquuwow.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2izromlrv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bqvjyojk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2xjjkmabb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2fexttonx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tdhmojfa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2blsgaaiy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xropkish.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2hxtbneey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hbibtnqs.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2tymsbtpp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ohetbwro.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yowsgjwg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2iwawdluy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vsbsblba.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fdqsumjp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2txtbwncp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zigibwyd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2byvxvdno.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2yjjxtwom.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zpqabaoq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2oupoojpp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdpxlxgs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2svxvsvno.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yrqvcanq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2oljssiyu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ientedwi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2upztjgel.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2asmzyrcm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2qsgnyjvk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2djzvtsxw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2rpslvknd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2cspoaiop.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2uxdwqvix.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ikhrbjxs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2cvoicphi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2evcxfwbw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2wqrwexcp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2detgunpc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2caeggzgl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2odwygbvk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xicjjgjb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2xvhknkqe.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xpcgonzx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2qnjlibiq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qgnwespw.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2yccjmtoy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2eqphcqxn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eifbooaq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jfeqvgrf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bjsjwrby.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2icvjtexi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jzfdwert.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pqcyjtlr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tgdxjvtj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2oxjfqfsu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oqgxabge.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tgjjblgv.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2awedxwst.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ahgepmzb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pbvsjjyo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cgxolpsb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cgyolkoc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wktcbgjb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2voeuvhtn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rauanuml.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2phbnfsjt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vvypquqe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2erfwknnh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2hkiutvlk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2mrkhlfim.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2vpwqurqg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xlxdipje.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2cuwlxlaf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2wijlnwav.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ucowcwvr.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lwncurfp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qqknscwt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cphxutye.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2zwhflwyw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2nvpllckd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rufrfwik.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2efsossey.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ieyuevqv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oyqjpbqx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gnbdxmsc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ldqyqbpz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cxcopyyh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2pphzfxnl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rnwhmtja.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rjfgrbvx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2cvfberkk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nytqujfy.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hnedtjbe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ezkstkkd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rheariqa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2qwjstejx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aemkpgrn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fsqmeepn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zftmyjvr.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mvuafjvb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gevbeohg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2vqppsjih.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vlktlepw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tgawmtwu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nrrbpakw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2xchawlwr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lcusxpog.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2yfgaoiqm.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2gcdlrlta.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2uzufbeso.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dzqifihk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2tbymcido.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2trwribkw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2yldtiymc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2dhhvfaxu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zhpsqiuw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2nxnbovdx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nwtxwdri.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2pqordtbz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ooqrhqpv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2uuwxgqwi.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2ljwmevrv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2crxhyggu.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yvzauyuw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqhuwtym.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2szhcxbpq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2mscgkvso.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2zyniunvc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2twmoensd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ubagofnv.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2yuctqsvh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gvsflbbc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2uuhaplej.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xnthdghg.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykxnmkfl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2yfnugaxn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2epyxadac.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ijedcxep.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2toxqljyj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2liheqlds.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2kydbdgks.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2cjxkbpes.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ptguzxms.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2lnzmjffp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2isdousub.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2czsrtbzc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2niauixij.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2wpjcmvnl.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2dxxgwrvc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2qtdldsof.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ejreoior.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilogugbm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jpcivtfl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qbbzeyfe.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2mofjfanr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ohtooxwk.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2gcyvuiio.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2jtwvkbqo.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkehrazr.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mhypyxhd.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mbwrqakl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pbfzhhdy.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qappqimg.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2jifqctie.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2zrubojxm.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2xbigotel.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2xsvzyktq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ijgpghhb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rlixjuaf.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pyckecng.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zokxytqj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2yyocxhwi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2qdjkhqig.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ewppvxdk.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2vjswrawo.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qnnxvvbl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ckxprcuw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ocpwckwy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rlvxjtux.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vshjwzkq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2rnofjqap.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2ygamielk.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2tfzeezad.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2vitkogex.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2yrzthekr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctmdjkom.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhsjocax.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2rclejttr.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bgxmktxw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2bwrccpsq.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2joyzlile.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2mglkmfja.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2udtidoek.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2miaifwqx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2opetvmca.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2jtjpqlef.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2thyljuzq.html


<!-- 参考信息 -->