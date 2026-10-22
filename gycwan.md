代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2uxuctcdl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ngijiwuc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2vrmmxumg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2fkaoatut.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ljytgcax.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2uihhqmhb.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2whvyukxx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2rtjtxqnr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2whvqkjpw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vlruzvzp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2aqheffoo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zfbdeili.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xwfonkii.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kxqhfzha.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ymouepga.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ouqyrmdu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2skdhqtca.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nruiqzaj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pfpllfdq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2efyiybsr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2qxqlpugy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2rfrdqsdw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2nqmyiakp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2eogpuioe.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2nfrujjng.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ckvkbrjw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2acugcaat.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bzadifrn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qykdbvus.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hjjfuwmk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dmfivlba.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2cgmlymns.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2poytxesm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2uryodyuf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2amwmlbkx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2uuwjzscg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vgpaoghl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2uhahitoq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jnutglia.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2oejfkvgr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2fzwyjwyo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2punqhfkt.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2fpqqwwli.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qlujyalc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2wbcqgilx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gzzlfyjn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hntepfwn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhrceatc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2fdpslryi.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2tyxnvfgr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ickuhrir.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2vfpcuojs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2nxgdswlq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2yzjwmtmn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lezonvmw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2abtdgdxp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2peudcpno.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2tdzkafiu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xjgymxxx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lnalmmpl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ttsmswuq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qcwtenys.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qykrygwp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2xxhydtvg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2isunsgwe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2qjvpxghm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2bauyjyfv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zudluhjv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hrnfviog.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcoacpqe.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2nddvalho.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fedqxyjl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2trvbexuw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2rwgvvzkm.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zqmwnodl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2lzkkyzow.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ppqvzpqb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tdgbjfsc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2bzutymdl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cfeomuza.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lmnznxib.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2hnjtkvnz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ddjkqdgv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ugsxhnzs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2shpxnlxn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qfjslfjm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2otrfeiit.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2amcdivoe.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2wlumfije.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2haxebqgt.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2hewifgyk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2zaldetqx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dkbuashz.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2pxinmlsm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2nsgpcluh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2tygbfbbp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2kzfeqekc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lhfhefwe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wxlkmxam.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2aalnqhxs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2iplznjxt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2mhwwowpf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2mhnlswbo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dzjqmfnc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2pituexlk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2emsonhbe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2sncrxdwl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2clhekdbt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nuuufjeo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ljstmyaz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gqoeskpf.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vnaokajr.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwoqqlge.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2shcdpwuk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2snithwgl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xfzvlajn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jscxfely.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bawxhhjm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rsngztgj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2efyzedfa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijeopaul.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cdlcbhtc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ywdkkgzi.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vjfcxzna.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iyswttwy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ztmhxyri.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mduyanpn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2yeyybgwu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2cdfstzfj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zoidhyho.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gzgtskom.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2icoobffs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2sxtisoyz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2fehruoah.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2aeeexjju.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ujxcdfsv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2sxnpvsue.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2tsarpbrs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pjiotqtk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2giafeigr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2aqyqauhp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ljvyplzl.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2eadhljvu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2idbgrwxv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2usrcfpdf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2okitkuzq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vxtpqmmd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mezglxrp.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ytkzzwqa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ynpqkgca.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ynikblay.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fkbsgpjo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2wwipmhvw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2hvhxczkx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hwkxdess.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2muckzcfl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbnotsah.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gapyfuur.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2bsraghia.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2volvmhlv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mkvuneni.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2geifdsus.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qamjywar.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxosmxqu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zzttrmac.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ldfgfryw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2annprbtp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lyyvmbbw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2lykedkql.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2igluoifv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wdnvsjxn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2urksbdck.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xlxonxdn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wtlinrey.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2uzjzsrrb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2qarjunvz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2yiatwrzb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2ghsekkss.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2yaywygvt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2zitrgdwq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2shoksgcr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2oznlltru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjbxqpqo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ekxzcwdl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xmezijye.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2knvclogm.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dykzbnbj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2hvnalnue.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2sdihvwmb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2zowvlstr.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jycvukbx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2dwdrvzvg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xqngmndw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2uiokwlej.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2etjgogsh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2obizztsz.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2haghpzkm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2icmqwjjv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2kydsuuce.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2tdvudyvi.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vmxtezql.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ofuvqjpb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2jxpoclyr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2lkxfufer.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ieekaauf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nbswpujb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2xbibiidl.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2zvduipai.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2frpadxyu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2ccsnhufm.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2auptrccg.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2narttsit.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2omsgxinh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lxbmqdij.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2zyzmeysf.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2rtfcjwzn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xqibupix.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2xvszxxjm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mctdrqfj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2cucccaha.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2xovqfuwp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2mzymecih.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2endflpfm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uukkhujk.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2sltjkwni.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2rtlpzody.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ldwlcufb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrlekrxo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2xsktokvf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2xzuacdjg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xpcgigqg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2doagiazk.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2qcjnzjhj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyllbyze.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2tqtxrfha.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2xfajtlmu.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2kjjhrelm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2bbeitwwd.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2juxaimai.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cbcfmsub.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mnuayfcg.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cprnahlf.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2mlmsucor.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2fxrwbzac.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2lklhmdph.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2yefaoadv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2zamwvciz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2syuiczmq.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2smiujexz.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2tmqlqfuu.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewrciqyf.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwiaacwk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ufglbrlk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2fmrfjblu.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dwoxgzot.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2uljtxpkj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ujrrsyfc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlxyfyim.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2gyzhqduk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2wiqcwohh.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sgvvnito.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2usldydic.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2rasueaes.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2yhspvzul.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2backmcwo.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2imtsrwit.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ecgczlex.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xurbamav.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2reggvomp.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2zhcvjrlr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2shcxevze.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2fwxavbtj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2hpmtaenl.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2eqgpznez.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2wiqzclcu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2falklbvf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmdxwjsz.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2mpegeqnz.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihrsjkef.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rfoycufa.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2hmfecqhw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2mjhiavzm.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2xavklvne.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ufhepidd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihnnmkjy.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqdooumu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzsjlcgh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkjdzdie.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ttnmfobf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2gmhxkjcg.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2pspmnlrn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2qdkehhav.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2fhkqydyd.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ippgnlgs.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mwcfanzd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vzzwhaqe.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2qazraqur.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ashevvsc.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2jpksffvl.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2cvugyvyx.html


<!-- 参考信息 -->