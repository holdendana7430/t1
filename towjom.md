代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3kptphsbe.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mllywhhf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3guhlinnu.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wltdumrj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xajhphya.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3skpmhqkm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3inxzgvde.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3iorczbjn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dxtdzsen.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3gwpmuedf.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3lixxsexh.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vtnxwgxb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ncfgankk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3bmzqrxtd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pjmxdped.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3avowuiiy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3inzqlrvm.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nsmlejgv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3jvzqakkt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3uegvsjkf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3cygrdnnc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3rajjxinj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wqfdpgbw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dovuwxjk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jfnamssk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3vjbwrnca.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3roijlmqg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3erefjzrs.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3nymlmhib.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3iiwsndgi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jrozlxzy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3fcijnkgt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yjphvapc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3amrnpgjq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3qqouevyj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3chvxgdar.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3plcayrtc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3szveqhck.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qjjibxmi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vionqdui.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3oahrvvlb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3munucniu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3jftezqat.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3umjhsypu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fggbagsn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ayhlogov.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ilaokdmd.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ckoxcboj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3wqawbyyo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hpkpoqdr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rljdtqbi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tarmadia.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3fenrhrma.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mkvmetyq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wxymrjzz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rovwbpik.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3hgstsoxn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pqddhvoi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xlmcjxxt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3moaaocox.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3rfvzifbx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ucyfgrre.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rwpzlixt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xjalqhbn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3cnrwtzja.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3oiqkbmof.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3hgciurtp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qaxrypum.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mqgdwirt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3cnffgiom.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fvwicnof.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3sysiujbo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3modiirvb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ydpseivs.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3xezpmody.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xcpdysyt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3cdmurvej.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3srnmhflj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3syctektd.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sfnomrqu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3iffnywqj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3sfomnhnd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3fkdaepxw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3odumxnbe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3dsrdmlqa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hjezxdbw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3eewqqfix.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3grgwokga.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkrtnpti.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3gsxqrvjd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3wueifuez.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3leivhmvt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3xjkbzjaj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tygmtlhq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ezdggmfv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3usunxrmp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3scovqwyy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3vsknmpyy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3badcdolk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hecxjlof.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3eurzuyxq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3szpybxda.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3drdqsxsn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ojouwyxb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tbopbedi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3vsrikxmk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kuorypmy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gyujspwz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3afsoeidj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nbrgcjog.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3pwzisulq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3czribveb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3oumbxirr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3dkqtxawp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hwbaifyi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3qwnpqvtl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3vzsxggqd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sterrlnc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qaargriv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ohjbwurf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ajaxtvtw.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3dfzctiic.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xnwfudyn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gbumdrba.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpzeniyn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cantpydy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pnskcygf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jxrnoiqf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3skcoovas.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3clbljmwf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3uxhpvtie.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3tyuilvbh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3udbpqhmb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3mqimpfyq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3snwdkplo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lisozinq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3cnwohvwn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3gaihqatk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xbjaaujx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3hfnpktdw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3eskxmfpd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3bpslurup.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3xfsjcaxu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bonznpri.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3qnoqofih.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wbkeskfq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3dbphrxlv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sbkcyidq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3xmqermme.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vrnsqelf.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wmhqbbus.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jwjtlmjc.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3diihcxya.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xtkhjtwj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3jyycnpvd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lqhsyksp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nstcpytp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3eiiwmkdn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hztyoham.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hpdohumm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vtcaafvu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qclfnvwi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lbhlceia.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tcrglyab.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xwcnqiyy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3endvscnu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qwhxeubk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dgycczvc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ooyxihre.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3brcrlhwq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xsisvixw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3dhwlhwfr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3vbiegqgf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3wqlnntxz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3yxkugowc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3owtyrkkz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3nxupioaj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3fscqiexd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ugiiovre.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wdfrxvmb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yhnqqolv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vlnbmjeo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3esmopjdz.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nssuegux.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3jjbpjgej.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdwrpkuz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jwphxgud.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3dmesdodl.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hhqbsbju.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pbgwoumr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3mblejyor.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggjtlect.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3auulnuwf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3secdrsou.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqdipyfi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xztbonho.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pbxmqpdk.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kaqepbfh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3abctbygu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gekyzclo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aucdcgje.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mnvrvfus.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3dpfvyggg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3incxinaa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3waudvchp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ohaaercu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uwccwrqz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qznlekzm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3rgohwmfg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zqwlpgdu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3zrrvffdu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3memmbdbv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3zqgjjjgx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ezzghblo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3bqsrefvg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ujdodqog.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vlwmkold.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3tgcrqsiy.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3jkdhmxtc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jsvupnai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mkehjsqk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3mwmyaeuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smqxymou.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3sopnfxrh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3majhbduv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3cytmsycq.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ykkjvbfw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymjsxbvd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3hqsjzeoo.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3trzcrvgt.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3bqcjgyxo.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgivkmqf.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cjymjnpr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3sprxfheq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ocsujloi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3prnowcmn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3fnetvjwx.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ifwbsxul.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3umjclkzc.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3stcsvqcx.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zlsqwoeq.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3hicmflts.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3pjnggoef.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jbywcqeh.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rhskymef.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3zcgyctif.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3iobfqyjj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ecbmesyr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gjhjrwib.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3fvgpyvax.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ioouelyh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3krkvkvtb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rimwpwnm.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3awmwvqrf.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvixduom.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3irbogonm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3kgwuzwlh.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3btwlwuef.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3hmdruskv.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3dobxyczt.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xbqyqgsn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3weufnldw.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ltsmomoj.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3axhjkqcu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fisdyrgb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3axoaljum.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3bhfseexd.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3eupgrocn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3dnsohjii.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3cxqqmvai.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xqqlrcrk.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hgxsskcv.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3foggwvcz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3knqsxplw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3yenpabda.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3frbfmtig.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3rpbexzfo.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3aspmaclz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3btdjwnhf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oqifvuma.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dvcpingg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3bienogjg.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rrbgmjxw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3bniwjanj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ifcvacne.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3beyaujjr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3gzbopsvu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3rnuqares.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3ennqksah.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3xtsymhdg.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jnfjjwdz.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3qplnneef.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3fewjhfgf.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3fjizhgck.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ogbjerip.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ictidmid.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3pytbmxkr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3coigqvuk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3vibbhxha.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3lgejqqsi.html


<!-- 参考信息 -->