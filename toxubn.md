代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2junnecky.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2icprkbwp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dwenjkik.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2koiwejli.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2exjpvkgw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aekrlydl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tzmsneue.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bqtxtyia.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2wfesoskm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mvbxqsgh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2gdbeycgo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ybcuqcpy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2avaqeaum.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2bxgcbhtp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2jmuabmwm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xvunrdve.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2nebttrcm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pplkwzre.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gamarqwh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pzreipdj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ptcmmrcz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2xnzetpqo.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xyddwzet.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2meyitrau.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2nimmnkac.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2hovskkxi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2roneplqp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pefzupbh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uclnjkfd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jeimecsa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2retthzjd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2cwetbckz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2iekvssmo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2sbnptwaw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2xqzpltcc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oqnelrjr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ijmhcstx.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bwwkolbp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2brnwfwnr.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2mzwqxwpj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2tpcxlsae.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2zrdpzvma.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ojmzxpnq.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2dlxiwdmb.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2wuzupcfu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2mbrzmldl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2xuvbotcq.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hcymchic.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ppeoibxp.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jucnkmut.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yiqusgjl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2kpyjcupk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2onqzbcls.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xbbhcibb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fayanzcn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pwqlbone.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wfklvqsg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2pxvehmuu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2syhjnvjg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pzafxvnx.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2prveuxkm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2cuxhxrqu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lvhwgphl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xinbkbpo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pafqzndo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2lumrxiaf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2qirprfjt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ftkzriez.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2frbsdbwn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uwiqprkj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2yfvnqzjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lwktmovn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnoqljdh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xfadgeyn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pmpcewtj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2babikbrv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lfcocluh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qgjvwdfl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2eohazrcc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yfnecfcw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dsmdqmmy.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2pkuqxibr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2khvuxqre.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvwlitvm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qxmpnaua.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jotrckqp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2sbsytjms.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2dcccdzcd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ynwglcfx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2rpfgkowv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2gjdmilbn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2mwjbsntm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2unnclvdt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mvimawwt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rzktgoji.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zqnxsrou.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2sstqenwf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2shmjvite.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xtaslsau.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ashegqtt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wjqqiozw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2xqzalyla.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2itmwcvez.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mppzykgm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2drkozkxl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xksoviyv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2iyotafos.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vjoapthg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tsvfomlg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2vlwdbvic.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aqiqvacu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2agbqigks.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pjbkumqn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2uofgvzur.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zlsmdpks.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aocxpoww.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iugxdiff.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2nptxumji.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wuqcnarj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2peljnbdg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2njhghnpz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2miqotvwd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hdnebqvl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fummarht.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2szosuyyv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2irvwjxrg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2yjydmzjf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zxnhkvxn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2zujfvipp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mqxyxjdw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2tqwdldfc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2kymtpsea.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2bttqzdes.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2rxcwtumn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2nawapswd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2skhhqrqk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qjolkvbn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2pkbkltmp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kdmxchef.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eargqunj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2upwwcrxp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2fdqogtmi.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2znhjlzrg.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jtourwzu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2grmyfwoz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pzwdplsy.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tffgnvxz.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2uezvsjdg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vacwqtyr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wiledzsj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2bnjnlwag.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pnzbmcur.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2wurjsqts.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2hlogljnp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fpljxizf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pkdfvdgu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2phasnazg.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jlhqnijs.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2krcnzqeg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqdzegli.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vupduqgz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjcjskek.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2xqejfbmj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wuzmuhcg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rygsxonp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2axuimsij.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2cswfhkkk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ilngjxve.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jciyfqsd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ocpahohc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2uuutuwcg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2fdhujjho.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2xwgjxfqb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2bruzamzq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jxqkupwr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fybcvfwa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2hqyfsrux.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2pwnxvqxp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ibhgbnkb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2qbcbcugz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdmjfwur.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ydsuobzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lxtqkhud.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gmefxjav.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ummpxktu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zzyuqtse.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uodyftmu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2adpqgldg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffqfwrre.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2dppryhcv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2capwlpvd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wnvsdvfa.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2iomfynbf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2myzdcukr.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2bkfoakhd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kkdkulhj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2znknogam.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2aipmufcy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qzzxgoag.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2opohyskc.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukqmlnun.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2rpzywvkp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2moqbygnu.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2afjebfjl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2lcqbktzz.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wonvxsgk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2rkyctuqz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ddvlwxnp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2uuaqebfo.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sujhxrmf.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2iybpkutd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ekxbbkhp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2puufrrvp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nmhusovh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbctbllp.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vugxolzw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rqkxmxhc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2tkcexuil.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2avsjdxsh.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hejbtdzl.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2zxyomerl.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rfistrhu.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxvbxqzf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mzvwvdpz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qbpwfbki.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2egjqehxy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2pqcieoic.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vutaxbck.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2upttndqi.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2olkywiqf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbvkttmv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mnopbqwx.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gnbtxocd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bivtgztv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2axhesvfy.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2pndwggwa.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2evjidtry.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qxscddpf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2lsabzcdf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qzsbsmmy.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2okaatoxk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lyrdnprq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2vklixbev.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2cbnkxnpc.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2stxbufoj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2dkqxzuuo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2kjtfjrzr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2udneyjmr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2yucdgrft.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhbmukcq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddjezxqd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2kguplzdk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2prlwaivg.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2wjcfeaqb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmmlvnus.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2qalyythc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2wcyoaxcv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2vleduglo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2btvlotkr.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2qididvml.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kvfoeugc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2sswgkmwg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2sgpchbvz.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dnsfcrxt.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2iukntihu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2atqohvgr.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dlqeeuck.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2fswhjada.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zyjlgkjt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2cnvipelh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ilhnfhum.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zycgjprc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2trkvamln.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xywwprpp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2jalzyvmg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qrgpnovm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2udngypxm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2pxzlfjfd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pkxsomgv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ezseaosj.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2czfiocim.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2vttctjoq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cnczxqyf.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lodquvmt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xnwgdbvj.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2pmjkimzi.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dmpjqcvw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkhapjen.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ceazoqyw.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ufgcbavx.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vnlagqls.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2xquecxxl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2gvyvsypj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kjfseuzq.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2twxrslzk.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ucmrvvfz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2udstzzge.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ngdslwlb.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ruurvhxl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2wonwmomx.html


<!-- 参考信息 -->