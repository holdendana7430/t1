代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jinpqkxo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vhyzuxja.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rmjpceop.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2xneiqdty.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2uglxkzvh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dpiquzjj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ofatrhka.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2fuodvpid.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2pkhrozhr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2pqmxfyjl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ryaaqtpv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2gzdlcvqh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2uxlskkuy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2bxlwpeea.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xifprtke.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2jzolbpqq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2igcirwzm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2igdlqbgd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2bxnjbjrd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2eulltmfk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2igwtwwgr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2xeexoslw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2qdjnzbhg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vtnlxiof.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pkzocjln.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fagstqop.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2dtitefrh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xcyeyhso.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2mvfbhfbr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2hzmankrc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2oezpobps.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dvtassgy.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hnsysgsl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ducmwvlt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2hrgofbnj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2jkjbechl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2gptfmule.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2fjifaehu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2hwovlnce.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2bfckdrgh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2yqkfjnxb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2iorhveol.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2oqglbxtd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2relrskhh.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2pgsjxkae.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2mifhyckq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2mbsnamgv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2bzzrvtyz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2hcguqdqr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uaybivoe.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jcopmndq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tcwlakwx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2znpzvjjl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2mqclmrqb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qcywqxji.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vbgzjlyb.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2wjcppnkt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2qxidompm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2odboywgu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mogaldrj.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jnocpmnm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kgkjvgvd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2yuspoegv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tfhodobm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2uwqdbkbd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cnmzzsbe.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2yrqzwebz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pmippdvx.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2xydycyvf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2seoasytn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ilceybfu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2sfwtpzfo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tkmjvars.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2izgbgcfl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2vlfgjtil.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kffsvlie.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ebxsitlu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2agnchabl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2envmjxvn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bgfhhxpf.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2isgkjtlu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2djolspyq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wklfudza.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fpfvkmha.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ovcsfvrm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2cjxpbdbw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2xnwwwyux.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2xqrgiynw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2dcmnfwpw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ztmeuocl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hfojkrto.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2phsfsleu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2dyihjtdl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zgmoibtj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xmnegmjg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2gjccepkq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mituoovp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vpqgtsrs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gvjkzbpz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ksoqopjj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2trvwqjxy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cqmonzaq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dspcbwci.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vbewypoo.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2fccgcpaq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jpdimnwr.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jcvxwgyg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipcptwje.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dguepanh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2psevmdip.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ysqefcgo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2taptlkej.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qovionmx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2kfwseuqt.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dlrkkipv.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2twusnwis.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dueecgqs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nljgnxat.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fluabaxp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2egjyamge.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qcilyrbd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2merugznx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vrmnwsbl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2moagdsjl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2gztplwif.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2borxojxg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jyrunoxm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2nqyhiakx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2radprynw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jnyflrib.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2tjubqwxg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2idnnzbrf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2tijfijgx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2owfpznzl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lkisthhu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lmcxmzep.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zzfgpfjz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2jwydfurx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wlpvgbxm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2fzzmlfvi.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2lfxwrmox.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzvghpop.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nsvdpgtz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kjmbfntc.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gytnwyaj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ktiibsbk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ilqjrobf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2himaabfh.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2rnqfmyuo.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2jdxbdgfn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kwbcrctb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lcxipwmf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2olmeazuc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sildielx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2khcqwwvz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gcuoseml.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zcxayqlj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2odartkup.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2txiilkji.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tnjjbcuz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tcoimyrt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ypuguhma.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kcesmfdu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rudlptsz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2nnhiymla.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajpcmnhu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2cadlvcsx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2kobxoqlc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2xofhmhqa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2oaqvfblh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2xhonluls.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2rffqpmqa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2llbjckxg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2hzjwweze.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2tcxafcnh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2hygidarv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yijyrkzy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2bndprlsk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kbpwqjbb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2wvgsbxwg.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rbshqfyk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2helevsjq.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bbkogecd.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2bpzlfcwt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2proabwgq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2okvonovv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tzdvlyke.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jinfezjk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2jtmmcqyx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2ytjnipdc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dcfymhox.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xleewkdz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2fyvaoltp.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hwrgbdpu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qamtuntz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2famspfok.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxonmqxn.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2bdpvvxsz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ywkxngid.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2zfajuuyf.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2upssrmfs.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ecpnsibq.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2sfzxieif.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2duzwmxxh.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2nejyieep.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2qfczuczv.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2vparvpur.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2pelookyy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xcplcyhe.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ojrfyuup.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nnazqkmh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2mdpkfncn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2vkoejtww.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qutfagck.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gtnpgdjs.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2ebsbtysn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xwajbvha.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2jplrjgia.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2geydvobq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fvouazui.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2edwcazpd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jjqevaat.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bcxcumgc.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nktbbwpe.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2zhzkjiks.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ovcgiqse.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lxssionv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtcdouyx.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pbdubexq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ysljlfcd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2jyfutybx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2tstenvcc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2oxibecsl.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2sbgrapgl.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2hznanefi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aqxvnsvp.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2pbshrzgs.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ygjevlfk.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cmnwxucl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vwazfgml.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2yrdizerk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2hrepmeat.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2togjgyan.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2pwxkdtan.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uawomcsb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwqrgvft.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ptlnjgoj.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2npktfqpb.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2chovxkfo.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2fzklgtrr.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2tzpmsmxc.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2qnasbzlf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2apufnfvm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuplyfbr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2zkdcndrj.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2ffvwflkk.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2ecbyepfn.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2qflgrqse.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2pofshnaa.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2xpwimelg.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2bvikhhfp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2iktptomq.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2hxksmfxt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2abtuuxoq.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2aqflxazc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2jeloldmh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2qoqggjku.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2bjpdelyc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2ddmmiwfe.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2hivpaxtu.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2exhtuizw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2eyawouth.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttiowbgv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jhfdtfro.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kkkfdkku.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yntvqmnc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2bjozzhhx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvsbgryr.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2jdxopywb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2dqvmlbdi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2eopikiif.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqpqvnlg.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sthhbrwm.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iwtvrpca.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bovvahdd.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vxlmmahs.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2imqtbrlt.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2mzbrwjfz.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2hfiiqckq.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2vgbvhawq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2selupeob.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2kizrkbny.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ijshtagi.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2eicmcwfy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2pfliiyhc.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2ztaxnfjn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2fvhucqzf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2enysopcq.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jhvuhmsj.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2irpckmsq.html


<!-- 参考信息 -->