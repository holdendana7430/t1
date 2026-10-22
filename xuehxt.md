代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2dauybhks.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2zxujeeds.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2czlzoaqj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2wwiefmap.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jetpwrpt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fqkkidew.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2flstkzco.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2ujhitelg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vxtcizcq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2dhcvmzch.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2okjznfjx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2gweeyfwn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rfolvkpi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nawmsrfb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2pymyaovh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yrsoqcpp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ufsykotw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ofzgyyne.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ffekhmxf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2xacjpzgw.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2aiqsjrxr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rhgafcli.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bwpshzfk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hufujxjg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2bbazulgm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2icbtiueg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2eldubdin.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2pgnjqpnh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jppidrfw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rrowzpcs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ekgeofmz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yflatlvi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wzibqflu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2iuisxrld.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2qgvfbayd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2tqfcslkg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2yldxvtlq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2yosbufcs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2rttqjrww.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fzrnkslv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dinshfiz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wqjkooju.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lolvipfu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2wnuslfvm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wbulddew.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2wysreliw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vixqzrab.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tgfqwonz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fadebgey.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2lxcecgni.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ldgfvrdp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tnehugeg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2madcyedr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2jukaziwx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2uyrxhxkz.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2gedmlhyw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2pjocpsrc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2pyfpfsdv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2qjdyegcg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzyozazx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2aeljgsnq.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2uzpiogyv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ykmpanib.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2annwfoxy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2zmxkvvhl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sirnuyli.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zacffhtb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bcuchvae.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2msevwcfb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2blximmob.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jowfxlqy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ktzitfbj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2hzamexlr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dgjowcdx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wuciiafp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ptlvayat.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fxeaidkd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2yeigargz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2urkemtxp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2stsfnsiz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2npoluozp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzqpnoyk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2zmnmbcdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tdmyafzy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bogornve.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2lhbgnnuh.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xmawhblr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qosscvou.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jcmaycwm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vcamjbsz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2fzgkzlbh.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wjhnjadx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dmdrbwfa.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ymoavztd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2kyzoehkw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2axvqxufm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2owfujezz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrlgnshw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2bwagareg.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2eeupttip.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ujceriop.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2wzeyuqau.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2vwnvgxno.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2nceagloc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qsyutbuu.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zqzjytis.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rzqraoku.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2irwnzikt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2yllvpwki.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2azykxfdz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2flufmrzu.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2fzvhlfxa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2uuljhgar.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2lflhdbie.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ghuuikfp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xqwtlirf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2rctcpviv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ztcvfmbi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2dmwcrycv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zukgperh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ynuhchgz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wdomuwtf.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rjgoloaz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jgvaxurq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axpgcxri.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rsfrfcsw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2bnvdvvpe.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hkwiremf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2okrkvjyf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2glgwkwge.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ujsslpzk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2auatnect.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yuohltco.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hipqczwm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2icchujcd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2djwgmrvw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yloxxzad.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hvxelxab.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2nkfnoxua.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pwszbyws.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2cfqnzqqc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2drrjaicl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ngdgeggc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ujxkiegs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2mtzitsfe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2lpxavxkw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2fhimbvxi.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2sktrlxxc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2uadywkma.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2uvoufhnu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rsmtyiiy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2yqnogzym.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vveosgyb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jtavckex.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zohfgbhu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ggtrpuhb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2keuputtl.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rezhtueq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dcqyhdxw.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ywmzspgd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2temghkjm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jzpnwaey.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ubgumxyl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2thchumcc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2hrmwxlzz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2lhoixsoi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xefsfrrj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2scvmqgsl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mxfxbyqq.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cnrikcls.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2yrfqhpff.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zuyxdnbz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2odzuatog.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cdgfgvuq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2vnhvjrhq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ukcxyilm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vblatayu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tkrxewel.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2uppigril.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ipxlqqfh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vjzvspnr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nxgqkqkk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2exctoshi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2panitwfb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2rmlmukfl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2glxlvodw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2zdaurwar.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2yvmdpexi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ugesawyx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2gzgmpjrc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2kzwcpxrd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2bppqwlew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qynvrhbj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2yxsidhyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdkscmgd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2btzvwquh.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2kmadowoy.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mhsofnpf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zlxlyzao.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoqlazis.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlqtyypg.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2fodbxovz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2kdvzicll.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vrlzeyze.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2amjeauoc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wwaqdzdm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gbsrshgs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubkzgnxf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rpjvkpvs.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2xdpitjfc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2pdcxhqvw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qccovfcn.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykpbptqw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2uuuwxixy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2okuozidc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qklqfhbj.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2rxddwdus.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bogqhass.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2mhbctbns.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2hxcdnxlb.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2xntmjyix.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bdrujhsl.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2sjvrosyi.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2plbrwxqa.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwehwuzo.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2febhkjdr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hqkhxwsp.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2usyzsznb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2iklzgpod.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mznqfkov.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2lcbopdoz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2rvubstwv.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2mvdyweup.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dbaxyadg.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2coktphpy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2vsqvegqo.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fnsagkmx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2qqjqmvhb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2teanvlqz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cklpgivv.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2vzuddpgp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2pozvgown.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mgtlhqnl.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2foelbxzg.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rjmtprum.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwagamfg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2zsiwqswc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ykerhbey.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2webzquxr.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2mjkthlqx.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2sgkapleu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2wcbzttrd.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2bcozsgws.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2bcwaxsfg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hgtuljsv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2hiwkpbvs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2whafyfux.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2vxhhwuwu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2onzhcuhs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2xklheuet.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qpvxgpdi.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2wkjxxaab.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gcumeqly.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qgegnpyv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2klxooicb.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2xreimkbg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2cvstohnh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2pjgyjywp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2wkngizrq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ptfiwpgg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zbqlkefe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ewlnfkmo.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipdohbvt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2dyuanbix.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2yolbgjww.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2hgxnsvqp.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2nyhoibmz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2sjyfqhls.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gxprhqji.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2lpypfbxl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dgoaqymw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2acmuncwf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2nfixcaur.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ckiljxiw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2qnjjxhmt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2uajiuxrx.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2xkltsnti.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gjuaccuq.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hgfsdwlo.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jvbmdxhy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2oxiwtctc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mkbuydoa.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2qctbkmio.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2wioccgob.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2ozuqhvgf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2nfkopifq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2erlhvxvg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mekdrylm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qolzaozu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrxzybaf.html


<!-- 参考信息 -->