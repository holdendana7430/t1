代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jwgdjzwx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yuuuofzk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3gbkndbyh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3piihtszv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nkrtdxux.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3kajnwzef.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3grhfothy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3uwlbjmrc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3lrwlqtct.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3lqscjdxl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3zrmiyqmu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3vgzjyilg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xoizfxok.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lerxriri.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3qvdutmjj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3fvpupwbv.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3azsturjp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3fpntroao.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wlwkbpbz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3bhcenlzk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3nakzqcys.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3obhfirqg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3epirnekf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3lkvurgzl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3yqtxyfqe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3mndjjtjm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gxnpfsfg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3beahorho.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yuirgden.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hodvihao.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bkclmzci.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3kdvjwtdh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3hrpaftww.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3lixickst.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3hckqkgnj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nlltsrhv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3uucyjajg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3babudfdn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hmkioyap.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3opdjsacb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3poppvqfy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xinmgfod.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vybcqgsy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cacrvubl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3mpelbxbp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3dvfbyvbz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3wueqlrfv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3nrtssfjm.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3pfycpwga.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3srslliqc.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wvvodjea.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3eovogxli.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ihkewayf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tqxyfhao.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhwzbpcs.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fuempgeu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsrxxupk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3yhybyyae.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhtzjata.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3yiahkjta.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3zxfbynap.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mrkhhqnx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fljkaxmv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3aqoabexa.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ozobmmcg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3fflixmqr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tbgikqrz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hdmltatb.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ijeiwejp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zqvdkesu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gagojxkf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mkprpsaz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3sfyekltt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3fabqmimn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3zwclbjht.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3derqcxcz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mxhshopy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sqfdndyu.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3pawwogez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3btrccnlr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3efkrewfs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ybbtymzc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wrtbrrok.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3dxopwijq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3hpgofxzh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vzxkujlt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3hlizqlai.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jvpftnfa.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qtfyueej.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3wcjsclrc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3irchvpaz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3aunisfgw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysidyknz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwmljuwc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tconnabc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3bgwyoipt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3yrbjoynn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3marhtije.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3mtnljbtg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vgdyvxec.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xhqntmfg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fpxybllh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zrvzjimb.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qhmcourq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3rtaicriz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3nldidlwu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bfqfmsaq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3fvvinlml.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ilywmljl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3mevxzdwh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3shetrucp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3flwvwwcg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3cryisdqr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jqocjylz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kanndauc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vvetdkah.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3yktfhuda.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3yjwbjlnv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hghzaqtq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxjefoeq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bhyvohmq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3alsxjhxp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3yyucycte.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wgmbpelo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cxiqjitf.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3xgojnjqa.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dgnhkapg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ymzcxkja.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bivvgrsa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xupquudu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kzwmyhcl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tgvpokun.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3slwpdotq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pcqeuotx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3fcnsieub.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nnpnfitd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yaowszlg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3bfmpydiz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qzfkjekl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3msokaxta.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qflbaqam.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ouzzajnv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3adpostkm.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3bvbpatoo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cagtahbh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3rgrjftwy.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lylosqbm.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xyzyokvd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3alxeciov.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vbveciwg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3sjihajje.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lwfwuxsm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3ukiocpmv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqagybbe.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eghqvsgr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yxyxzdob.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3joeactzs.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bzwkgydl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3dnfsfwrw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qgposmmm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3umxcqlwn.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3dswdvvil.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mshhymsj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oaggghmw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emkqdgqc.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ialvfipb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3onszlblj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pemgzcwd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kdrefyfn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vhpbnqeu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3uywsystg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dbxgqcdh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3nhgnfpcc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zqjhnehx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qvykudvw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tugqgbhd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3tjixbkxq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ekiyhoyu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3pkqyjuno.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3howoveua.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qtyltpwe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3xcskwolt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3jkxsmktk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3zexlflgk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3vdkisfrd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3zilaehit.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3lrfwjwzu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3jewiyjlz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pbwhdflc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3dhrogcth.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ermidcuw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qkbhnccz.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3sqhcmkmp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dwdwjajz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkhkcvpf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3tzsitcnt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3yucbqgnc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3lujnuufd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gcexhuic.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oiauokmi.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3xpqtiplr.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3rbussgcs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3qahvdaej.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mnxntuqe.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3snaopmsx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jxqvrywd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3bybqlvqu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3bfwimtma.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3friavvuw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3thkrfyot.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zjimpilp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rzyoxqpy.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3lyplvmgh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ozcgouao.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3wpzjbznb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3szcneimv.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3sthgnfko.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rugzftse.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3vhsrxxfg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ivkvfcra.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfltonzl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbuylvyb.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lvwfnimt.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qlvrzjfr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gprlhpht.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tsppawgw.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3npmkxtyn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ujuabfdq.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3lcxorinf.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xntpchup.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kalfemew.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwnbprco.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qjgdpjoo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3aeoooumg.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3yjfwatde.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bixqnamu.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ejsxacbq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3oojuibax.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwvdhxpo.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xlmbvwbc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3blyqwybo.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdwltbpg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3meclltof.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3bqunizoz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3lbfygrlq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3eiyhkxzj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3papiutft.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3feyiurxy.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3adyamjrz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lhepwdzp.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lseqisag.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3afprwral.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3bnicuwws.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3rrgtsabx.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3bukjlaqv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3juymbguk.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3yqtyhtsm.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vogsekox.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhssdosk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3extwfmhj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3rxbnilht.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3gvfzoeyo.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3babdzrwg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3saqfcpky.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3frldkfsa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3rkctltib.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3yiaajbxf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3taoicvbp.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3tyewrxcp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3hexqeuso.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3fkpqoyic.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ixejswcm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ujzzalwa.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3rypcxlil.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ojweusco.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3khrilvru.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nvismatt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3cuuayixf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vhxmgwsn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bxqqnsdk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3gephghnc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3aepcazoj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3qrjkxlrm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrjqgjmr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vudnfoon.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3svmkqsxb.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3klmycgms.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hkrjovtz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3slkqujzi.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3izmukscy.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3izjqywac.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rnovqamv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ryslsexx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkhnxiqx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxyildsg.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmfqvvdu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uoyhkecg.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3oqjuxnvw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3resseikr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3wlwconov.html


<!-- 参考信息 -->