代发 wailian999

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jqsqlpfa.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3tfauvjct.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mraflzhi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3letyrjbn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pimuhptu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3kakfmjlm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3fvhvctie.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zguyollu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3sigmuhrc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3vdaqntes.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hxdgkstg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3jwpmvjuz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ejzmwljr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pwqbxolt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3arflmunv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3jqgthqmb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wfxmbhoy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3iriucoov.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3czyzqttq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ttqlgaxj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hbaoefyf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3hkyswero.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3yawogtck.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3apthlrug.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3wvxrwqef.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ntanevta.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3efobjuay.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3cmeixhea.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3utmgtxbf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qmkavotu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3cmztqxdl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3gehnxicm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3bhrlfneo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3oirkzdmf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ilthjgtc.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3jfzykjtl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3iegesmcz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3kzfkofov.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pdoxmzdr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ciwidysj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3csjnoihb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3odivxfda.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3qpozarek.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3yxeordvr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3gxrfkgjl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3yiksjtov.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3nqdneftn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jeycgnte.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3amvkxcre.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3abotvxyd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fptylcnr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3xgfqdyvp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3sbrwossx.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3phgotjty.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3dbzjjljp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ejnabqyh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3xpuvagoi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xmwhedqy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sdeiquor.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3djbulaqz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jwrxsplq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3cnuvuxot.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3vziqjbpl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3behkcgqg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3edbdwkjx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3jejpeedl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3lnkgokal.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ukaxftob.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkcefqjx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3jlroethl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3vlckhora.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3bakgajyj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3ygcwjdyj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ibagvnlc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3uqzjeegb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3svymsbgd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ksisxpsf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3kaymjcyk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kfrxrazm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3pqtanzqa.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ffbgnmae.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ooqozljf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3apursjld.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3zlpqyuab.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3oviwoknb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3sqgdusml.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3cuqyadhq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3wqudkaqf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lqphqblw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hrwwyikp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3esfwheic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkpcxmre.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3iysdufxl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3lascjtqs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vrmmowzf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3tcseasur.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3esvvxbxf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3petzqdon.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qfeviqew.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cgqigvtm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ckpmsbfd.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3dvcjxfco.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3rktxjqqe.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3tllsieva.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmmmhaqc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hkeavtid.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3skcoifpu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3vrukufik.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3giitvgnv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3srivsoxo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xigtertr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lfthdkdh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3beohrdwt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3inwmudkn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lureyrvr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lsusocro.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3mrxvbjil.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ybhvmcpe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pbyjnevy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3duqkmnkq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uiricmsc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3uepfncps.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3riucqdkw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tqlcygzt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3vpegugeh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3semjgufz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3cjpskhra.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3reclsmfv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3pcbssvua.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3scuaomzz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gaszeeqh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kjqyzbwg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sssnbgbr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ulqcqftw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3iykrersw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tdzfgznr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3meedcjtr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3mgnmkmch.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3siwuzipm.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vneorrii.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aheqtqup.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fystrzdw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gyfwqdvu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3guvacoof.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3umtvyact.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aieyxrmd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ahchrwxv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3koofabco.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3zvyhmeoa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3axawkmyi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zpljkhyt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3oldnuizv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ugrrxczp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3vplceyvj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3rudsorll.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qojolewy.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3lblsrapv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffzoidmc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3guayyfce.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dbsgjoaa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xkgvyprx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cidqqwkz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3dklioqlo.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hpaqjdqi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wmpikicu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xivruiki.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3khwfusrn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iymivkbo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3dfdjtymj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3obpzpcya.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3yheaigpe.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzsowsul.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ryvkoqxc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3qrgzilra.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkgdqljr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wbghtvxa.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bhcfbuuc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pssjdamf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3aporcdlj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3amzzhrei.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zvxslitd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ubvsyxef.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3iqbvcqig.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rtsrvxuf.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3chvuqezl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bcaacelc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pwsudenv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3gfjxcuwb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3safzoago.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3btsmdnxh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3nppcvaak.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3cacmruet.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3nukkgczv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ovemoren.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3glcpfyef.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ononwjcr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3txfylywa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3oiyapyvc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3kdljufpq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3bpsnhwjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ghqfxhva.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3gicytqvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ssvttkau.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3yrlufeyj.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ecdupfml.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3bgrpaexe.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ptvjebum.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3qfjztcyt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3xyoydskb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3erdnwwha.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3brhnokff.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3guqgdbcp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xrhzqgnt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3hpnoqjtz.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3xtdkplkr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3acrmyqgw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wrpsuejm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3rwlxcpec.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gruazqxa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3txqsfygr.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rffqjlzh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3tvodrtjz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fidtvndu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3kadyuxre.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fugboazu.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hnpjkopo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ldwyapqv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3wvzthkag.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3skgeblvs.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3cdrzwdfv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3pgdluvfr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3dfnhbgmh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogmuunsd.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nvngqhji.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqwewtoo.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3esdzhlli.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rebucrjr.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3idegovpr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3vpiftpbx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3toiqjoso.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hunzjvhg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3pmrygipz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zevtsuyy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3urdzfmip.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3aydttwvr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3kpzvtuiz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zqtjamzg.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ciflxnvx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wawmxdoh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3fweuozzo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vjlvkgpq.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3nysfhkms.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3smdruqeb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3eelmtnga.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jvydzcta.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gidwomje.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3yiaxomyj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3epacerjn.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3imjdhibs.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sgrdjpki.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3engblqfz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3fvgwoicw.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qhyghmai.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3slxpmjqj.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3udjrywgt.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3xehhxqfo.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3mobtegec.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3izrjhodn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3vdjkwcws.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3ilozjpbu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jyvpzvny.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3lgzrcyos.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3rudqzxuq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3snjqqiss.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bozbmfsn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3pausqzoz.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3glgscqhj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3jybqoctb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3yvdpswri.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3ifhagfej.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3akagrtlx.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3gmsndnlr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3yxzfwkea.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3arklzycx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3fbqujiim.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hldahoxd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wvwrnovm.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3grjlbvbn.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ybgzihgz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3nwikmpqp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3jffhzkeu.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vkqekocb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3yxitnuge.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3fezqukxq.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3jbwdpfsr.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ntuqwxvp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3heyanbja.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzrflbbp.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlknnynz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ksadcqfs.html


<!-- 参考信息 -->