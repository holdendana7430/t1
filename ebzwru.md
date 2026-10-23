代发 wailian999

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3euayqgzy.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3fsgvmczt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3zoqkpjvx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ilijqwhr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gmlrtanm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3gfjwdyep.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3nprakqry.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3gyyvfacy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sakriyqo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3imhweuov.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3viqrdpwt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3jmcntcfc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3bwclqred.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rlzhbcak.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vfrfunoe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3kilrozpy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3rtofifbh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3xnletnky.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jamlrsks.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dcsfkgag.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3wutkwtfh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dkkqoypp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3drwtkxdh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3csdavsul.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3pelhzduo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jpcxtlwc.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3jtcqcinr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3hqqgvjgb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3wfrawwrc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3xtpqavsy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cufhsaxb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rgeceupz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zjtkqwhp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yoydsavw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vmghczmx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3tocdakzm.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3xwrqcwtx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ubslpbeh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3wkozuddr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jvmfmlmm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bqzhyeid.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tbpnrwsa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lswovflt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3htheyiff.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3tgtqkgwe.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bwetcqir.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3fpwxmguw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ttodowjb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lqakxabf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3sivgogog.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tzvwtkyj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pqrrcvpq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3oszljqpk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3krnbxrlx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3eyzgbsjd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3glmtsthk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lshqbkzd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bllizxxk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3kejuyove.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ojcfhppa.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3tlyhgyxs.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3bdccdxhu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cwjjkjcb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3cgivvfio.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3lbhknxaq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nhdhqoyf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xglbkgjb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3thljusoi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ibuisxwh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3jmvlwcat.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nvfirswf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qlbfcejf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3imbutzmn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qxzhgqtb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ocbsfhnn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ruucthod.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3otnjxocp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3tqqkohww.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3rlqiltzb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3cvxvvkst.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ysuynhsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yeihkjju.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3afejoqen.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpwtrubm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3mopbregv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3snumeeox.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lazmypbl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3yavvzdfs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3kwjqbrlf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xbyfiaxu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3kmxgoahx.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qfiufbkg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lyyudpkb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ejcgjklp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3epqoqeiy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3oytwzsbr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zkkmqgvf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aldualnx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zkldwxlc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3hgymqztw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3oszuaems.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3isarrzcp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3hrnhjmfw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3fltqhcwb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lihtehyc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tpiyicob.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hujewhkq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3rkbhficz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3hwqgylyx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3myeelkpu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nzkyqyni.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ammqgpaw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fcgeokdc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3rjxykpmb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gtcgaapw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hfwgeczn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ugaevddm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uazhplxz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3cbfthgzg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hiovwrnn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ftmmoysh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3yyifedie.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dllsfrwx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pepuzedj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3onwkwsna.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wwkmzhkr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3uikqokmd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3isajkiub.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3thnicuxo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3fmppcvzl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ovqiaybr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lpxjwqzm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbuamnnr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxtltnry.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3prbzbweo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bbbmsyun.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iffleemk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zqlynrnn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3lxszzqcd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3spvunbax.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3xnaovhwj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ubzsmswx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bwdnlbjn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ruhopkfc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3cjgzboor.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3prpptcsv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3wegkmfuh.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3zbowysqo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3mzfnhnzv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqfjavie.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3eifszzws.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hfdtzwcx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qhwistrh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mfndvgfx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ueyygaod.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3svlqnxvk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3vofxdldq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ukmkvuqk.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yfipvwva.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jrkmsvvj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xvfybcsg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wcaocclm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3cicjjvih.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yefkrdgu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3iytqufux.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3gbkuxcea.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwxjavzf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kjhqtnjg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kemrleod.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wlhmxpiv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3nmjshjxo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gliiswmq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3firpugvv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ezbyefrl.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ydnvhncu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtlbujah.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3awheqpca.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fneigldx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3udydqjrx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hdomhgkb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3nhumrdqe.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yituewky.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3uohldcdb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ikeodzlr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3vsasgkxu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3rzouzasw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3dhofilbj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3pabnkksk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3geimrnov.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3nuapztfz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3nfyylvfh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3lmeeqdzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tywrnkrl.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3onrgepyu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ygrrpxhl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3deiapuug.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ldgdtphm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kgwuvpkg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3etaanlfe.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3dnskdwnu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqazgnqt.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3bcltuuvo.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3skhmgola.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ihnosmyg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zptxnzsw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3vgahshfp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3ouebbkxi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vkmxdous.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vwgaeyeq.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xpdhdtmz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3xnteddzv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3pzlbexta.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3plzsbept.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jhmxtakq.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kzlflelq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rztbgidt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jgyeersc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3chhwgney.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3tktgdryn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3vibikzen.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3purfmvzp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3uklbvudj.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3gajvguqc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rbqhjipo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3fzyxrvhs.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3feybjjme.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gtnjkdfo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xixitvjx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3alkksygl.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3pnubgvck.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zmlhgmse.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3pllcvmhg.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fcyofsay.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3arlxbpnp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmpbfrfl.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3elfdzyfj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wkkxmzhx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3kwifzaxt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3hjzwfimi.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3adcesfdj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3jtyvbtzq.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3gcdcrzyt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sbmhygjn.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzebozwe.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tznmytkm.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3scfbjayz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ykevtpok.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3vziqhzar.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3wttjscre.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3uscjkhbk.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ydczcxks.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mwwuoemh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ulzjtvui.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3rvtqqfhr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ojgppint.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3yndrckzg.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3eulmqchp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3ewescwzs.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3sxpajosr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3foslojhu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3fuucqthn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3iruubepf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3cvstnmgf.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3cklhdhho.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3qznsslhf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3yqzhcers.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vjszjaxf.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3muuzhbog.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mktktnwv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3qtsslekj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3hukrcnwd.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrhxxmde.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tbolzsjc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3abcggear.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3njpbumos.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gqivqwmd.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ebihvwex.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3yezkonhk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wseypkzv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ehkclbit.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ajfeezkb.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vteckkpi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3isojkble.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3srczkpbz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3dpqbewip.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3pwazifdx.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3wsthrudj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zetqnzxh.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sdotvgdx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxypkaui.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pcywluod.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vxktgnqe.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3hwvmbjiv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3keryjhvp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3bzxovjzx.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vaewvntb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifxonxwq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zuxxwmxl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3alcckqql.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eroxvont.html


<!-- 参考信息 -->