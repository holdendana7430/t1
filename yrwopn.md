代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3raoewmmh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dpgbdxws.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mqjwmwky.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3dxhwvlhx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vclegomc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bqlxqdik.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vzbzcxun.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3rgwyfoec.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3mnvfbgev.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3uwfprrdd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ytorhrex.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3xmhgqnbw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vfaequkt.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vayfskva.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3paswhfrm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dpkrzvyq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3inqrpueo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3swgoaklu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3yhbprnrh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ppgdtjfh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ldvzbfui.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3wjqwarhf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3yulferpd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pyyqznja.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bmqltlgm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3quqxalis.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jyjdtumb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3rwvgwslj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3refvpnyr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mpxrifhl.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3iqapmodp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3rbvwtdyt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kxprbdvp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nnbzbyil.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3lwyfnysy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ddyhfhhn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3gqnkjque.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ynhjbxhf.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3giikmaot.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3mbgyqfot.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3bbecmvyl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gxqouqgo.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcjhweyl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3teckdhwq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3lovlovzi.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3iktubxpz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3mofqwkxl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3hlnwlqtt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3curyaiib.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yxygmbxk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hfsssdzi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ifjftrpd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3njbxiyoo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3vecsewwl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kadwuxlp.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pfeirgrk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3lponayds.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3xdbpkfim.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mzpnlcyb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ngxuzvkn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3hzkrwdef.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3rqkyafll.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ribkqjum.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3makrwitw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3sduuqzsa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hetsxdvg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3unpjytlb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vvsyiwle.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3sehtkdty.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3fcrajhpp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gduhubah.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jjowjupm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yemykrzn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hshzxpxy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3cbclglvy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kfhnnbej.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3utzlzypa.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3hjnhxhii.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3pzkenlqf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3dknyyzct.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcashfwr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xqwdanbd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jmixlqaz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3feziguer.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3iiukgsrf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3aylsljxr.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vzfrtlqx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hfwribfs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3gljfgskc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ohxgyhqr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3doajggij.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ylznpkla.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qyktrykg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3apandelw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qufnlmaz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3bympwzsk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nhsvsljj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gdnvwayy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vzlvdrqx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oouyowag.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3cwvzazyh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dakgfmqg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3bafmuztb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3iylpcajo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3kzttokiq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3fdoswwzv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hqyfadqi.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrkbyrqj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dxvpitfv.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xvnncokm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ppjhweza.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kjfhskqq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjxmlnio.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3dinajpst.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mbrlstyx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ujfxrcam.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sytlaalb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wtsuibmv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yipostfe.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3etcpgyie.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3apqcmypl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3irehwpnj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3egznruxh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3mplzkpnw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nnywwmzb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3enafgisj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vvjrrpdb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mxyhwmqb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3lrlctxnh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3lbkgxmsi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qscltlnn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3bmjunogp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3uoghzwuy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3hdndewlw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hficmpeb.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3wtnxlkyg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fhfruuyf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3pevpbiho.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aoedlats.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jfennrbv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3lyvqehwu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3moyukamo.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dxvadxbu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ajxmfksr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3sjkudgkh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tczqiwfd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3tnuvwnvh.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lvknmlul.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3rwfytaji.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3tbascpdm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bhioefrq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ltymvqyx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xnfbhidd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbkwsrpg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ojfzesfp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3beukwnta.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sjoxdccw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ezokuloz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3gbwfnzhc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fgjbfuam.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pakdwrws.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lwvfrxuk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3whxtoqzo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pxaoyemx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3eiyorkjs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ukmsdggg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3lhxdloso.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3vuuxuszb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3yvvvqaix.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ugufimil.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3dxzijvoq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3gvyvqaft.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3cjzlytcv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3jlcsrbyn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3niprmmgv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3cxtvnjfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mmimvkhz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3scocxwpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hgbpfocp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3jkfsctui.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3mtrzuydp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gvjjmmbn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3fzjhanqh.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3lmcvpucy.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ksdmmumk.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3gobecysd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ksihnrsa.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lzxwootm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hdtjxaag.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3zzafsatv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zovhxran.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cdglpusv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pcmaebyw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wbfmiugf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3maeuwrik.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rrupmgqu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dfvomyew.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3cguifqhq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3xosozdld.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fqqjeorc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3yqofmazl.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3uqxvktbb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zfcejope.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3pfapblwr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zekgsnsh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3xhifsnja.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xvkafqxd.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fkqidpbc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3tkqcjxfx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrsuhrqs.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3npralifo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3llszxoay.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gfxayjrr.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3anoaqhuv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zxvsjhaj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ynienvay.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fufsthsl.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fhurfdso.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3whcoeuia.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zdaehaxb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fhzjtwaw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3mainfgbo.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3spslcbnk.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3qxigbucd.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3avvebztw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3xqxdyeye.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfsdcvpl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aibqiukp.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3eksywazl.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lhidshzw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fotcrhht.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3hcsqivsd.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3ewunrmal.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3udbwmxok.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3nmetntok.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dwzerrrm.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qzpxdxfo.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3lezkzjdt.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bgiymtoo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3vhctuaga.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3klilzlsj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3cssqlbnn.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3faqvndgv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3hqsyaord.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3lpcyqqmv.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kowxklxk.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3cuydgcsv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3pcjnyurk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3bglhhbgu.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3oxvskuou.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3szdmvmol.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3tbawffbo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3imcrsxaq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3oghexbjl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3gzcauwbm.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3oqxzsgks.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3josgsrok.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3nychrvmt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3lhjfzuty.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3didraksm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3muoelhwr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hwwmyamt.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3fcjoogho.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3zcjgzcjt.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wnoxznsw.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3vkvakmgb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3cjpvfnbv.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fyunktkb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3pzgqydtb.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ivdqqxgm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xrlwzsyq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnrhnbna.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bunyalfx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cgpseran.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hxaaoaok.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ppxpjeaa.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3qgaznitn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzjwfuaw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bsvcwfxc.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3jrsukzsp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uekfokyl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3jnshcgpm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdfwarqj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3dubejaxa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kfbbwuqr.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ebfouxoo.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nnficqss.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3mbfbyppb.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zqceymuk.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xufjqajg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bkwelqkr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3afawbhiy.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hfvpxndk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3wwggwwrf.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3mxgjggee.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3efwizlpg.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3gcnainhp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3dtgfqojm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3dhfhlcej.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3xtkzntqa.html


<!-- 参考信息 -->