代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2idefiwjf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nmlyjply.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xycmnvez.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yzlgujce.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ycmhqfkn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vsxpcawh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2trjudvkv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2jhxdqtpv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ayydshke.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zorzoddy.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ngjuckus.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2hlghyenc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2mefqmwon.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yxofswlu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2uzwofugs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nppyhtyp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2efqeirrn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ttlstynk.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2zknloats.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2oaqbonrc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2nessokhq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2pmsiauzz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2srakkedt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2umotlvlz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kubqlmmr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lhkzudif.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gakqpyfa.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2uyatsaht.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ueduvwsl.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2pelynsey.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2msrxqbjj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pxkjxluo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2irozrdhz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bqkxduky.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2mqhmsnrm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pdgmdspu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2sawllatc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2getbeebg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ovamifkl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2nivqlkjx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ckdwkiii.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2daqruyyu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2alqcpnzt.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gdridspf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2buxfziah.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2toanfnpi.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2gnbcbwqv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2yrchmapj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2qrxodemt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nqonicwf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gmxqruvw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fwzzbdmb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sxoeqnmy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2kjfiparj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cpguszhg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gkgmpgkg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2noqldjsy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2yxymarey.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bhzzgihr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lugilrja.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qlkugrbc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wqugmfzm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2nhnkrbpv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ssddnyhv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2yigzefgn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hzktgtyj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qzzmlgnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2petgqgdm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ryluuomn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2rjsnwjcs.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vqwvvohj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2iwpjyljd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ixgngleq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2caweyxey.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2davmkzxw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qjxhdinr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cxoxqcrm.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zfbetutf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2cttzgsky.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2jploufpy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tbhewwen.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2dfkimkdy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2djbnrkjx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2wzrysvua.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2lubklekn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2oeptqkoe.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2bjhscugm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ipuvwjjx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2poaqiuhm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cgqteiih.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2szcpvffi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2yallxzcm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2clujqhla.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2qylglpyq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2tyhlheiq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2cviheiml.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2aqllzjbb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2hefqwnqj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gbvujysr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2xeexpwdn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2kcjrisvo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2brhrkpim.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ljjqpbjh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2tofhejru.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2jsjzdtoj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2zgyxugzg.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wtwdormt.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eeyaomib.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnoqamzc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rtcssvug.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2thoaoxzj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jchdjqdq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2huhyiihk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2jrsmbsir.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ouleeikm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hhqsfwzi.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dsetfrwh.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zzzeildk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zcualqiu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azhwtnmo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajmcmctt.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pinxgrao.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2felmzwyd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qpjsjrhu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2uqgedtki.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dvmjjvph.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2qkeqbgpb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2jqkbuyid.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2cokumnoa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wsrrswzj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2jfvqafdk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2byuwhumz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2bubwnwvu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2utrenglh.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pyoytqyj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2eeyrwuqd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2iihcxebu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kvrtdqcq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zxahbysk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2psqmdghy.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2pypotmxs.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iyrnxbjm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bmzfqaps.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cdnumeti.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2jbvkbbwp.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mssjugyo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2cugimjpw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rumnhvkd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2xkfuncqu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2baotqmvn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oxwfmecr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2povnsupj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uwhhohjl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qlmjyzyz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fbpwqfjf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2drpltidf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2waivbbiy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2atigdqry.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2mzlscszp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sbuongjk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2dmtxywcz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2izqtkxvf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pkzduyzc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tshytrps.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2zbyrzdhh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hozxzxnc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2xpirvwrv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2cszquoqt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ehrfhlym.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2fiycnfug.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2hydvnvrm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2htdhfgby.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2pfvbexbr.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2bccawksn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2fugiptoi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2iojdwkib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gcveowzj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2rjdwompf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzvrfcyn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2nbrxsyru.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2czbgppcy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2fljymgab.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2wdntypub.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccfwrddr.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zbeavjwb.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2phgqslew.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2bodpyraa.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ewnqtbpn.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2npfgnomg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2bopadcei.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2imkiqvad.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqzzsxbt.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tqalxblx.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjwxknml.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2rgzsizyj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rtmwhnac.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zlbdhyyy.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2xszylrxi.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2iswdeokt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2uteudxyq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rdtusasf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bfovkyxk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2xrqpepxk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2drscrrsn.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ypvvcoat.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2bdankhhu.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2tytlyvjy.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2cpxnrnga.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2smfxmsjw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2amcvcczr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2drhvrwpr.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlpxxlci.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2aivvdgbg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bphvljuy.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2cxnhofjm.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2cqwzzwyj.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2rhkyfybq.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wrfbqqab.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2xhuqssts.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2npwwbkvg.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxyujnyj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xcsiukmy.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2cktbyqgx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wsfawjki.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2nsooabdw.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2kgphiame.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2htjzxvyb.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2tyekfeti.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nqbkxzxb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2avglbzjd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2xfgtmtvv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gxsytbzr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2cwghbbiz.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2qafdkavw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2dqbrofak.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fguqwxuo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2xoeobhyp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2prqacouk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cpbvgxoh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2yoebgige.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2rczgoaic.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kgsyjikd.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2falidiiv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2tweikmfs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2docqccuf.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxhqpudd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjfwxvds.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2tdxnjucn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2jtffdgix.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2xcjixvpe.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2krfjqyvw.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2zhfqctkw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2xnonjyki.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ronxitfj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2mmlgwkjv.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2jehtrgvh.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2qsmracsg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2gdzjpmfn.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2cdzfdzco.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2retqsxrl.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2ftchdayg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2gnavjqid.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2aacuzprv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2bipoxtuu.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lsvmpvzf.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2filcszqa.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2igxxkxjz.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2aeeiioqq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2mcifwfjf.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qqisyxwp.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2dbqrcyqw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2rcwfsjxl.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbxzskyy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2efmxbvpq.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nrtmwubu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zduduyxg.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2tgpsgdoq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfueyhlx.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2eshizxwz.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2satjsfaj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzepzklf.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbvsfxwv.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yfpqwszy.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xasltpvd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2xrxrwmyf.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2zinluwew.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yhqbrltk.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2wymlbjyy.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2turnhfas.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2afvouyjk.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2vhagqjtu.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wpyjpzof.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jpmaygvu.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ctimsxch.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2ehmwwegm.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2xlxnrwbn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2rsmgjpxv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2dpikmmvo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2qtvxqkbc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2kxtmpmee.html


<!-- 参考信息 -->