代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vqlxfwyq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2umcqpfta.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2hhwtblzy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vrertulj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eafoarle.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2scrceghg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2bqtuqwvw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2negbyifa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2tcstrtuq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zgzneamo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2noqktkqw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ybogldmt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2vzrnykuv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2bsstlinv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2hpzrgbey.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2flenyvri.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2uvffpkcu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zqvxmlzt.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2sklhjepk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2rjggzqij.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2oodhqpzz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ohkcxcwm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2undtnrsd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pobbvrxu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2kbamwgub.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ucrhaeie.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2lkiwzplk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ufiekrwq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2bmacgjrq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2hwgoljzf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2celbbkze.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hnbxjuco.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ntevkezg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yvwdzimt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ongpkksw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2cndinlxy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2tsabasxd.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2limpbqge.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2slehmvom.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mefeargn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tpnlkhpf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vnejnipo.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mcxsdhng.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kdnfbzca.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zzccnqwc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2rrqekfes.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2dpseoekt.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2thxkitku.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2xoeldiex.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2agqytddb.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejuypwil.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2aidafoan.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2kmduvuxs.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ooafqazi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2sswiecso.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2sltdhqsm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2bxdqmjow.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2begdlhus.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bixdxdek.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ptogqoli.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kjtlhlbh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ntonjrgp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kpvvcveb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pahkdvij.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2dumyzpvi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ncgklaga.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2angfgapq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2goqmxtij.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yirkdudd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gszihsmg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2qvyykmqw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vwkijcwt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sjcsbdvx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gclyrgbp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2mqjleaki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xyaslipe.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xmmkdkgt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ybcxveiz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2defobtuq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2akczxxmo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hundkewl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2awntpsxq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2cotitvre.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fjffjvqb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ieqblfge.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2lremjwfb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2cqpcbeov.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2rhokpxkr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2gytuhlcp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nkybboby.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2otrbzauw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2orlffdha.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2rpzhymoa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ymqdpnlz.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2aiegwpzm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2woxsrhns.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mgcbaafs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vkybhodt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fxxhkavu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2pqzkhmxw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2srtkeoht.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2djtbgdpx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fxqrkicq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2autzndgt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2glfhmlwr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2gitarwzn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rqnvhoql.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dtsukjhp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2oghydslg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bfqaqoms.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2tazbmlqj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ztofkvau.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2uuimlxxl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2rueuwwwu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fztnohft.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2biqaxubd.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gqghnmkj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2aubtmzku.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2noksvvol.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bxsthzwp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tdyzuzmn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2lsfekrqn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vzhcxjny.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lucuwvvn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gzxljvvy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2siqhcbkf.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cosmwwao.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pfjyjtqc.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bebqsnyr.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qoijuxuo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ecdjefzp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gtkhnqdy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2mfgiljyh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2rgphsxwt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fabjajak.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2toglcwya.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2whzybmfz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2knqqzdfv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2pgpusqcn.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ccdlqpyo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2hnxfrzxu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2odbevofi.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2boiduggb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ppdosdeh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ygvmoopn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qafjdqos.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2gvbsxkvq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zatfwacy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2eoxlxowv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ulyssxcr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wcvewvzd.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dzjvmmhx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ixkvajsg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cqkymtud.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2uqgezbnn.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kqmxnzpe.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gbhilvtb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2pcwupxwi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yzroqldi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kddplzwv.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sjimujmk.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xzdwmltc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2vcrvuhcp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2czormclo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ohdkvxjz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pegjjhrn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2pcxdcgkp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ullotlsk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ulsujzgj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lzurqkxz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2guuvluet.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zegauuum.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2kikuopir.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2twdmuqan.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wjdvcrrz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2nqahfuos.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2osemvqlp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2uvppfpec.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2fgpduxbx.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2kqvhnglo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2howgdkgy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2oavdyiwp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2byjhrrgw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2znbmdeeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlpkwvjq.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2yrjjnfdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nriefbad.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2chznxmjm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xyazfpev.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kutcbkvp.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hbegzvbk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ljnwyebg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2atoesqcv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2wjxwqpgm.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2fbvsryll.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2yvgrxspd.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2sfklkhrf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2drmklmyo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ikwbjtls.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jfefkjrr.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2bsctshxd.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlxytnov.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2cmhrqtla.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2jcgguvgy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2imubbtxh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2qygxdjqm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cchodtji.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ilkxqxai.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2felngong.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oadurmcc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2hjqnyvwb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2jjzlbyig.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2poumvdvy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2imogthru.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2guqzmkhh.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ypwrvxkg.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2diuryhmt.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2givroxbx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aybsbvyo.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qovaenwl.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jwrsnhoz.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zdsqjvlv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ulfsfbby.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2trtsxsvx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2suhuqktl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ukpldknn.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2djstknzj.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2feuhzzlj.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhbivxgd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xwdsyxht.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wzukblup.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2oipmzxwg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2relxvsie.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2vantbqrg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gmawlamk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dyqgghak.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2otckyzqj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sscujiwh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2dxldvyzr.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2gyefxtmc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2mygeztqp.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2ajzsbnpv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2inmpxqjy.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qhiaszdl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2wakjdjcn.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ghxvqjez.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2stheaxit.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2bxkiozbd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2segjfeim.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nlkewszw.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2uwvrntbt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2asprinqu.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yhmuirnw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2tjjhbktl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbtqfrvi.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ayadktja.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2unmiooxx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xfsewmmm.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwznldfa.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2kyyugmjh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2givwanxi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2wjxdhykf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2jbnpkwgz.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2tltegsqd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2kygiewjj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2gcwvclyy.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2exbbwpgu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkoqfjev.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2khwhmmlh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2xyfwgcvw.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zsgejztl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2welepigf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mnggbwsg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2bmitxqwc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2jyjbldgn.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2mvitaiql.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2wgwfdlpi.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qpiwzrog.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2zjomozht.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzgaahgd.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ebvhwzgl.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdvwdgky.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymbrgvjh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2mxrdsmea.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2zesjuwml.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2qscbkwme.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xhzseqbx.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2edbxobfh.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2pjzwdchx.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2notxwddk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwasqkqb.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2zsqpcygp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2lamxiezt.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2jenvdbff.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2iolgwcyo.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2juvsfruu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2kqlvfbfb.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nejghutx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kjllqbrq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2txemlick.html


<!-- 参考信息 -->