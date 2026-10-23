代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3lemtlmjn.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3aqpdlsil.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdlmlrnm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aprdiica.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3irpwtnsv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3chuurywp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3oyakoqtp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vxmhmcud.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3pkokxknk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3rsvgxugp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3akiquvjv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3lssxqsyg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rkahcbzi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3iiwygauw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3dtcrjfjs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3tujvielu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xsgxtkzn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3jlxbgioj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3upgfeepq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3bknarbdk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3zbrqhisp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3djevlonj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3nbaypdns.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nklzcvvp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3gnwttuwm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vnsxnwed.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gcwemgoa.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ufqgvvgj.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3tivdxedu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3riaqdful.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jcrvwizg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qorzrigs.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3kyiegrok.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uitukrty.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3fvadqoms.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jlgzvhrg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3tmloefjg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wvmrugra.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pmrprhkm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3buxbjgxy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gmwrlzfo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3nfcgmjtq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3okfyujcj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3wtgbtcfv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bdbibdxb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3hyigmemu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3xrrwvrxi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zxclmalm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xbpnlqmd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xqibjwox.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bnkcxsts.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3tmlpbsrt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3wjlfoetp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vokegsks.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3twedbjzo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3xcewedef.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3uwfbyven.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mpypztxp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ejhuzhfz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3kioghesn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3xfqnpmmh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3eosgrlpm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3msfilyoe.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3wfdfcbwx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lszcfoll.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3jekyegdn.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3ebqwoqfh.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3blgnzxmm.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3xeumxamv.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3dfqvxmgk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqfnngit.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3kvaxquos.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3lamdppvm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gekveeqc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nicpkpah.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bngckdtb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3reniqzrt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3mmvobjur.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yxvxzivn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3efqwizvz.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3jfznxzyt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3oqljuwbd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3fcolrzai.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3iweuotua.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3smrelsop.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3tjnxwqru.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3bmrygite.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3aenvplcn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ejimmaev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmjyelhj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3trwhcqxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbaznysa.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3igovualj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3lzblyuts.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3monrahab.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3cksoiwee.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tnlpnsbt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zjwfdeti.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3iuybwqol.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zortsquw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yvikklxb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3vyknvnoi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3mzbjxdty.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyrpzyrg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3euduhnri.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ynnyqggz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hgyatohb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wxpdorrb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wnzypjwm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3lnxmrntb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3sdbgsmex.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3cfcleihg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3myeikbam.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oepqxhzo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jirepclo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3tipvqdus.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ffpnxtih.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3buvrdtvw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zssvusak.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3pxrfdxja.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3scyjvxxv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3yiyvnzpx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mscncauy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rhifelfp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3sptefpee.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qgahzego.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3llvkseao.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3iwmdrzuz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jreuakhh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3oghsrzhi.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oyesclvj.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3idzvqliy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3knfycpht.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dmyhptvm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3epbjxdll.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fyseuiif.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3alydrqsx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ieeuwttu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xdmxgreq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aviuanxf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igbrmlgh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oosufdvx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mysqzuse.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uqebsejj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xgevoyie.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pkyloloc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3vcojxiwf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fbgboflt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3spgkovva.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3phdtqtsh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dqlplzmi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3jzjjkcfw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3adrqwoem.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3uulrgyjf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3kfdztyvz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3hwvjbnan.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3intjaxko.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3zdrrwpqg.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3uozgbzpl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3scjjrvzx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ieudrswa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3igpreegd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3cbzkanda.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ctmbmyox.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3kajivyqg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ordqjjhf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zrdybjyy.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lvogpyaj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mbqkihbp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3baxlcvfr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3igzttxfa.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mazvhzzh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hdununls.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3kcenmpdq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gswarxzs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zpafqxlr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kowjeijm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rqwcmtfn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3yfwdegoh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vfptpthq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mtsegdbv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yakbujeg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3eydizadq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3omnddvlw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dawzfpzn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vqgpuwsh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbsbneyv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3myptiyqf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3zbxmjsgd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3snoieysk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ehudepel.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3rtvzvsde.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3lxbwqifk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ydmpuyzp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3tdfejupb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ctsfgpds.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3itopqwzw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3rzyjnurx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3mpmnjkkz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ikzdrlob.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bzgbpujf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3mvsjhrjt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghlqmhru.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3gflwhbku.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3vnondezm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3oieyzksf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oiysxyps.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3yvkjbnqa.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ekqhfmmx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3kvthnbxi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3kmojhtsz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fasgjwoe.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3elldmnza.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3oaabbsdu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wfwrdluc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvjvxbhv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vqhtuwnn.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uraeyuls.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3omwtxmsd.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3siyurqfg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jugqfsfj.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3bqhmgzrj.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3jkaxhbpc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3illxqvte.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cjrxravs.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3fzyekdoc.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3omkzvcrh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3vuuoetua.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ntpntsgu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3aatyrfbv.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3mqmyvvlh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jpecaykc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lthipuxz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dlvandez.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxqgtvme.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvounqfy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3bzgcaaxz.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jfvjiitt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3tesihyrc.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zatktawi.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3rvhfwuzk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocrbfcqg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3cqldomqm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qfqbwlbh.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rlrpeciz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qxjakujz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ekrdfmyj.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rmvxijmi.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3czinnssz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3bdbnrszu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zekiazbl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3chyrsehd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3hhrzguwe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3utkbjial.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3wajfrpod.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3fwzdsqyq.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3cyzeirsd.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3uizbbadt.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3gaqtttfg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ytiqrznf.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lspvmhwl.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lyiuqoua.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3eslthnei.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ualsmrmr.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ghtiztsp.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3idntgoll.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mtqzhagz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3urahztsl.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kckzmunm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rxtbrfit.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3hfdklgtm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvtswche.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3zbmruiub.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3mxajtsap.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjvfzoxz.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3bniakcyx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3urvbbnox.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcvbucdt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3ggnonshr.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3yarviohn.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3nerqurzu.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3mudwztqi.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3fctlulvt.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3fyxrrout.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ehgsbzca.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3rcjeympw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3qbzrdowx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ozrpsvbf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ffjuqabq.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3nsupohdr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vsshzmhd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xrgovbtv.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3prkxmwjb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3rvohypua.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3cdkzedis.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3trvqmmeo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ijczdkfu.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3phjubnyv.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oifvkylr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3krcratqk.html


<!-- 参考信息 -->