代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2zsneyugj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rxxcbhsl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2bmkgbnvk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wapgzroy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ksgmhlcy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rvtxddbd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tuxkumuf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2jcypxzcf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2rmadftpb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dqbkqtlh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2onwatekm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2wtztkdnc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2vyqbrnjb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2kgyuilce.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2vonhjniu.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2zvbssrfv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ghjdqohj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xgjtgovb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bcaybzjj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2mvvuvzni.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hjanmzwu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ioisdvkg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ntowahpj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2chhrtdyk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2pkjujuqs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2mvmykjcp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2rldpawan.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tnmrbxnd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tffqoszt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bitrmqzi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lmgfagik.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2pkulawjj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2sdocihpn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hujbnigw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2omwkakbw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2gmgrzjol.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ijcbymce.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2vbcriggr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2iqqriubm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jnqyyryu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2qnerzsxg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2aaalblke.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2jibcucqc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2tjfkrnkj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2baqtatsa.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nuwqunrw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2inuzrstb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfovmhnh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2pcadhtce.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2dsukiinw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ahznhqsu.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2usfzeqki.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2cghqfend.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xykzcfyo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hcdeaowe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vsudhivq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ggooidqc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2vxvcgqfm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2inmkuzmr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vfpgnpye.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2kmehgdby.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tivkmriy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sbrnvqds.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2byqqygbs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gdgkgfgp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2sapenwoe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ramifjvb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ckopfzda.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2otwenhsi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gdiqyuru.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2bksdrrti.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rlgxuuwa.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2luifjiqt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2gihuschp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2asdmoqcu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2jtenvshi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2okwoyynl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pazkptkt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2psdmszvp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gyoateax.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fsnvpfuj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2wppgedbv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2puhpjiiv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrsokpik.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yalutvvy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pdglaeel.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cmcbaism.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2pgfvqhus.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2vcuzqtut.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2wqtpmkwn.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2znhjpkna.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2aktoihqk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bidfdekd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2dzdaypgq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2frbgdluh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2wrzohbxz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2qmarsubx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gsbcscpz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kqcoitjx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2epqhypsl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ppnntoqo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2dhzkwqyp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2cichhscd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kwfuetvx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tzsdgktd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vnadpmkx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wpwzucbi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2koehfdhi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wfvnzjnx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xqcwgkol.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fkcpgoxw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ufvkbbpj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iinryemb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zyefdcsw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2mjrzjlwq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mheklqtc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2urpmvrbo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2aylcqymb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ybsxrcyc.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vvhoywna.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqenmaei.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fcoykslx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hmxeophs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rxdxwecf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tsrdpnlg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iigputzn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ttlduosc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2bjcbfpuv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2mwdeykmt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2obhwuojd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kdmfddhy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2gnzicbib.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2lqylasfs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ubrayupc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2umdhtudc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2crdpvxok.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2umkaqshl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2yibutdof.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jtqgignn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jpeobmbr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xgqaucqm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2omkuthzz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jfsmcjyq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2xrbyhqna.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2dcojvljf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wlzkbyrl.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ztyzacgw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hbajipfs.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2afdaseqr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pyrmzgdb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2wsvnvymc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aatmurus.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2fcbqoljb.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ebonpzrh.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mnzibexc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zdhqoklm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zeozeplf.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fplbfhnc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2hcppxkes.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ffropihu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sovofbtv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sazxiaba.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2nosdlwsn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fpdeojca.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2zhycmwty.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ypowcwqk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2psxkqwal.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tbxkroox.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2uqclnrtr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rusezhkl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vdlmpdgs.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2shyzmhft.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2vuzhemop.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2agonpwes.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2burlnfhx.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ineljsxp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2xvacxumq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2snihcgui.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2azlgguzx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2kokustxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aaxfricr.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2krsmenaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gsiwnbmd.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2sgiokntg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2llhkrexo.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2uvbntwby.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ujcckvmo.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2rdystmgl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2qxgjtwur.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2grdqdhtv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2zfdtulzt.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nffpjghm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2zfqeeufy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2pnonvzns.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2xcnlinus.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dvncnuei.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2hcvzwqlu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2aaosfurl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2uuoyewzl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2nrzpbmcg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rjfnloiu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2spziawws.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jordopww.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2aiflhpdt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2dtpotopr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2takzcqgy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2lfbktjls.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2vujsxunx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2qvfopmvx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iamyuqha.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2apxytzgk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2lxrlypyh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uidgomnh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2schfsuma.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wigczxzm.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gfvqqjck.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2fgsuzuja.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2bnxvfemr.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2bpbbvfuc.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2vkajmjyg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2tbtemjkt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qmnpzdwm.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lrpuzlip.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vmjmqpys.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wtinwtxo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2fjvuaklt.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2gyuftmnc.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2stngxvdy.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2vunoqhgv.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2ubqgrtiu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2azuikkkw.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qscefihz.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rxwomfnf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mensleod.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2uaqryyfv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2xktbcweb.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2yrzwukvh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2fxgsjddz.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2omwgalmo.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2evochuyl.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ztcqwvar.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2djihpduq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2chpfkzgb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fsvidbxb.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2yktxfnbc.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2rqdlkvvr.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2noevnups.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2fctskdnc.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilcgzkak.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynnhdhdh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2setsbida.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2qaijuqcd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2npwekfym.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2sjcjxwrz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fciqodku.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2lxnpeuqu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2uqaadsqw.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2fqtglfjy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2vurmjdow.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vgdtgfjt.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxypxuri.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2dfqvbhar.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2jgvxoalh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2iflidcwy.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2qgceerna.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2tmjpldtv.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2yiqhxlxg.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2bcmcwkki.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2riwycwye.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ygyqfahu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2gqyinrqe.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2rxwcciyg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2zbybvmky.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2chivkmsw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2nozchpuf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lzrastvd.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kdavcdpw.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2rtznmjmm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2uetqblgl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zfbvdykf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2xcfifjwf.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2iimvjfzo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2riajzjsr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fqfnaybw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rquepimx.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hanutphm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xtmgxwxm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2whchwosy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ckivvtyg.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2oqrbyuja.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2imqwfgwe.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2cttrnpmf.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2lknoyicw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pbbhzuen.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sfpvnnxh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2feutcxxd.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tdumtemi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2ixconpqp.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2brqqybpo.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2nqbnjgad.html


<!-- 参考信息 -->