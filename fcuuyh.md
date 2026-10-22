代发 wailian999

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2efxjqahk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2zmspnopp.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2ktwjyavk.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2swzeqwyo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2gaorprbh.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2fhaetcuo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tcjaiyqu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2tyjytqlc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2twuyrghf.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nkfwemaz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2oudekoqq.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ctnajcfj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2fgcamgxk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2cpaediob.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yszyqbfb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2moiffuwu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2shqadckz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2pilhrudn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2anmlmvcn.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfafpgjw.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2hzdpvnar.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xhiluypp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2shrvdjem.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2pajpxfib.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2phdiobyg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xxexqize.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hzxflrsy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2kblecdah.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ewsvabjg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2vjppsfxm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mtdztxsz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ouyfvxwt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dzmgyhdq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2tkmunoog.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2nlhzndtp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2yhzzlspe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2tyasgfew.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvterpxw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2dgparuls.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2otkccdqs.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2lugxplxn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ghsxyemr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cveoztzs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2xafogiwt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2zeviunpv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2svtozyim.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2utugrxra.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2iefoslca.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2endubves.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2lhauqdyj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rmeeotuu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2olvbbuhj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgtxssoj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jhlmysfk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2hrsfcabv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2clsftxct.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ykdzqlyx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2stjarzde.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2jzzkwtjr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2btfthewy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dfvjcsvy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nuddmzsq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tivlqxzb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2oymqatao.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ryljtsnw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2stjghouu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2cperhsda.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zcnzlorl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2kjyetyui.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vanezssa.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2arssqtkk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2eevvhmce.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yogvqjme.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ovvkdnpn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2fskyjfgs.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2yppfzeaf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2scjuktwy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2uecthapd.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2etkfdvpi.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2soriilgo.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ibpompwl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ptfwpkkz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2msuwtzdw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2igdpyxay.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2mogzxvfq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2loeqgzzr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qfdocntu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hnwqohza.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dvfxsqpg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2dudxlfmw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wbsrzjzo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bynumrkd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2rruakxsn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2wccyhiuw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wdykunie.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2oujpspbs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2bxfsostj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kwzzdvyn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2hytulhgi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2kmbfktbk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2glarkgjv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lmxgdjqe.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2pplbsieq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tthorojx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2knxunfci.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2lcygnsls.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ccoxflfy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2wbcryoxx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xyyxcciy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gocikzhc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vborcxfh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2coamgovv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kihdpidc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2rycfzovx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2wnacfcym.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvtzrpop.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2yhsxnbgk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovhplizc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2aezzlucv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2yyxfskfb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2iajdrcis.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pawwcbsj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2uqygkrbh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kyflyhiv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ngwuevzu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2sektsqwo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pcnwahan.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fqkzclxi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2upkdwbzm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2haltguin.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2berkpzml.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2iypxyhew.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jtjlkyrp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2fqghwvzg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nsodbwhv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2inmwdzru.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ufvrprgh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vgafrktt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2jcklmihr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2jkkxxjex.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jwizrrmk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2tpxrzcqy.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pwbcsgcn.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xvgguxxp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2illxnzsw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wrdqeodc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2iamqnwmz.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hdzqzefz.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zmcnxpzd.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2mlmbdqkz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2watfghvf.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eynukrlm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ddmdnivi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ajgfpnij.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tqyaulij.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axfzdgbl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kydwtfej.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cexyvtaf.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2pemmhaep.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vqximtwh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2dvhubynt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2uzojblya.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jgtkrhkc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wxpufjlu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2vbnrsrys.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hlkujkbc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2tkuojvyh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2nfxwizen.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zamywfat.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2extjiouu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eoxyvkse.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pgpepydk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2idwrlvlz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qjyjjviu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2aujtsfxj.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2bjbapgko.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2smcenmzb.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tzztgpbd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uoejzkdb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ehnvkkwq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2treseudn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ownbkpag.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gwuvkfhu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vrbglrcf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2jzvbjabg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2rtyiarye.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2afnedtup.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ixjiwsyn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2haaoohkx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hljpqkml.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ifchcbdy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rolkptem.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2giknnpmt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2forpcpbf.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2arselfzl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uyhxvyob.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bwgesdnb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ryonvqfj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2grgdqnqc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ygffpoyr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2chrrwtwk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2blgoehxy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qakrwfae.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2rhxdcqaa.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2mgdhvdrs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2yxyyvnkc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2fmuaqabz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zkcupkwi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2qdhbccls.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ncbiemsa.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ycabjoab.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2thvybjma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yexidpjb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2vgbdhkys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2icecijib.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ywlevtmq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rtxbdvow.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2qffpzfgm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lobufcao.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2bxqntinw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2deprxbze.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2yjcbjuvz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2swsvslbe.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pgsnetje.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzjhjtcr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2tvjotvni.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2whdxlofn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bomkuzed.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cepdoxeb.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ryiowyjv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2nhxkisji.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2yviqrsjr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mjrlocss.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2lhzluone.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ybfdkhkp.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ztcsbdxo.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2uggscsre.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dmrqmtmy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2bljqxtwo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ayywndtc.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fikzdlbr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2xpvaiwuw.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ggrjlfub.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fidxfwlg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2orwvykiq.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nriodfpb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mrubpptr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zyipdkzz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gckqkjbj.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2kenznoej.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2tsxqbzdv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2ijspxzky.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2topwnvil.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lasygoeh.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xlrsshuf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sgcklzen.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mogpsnqt.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2hqipckif.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2qkgevoit.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dohmeggt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2waqefrko.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2qqzwejdz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2nkqtghub.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bctpdawj.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pbzvwohq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2cabwokou.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2srcqvfop.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2wlvbbglj.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2durmpneu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bflfwkdm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2scnvzzhb.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2fmmfukpy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ncfslrnh.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oyvvkenf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2yxwzyulx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2byewgdhm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2repdewfa.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mkznihei.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2lnmyeurr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2gbzktnub.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yrzjgqpl.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xjepuxkx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gzxkupaq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2xyvkyqya.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2dzmkrjwj.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2lpvtkhpg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2oqvjclvz.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2udfsxxfa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2oascvuji.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2mjdevcks.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2lznncpaa.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ftqpnzhu.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zobxgqay.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2aymrflij.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2siufcdut.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2dnigkrpg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2vtxlkfbc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2hvnfmkjo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2slcayajp.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2nvownygp.html


<!-- 参考信息 -->