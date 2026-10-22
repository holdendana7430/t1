代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rffozxif.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jhclxzlw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2zqwuptik.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jntyntka.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2mnjisxus.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ehhpnrpp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tlofsaos.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vykdnbaf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2herhourf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2utxsoqvz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dyruxlbr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2gjwwctvz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2nygqjykz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ygzmycyw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fqcwwxyd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2gpwuazxk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2plprrfrd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2hyvtauxn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xtgrlovd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pujhsmvf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2gbnqbkjz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kjnzqyuw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jxdqaodt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nmpdfidi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2auuxxqae.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2gaovymxe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2gvbukqci.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ayeuuksi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2oiteuhje.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2huwwhgji.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kvvlkkwd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fmapkdrj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gystlgmc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2pfxrvdgc.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2komegjtr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2iussvhtb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ufijnviy.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2utvikqne.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2qwnpdudp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qpmnwfdj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2cxghpwsp.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2oyxfkfse.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2nyiydicv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2olxpenwo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2woqpduzq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2oznyjtdn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2adgbknpk.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2slgtjusx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2updpaiyt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2cxgppdbm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pljymufp.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2zhpqldio.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2dvxchrlx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rfnuanjf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cpcirnea.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zscxpivz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bakrbsmm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ttfjtnlm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2hlybpwio.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lnxuvejc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ylsszqvr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2eyqhtjqv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aploayyr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2buwztein.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2chrhsdmv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mlgswain.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2kldghxem.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ahqhcbbq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rzdwfqef.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bbeysexw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ldwnpcfe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hutirykj.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zqpsazcc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ujkqvaah.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zpiltqfx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2sartfhsa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wangwwxf.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nzrowomr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vopxkhot.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lhwwccji.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jaurwdxv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vyfjhdvl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2pyzrargt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gzfmaumx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2apavofrz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oambxyal.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tllzebhr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2uorsttxk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ysldmgzt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2dordtjmw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2vqogjsuo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2gsyaudjj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vedmghia.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nqwcucve.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nodgfnst.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2cxwjpxmh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2yrkromje.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qbdfkqjq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qqrymyap.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2boarrfmc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vlevglqu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2pqhvscxw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mttrdfmd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2syvcrvon.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2lrewhicq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jvnfwmpi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2tzhjdlgh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ppuisjpa.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tthgersw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2soixywtv.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lpvmoiwb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2atfqwifv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2snvygmai.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vaoxhifv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2gqvbgwbd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tlklnpyu.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2utlmreer.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ppkwfgug.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxompmui.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vfkmawur.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzjlkhyp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2odprtljp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gqjfuvrr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kwoxzsmo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yshpjups.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rhlwkawp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2rcxhwprj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rqgqhdjg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zxexecju.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gkegkkwe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hztgedko.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2qhwdwygn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2tfimqbym.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2vgkegwep.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2mlogxdxt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2eseefibx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2touwgliv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhxeoerc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mkpmtrqr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2orawzjbo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2cxprjqmt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wtwhxtvi.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2hbzspalg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2keianbbj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2bpojwuuu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ngunktmc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jkqlxbqe.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ezrfhqqg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gqkqpbhm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lteuxaue.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2nauvrocz.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bteqajqu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ckbmfzov.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2tubaakzx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iclhgrlh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2uaipobcj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yxfctfgb.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jslnyhqq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2gdwaqikv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2csmonlaf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vrmilytz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipfhvupc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2fcqqhcxb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kiubtjug.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2afeyhase.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2somecdww.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cvrmfvpz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dizznbnt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hyntwtcn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2adgnhcwv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2zwhrfnbb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ynmupinp.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2oznwamqy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2vytuqhhf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zbwdhpbu.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2uhexhrdy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2iorskbhe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2saflyocl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lqsexelt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2nznppgkb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2usbabgtz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2eanrppkk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vbomuaks.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2mpcxklnl.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2vvgyhqdf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2fijzrzfg.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmamlilh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2icfevhac.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2eoifzulw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ylwljfgi.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rzllkqam.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ypkrdwuq.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2apoqmfwq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2zmkqjuib.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2wkrtmyvg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2huzwftck.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2ycyowzur.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bqjpwpip.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2zdiccnkx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vmemxpfc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2srencsvd.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2auyqvbsj.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2fnckzbce.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xwtnnsnp.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2euaulnek.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2llfquieb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2iyxhygfu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2dihuilhf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2owkmhyvg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2upribgvh.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2fffudvnk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mjqmdgir.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmtostsy.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gwzvivxx.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hpiozxgd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yvgsjeje.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2vobzrxsk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2tcliyvqf.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2dpzvditb.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ffchzhbn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2kzxqgewz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rfukxfhz.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qfunqtam.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pemnxvja.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgrflotl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2kdgqtbrz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2szsozjvw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2ldcugvky.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2skntiobo.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2btvuttsu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dnmkpwyg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2hubdixvx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pwbeloym.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bxznjygz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2elcsiept.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2owptfwru.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2rfrqnekx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gqggijxl.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2jdfrpkxu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2qpbrfkfn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2rwhwuuph.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fpcdgtll.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xzbkxauy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2yuffvmiz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2jwhmrzso.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zbhcsyxv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2qhegvmqz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2avbrhhhl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2vrqyspsy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hureqalr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2gsvylcil.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwetoptu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ihdvjycw.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2ixekmjpk.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2uuamhbci.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2hvfzcikn.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ovaavwhu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvponbie.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2pyxygdjy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsturega.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2wjlfaugy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xccpfqde.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2tejxazyc.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpzyseey.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2cestuvbb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2fcsluoia.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wkllybsf.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2nizzfdns.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2futottiv.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2norsmscx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2pkvsschc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2sgaqmrnn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2tqwljajo.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2odvrnwoc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2pknignza.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ckgregda.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2gizjeehw.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dxzusjjn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgfxjjqb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2kawmwszk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2nvzqrrhs.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjmgiwih.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hczrwykw.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2mbimuhdj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2apvmybtg.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmctoolv.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2szmdxwjn.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxnmnxpb.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rodwgefm.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2hzjmcnan.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2nqzkxzoc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2wvjtgoyb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2zvragklh.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kjwevpss.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2atidkeyf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dsntlhgx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qxepenpb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ulzpkswd.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qfcaannc.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2yxrpkhoi.html


<!-- 参考信息 -->