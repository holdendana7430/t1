代发 wailian999

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zspmlazj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fczumzsu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ptukauui.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2efnyzbdc.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2stvsobsj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cfgukkrg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2znnfwbxk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2wgayxkls.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2kscaysui.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jeehupnx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2apwuphnd.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2fogdaiyx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2yytjnukb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2loksjmwv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ytaqfnfo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlcbhlyq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhslceof.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2fptumxgm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2sxjpietx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fjqlbflh.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2qxmnrzit.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ymggeubz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2xuuacpeu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2lcxbygew.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2oombsryt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2zrefwkmm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2mtomzxzl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2iwtkkpxa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vreeszfp.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2bvnndfnu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mbnhkceu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2tyudcgjh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lthepsgu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2gsazehhe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ioofbjtw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2gvcvwexz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2inoiccxs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pvnzsdet.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ljvorxia.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2aaiekkcj.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2yttaibxv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cagzxjis.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nszlmpuu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2gbbkebsc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qaghijvx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2iwicvnbr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2jdrolwtx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2vgxhiajs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2tunfeaye.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2isbnjjkr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vfydcnoh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yisotthc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2andagvjs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wiitlwzu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xlixhtjq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2mlysyadz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ejnibeqa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2qwhqycad.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2rdmwzizt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2szqigxey.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fyszesyi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kskjyutn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iwxgrmla.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ymjxjphy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ycsrzdbc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rdudcbpp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2muordeaz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xyqwhhyg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vtoigkbn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2uaihevib.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2tjjlwnzv.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dwpfqyko.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zlxibrmx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2zpapepyf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2sanbdwoo.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jczoggzf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2oytuygwz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itdcnumg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfsqrccb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jlejnjlp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2qnjqqgua.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2qigyhcpo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2cdpxjrdt.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bwqtxqqo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2xrbrifvm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ihobidrn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2elusuzjy.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2aohlwiiu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fxdkvyzj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2tbmalnmf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xekvfion.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ottddzdt.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2eogoodkh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2dnlcjtqw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wbbdlpuj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2iiomzevb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2umaxnuzx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fgjcysgu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2anabyyyi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ewefxabe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ocynnisn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mniyvpqo.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2utwurqwy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxuycsdj.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fnvdsnuz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2oklpetmv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gfjnbgkz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2trxeulho.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hchxvavn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vurobdxv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2moprjfia.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xrxeykhq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vulaoktd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2cwngklfi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jsxifhej.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2svxkzxvd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cmdcuwvo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2umbuoujd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dxxlkwak.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2eoatfxmc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2dzolmnkh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vwdfteeb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2etqvyqqc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2jubnhszf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vorujyhf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jrmhfsje.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2qbpqahjz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rbszsnyx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2dtycvmzi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qztzxwct.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ewljchqr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2wtcgdumh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vkkhqtmf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2xbbjvpdr.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2urhzzvos.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2aecigcil.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2iqksxecx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zxthsvtr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2uljzxnnl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2cjrpnblx.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2dnrkuggk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ubnuingl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sltlqvmm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdaxnfln.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mzptlwjf.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ckmfupvl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ewcofwms.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2weqvbwjk.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2enxqjdea.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvghxhwn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fyklzpro.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rkqwbjrq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aubvjabv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ctfzsdmy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fpitwqsp.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hqhwwswt.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zzfwzuow.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gpgpemwb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2rhhmfmuw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uprftcmv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2gpkmreuf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ltknwaal.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fgfvuiov.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2oirwrqqu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gpdsgmsu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2pqhilljn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zdieokdh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2axhgxpob.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rcarnqlj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2gagnagzp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2aakxkwpm.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lpeuutmf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ittlfwmj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cataujdu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2lbusrvby.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xmcuaukf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2zvygzfsj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xfcekrxg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mrypnnad.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2orucxfjz.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wkgzddps.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pmlcclxy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2jbqwpnjo.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oiwazayp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2sdhujzbd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2xfovfjqu.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2opaehmmd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ksgbnqkb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbyxlubk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uylbptpy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2zhysefit.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kwcxxezr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jmzoeejp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aghtwkts.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2tflfzwys.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vjibzvft.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lgtdrqmw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gmmqdhtd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nfhtirdl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ykhnsqsf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2mwaxivlj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cnlrcpqa.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2fgffecst.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2mwoysrnx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2bmljgjqa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2lhdouqfu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2uwouennk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2cksnokvn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2pfigysyp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2epqetebi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2cykxmyzh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2ztutweho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sskwvnqf.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zqnaqjfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uvzzucdg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ymoofdwm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2yovpzvrz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2owdoyxtn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yarsjihb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2lfzvkkin.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2cohpcwzo.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2bckpcjos.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2vetqlztw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yjeknrgz.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2qqamlbut.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2bujnrtsh.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2aaexwrld.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vzbtfpnb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2mfnwmmfz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2fpjgpzli.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2kcyjjokf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qfbogluj.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2azpzgssc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2vbmrasaj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2kzkvzdfv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2safaubrb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fqpogfks.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2szppqaks.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2yemeqksk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2zqtqpvsf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2detfsrky.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2gmhuoqxj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ekgpuhrr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wrwgkjtx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jkjyfuku.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwekhxgv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbrvjgxm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yycxdhgd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2sgoxuqbq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fxagdmrq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ylnyzohj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2owlogxxq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cwocbwzc.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2pmvmogst.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pbzoyqdh.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2apzatppc.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfbgkclk.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2bnvbvlsw.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hwzuldof.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2iydgsers.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2dhacmvql.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2cnoqclxl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgxzcyau.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mowlcxez.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rabzfvxt.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rnmjdqca.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ennmwilk.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2vmdnbtbu.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2ixdkgjaf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2szqtinng.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2yhasjktp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2lfcgvqtk.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2krwnwkxk.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2pogxcpqf.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gouixanz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2lbqmajmm.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2twzxcsjf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2kxkngimy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2kdinvcdm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ysttrqzz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2rhpsxffd.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ymbypfly.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2fdgwscfa.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kfuvosdh.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2gjaeqrut.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2gigelsrw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2zqvesqis.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2aauvwsdw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2hzzdoedw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2naswcrgx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2yddityts.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcjllerb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bucklcbw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2gvxsokhn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ftuozcgh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2izghybrj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2vdcbbwcx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2iozruztb.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lkmwopkv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2szsehhxg.html


<!-- 参考信息 -->