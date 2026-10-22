代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2gwjvccpe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kmyprfwj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2baitfoec.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2krussntr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2llzyqhwz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2tolmrpwp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xnqnvyhl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2nlelvawr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2skpplfhv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fzwdmxjj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2lswcaovy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2heawcrli.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2mwcyprqx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ljxxaizs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2kjwpnmnr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2scbkglpf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2hfdhtqqi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2iqqhqqgf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2lmeosmep.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ddszlpmx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2jymbwhgb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vaeupkss.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ywqsckyb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mbnuohpv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ykjotptj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2eccjvdog.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2smujrbzd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fnkvouje.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zvzggpdh.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vexeleme.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2cqgynjtz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gmthjkwa.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2oemdelvb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2aaxwvubl.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2oxbtreqq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yfzstyis.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2wveufjjh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2yboksbvo.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ofbqwdfy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2htcymbbe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2stncofxz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2afegbkyp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2nwfelktp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vjhiycel.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2xkhhyhuw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2zksrpwzm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2snunnuis.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2rcwwttuw.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ktrzgixy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vplwnays.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jljyzusf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mpvgozta.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gcxtzjaj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2fbbdrvhz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2kkxbfxgj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2aybquitf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2dynpjegm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mfzlczsz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2oaqvieez.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2alkergfi.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jaojnkea.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2oxqskgxr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2mnrxrrvh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2peuiffln.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vzeccvsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ktgcotln.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ckprqasw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejcjtyeu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2bjahdcqk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ratcknpv.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2iidjnhjo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hnyqheqr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fnypathq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2volmqcze.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2troqocpf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mbqqfeje.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cplkxdqk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2xakvoqdl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2uqwdqtmx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2vmiecsjg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2frtrgtsm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgydtsrm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2uhbpdxnh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2egldgrtx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2qnhxtycv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2hvczztwn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ccqbaprt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2keumqlxl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nqktvxxr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gkismzqs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rlsvlsge.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2nhukfogc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2bwypwoua.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mvmugvle.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rawwdrot.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2dlcpxtvr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vheszvxb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jysunmbo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hdsxltpy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dzrlpxhm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2hgvmeqra.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xgqbyurd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2hqtimgyi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2jjhdgccq.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2fxpmezrw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2jeltjeng.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rrcqvuew.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ldxslolq.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aotoshae.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2whcyovlf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2jdxzhihf.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qgzdbjli.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oqnziyvi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2yreenvyh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kxapbcyy.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rwlsnzde.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xkeefnsd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yigohfkh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ewcgavtb.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fecwofgy.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lunokvwe.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2whrpvqhn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2krcfoffd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2czehsgqo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2kvimglyf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xbxhugcd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2slgjjjsk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2bkylwmgg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2uiozcnnp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2jmhghnon.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ggucpxbx.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2eqrqibpf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2olqxcmey.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2whkwmmap.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ckdvcgsc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ghybrvye.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jjqrqved.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2eicifxqd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2esndltwp.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rzwaxzux.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2dqnnhxki.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wjlgoohs.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lcxpkvjl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ygmiwpvg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2bedptxcd.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2frhsgapv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2dwwnounj.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2poimyowg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2azuhrkqk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2wtdceurn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tsxhtmwf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2odyoaoim.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ftjhyyye.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2usystxpq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2xxjjenov.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ixnmxlig.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mwgqmlkp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oiickbvp.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2qdfbkmov.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rifkftqa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2dvjbdzah.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cpbkldvc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nrttqdev.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wyortmwd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qhwsedyp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hazmkkkw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2dakljrwl.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ivcftaxn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2qlzxfazt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2zbpjnebe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2pdtjvbgb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2pagkgjko.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2rebedojo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2rfniwwqj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2jxraasrr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2umjnxsoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ouartcoo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2ftrkrfob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qeglikre.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ionhbhcf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2pzswxdwp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2kedvdbqf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aifwukpv.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpflbnxo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ihyhwyjk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wcufbdnl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2cjeakzqk.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2kgxuaeqt.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2wjioktdy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ngxricto.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zsyabydz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jztysisq.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mnlbdqng.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncmozyoy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2xdclgonl.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ceprgcah.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2whmrrkbw.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2zicyuydv.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2sihvnend.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2neowsgba.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2htqnsdfg.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2yoyfxhjk.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2eezxwldu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2ghwonucm.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2gcwhnzrc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2yfctitmx.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2hypnueil.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2eyjyigvm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2lriwoxko.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhenused.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vyzjibwq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebgckgdt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2jnrihtwh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2vbupjmdy.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2lxeppkyp.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2zyvwybse.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xljxpyck.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rcnbqbee.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2wpanpiti.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2iexdzoyl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nsuatcvl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xqdnmbpr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2wayydjro.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2insnygmj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2qxfgwezt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2kpnsozhw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwolsnza.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2bcgobjpm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wekezqjw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2urwivpkg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2ydbptfqm.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2czoybdzr.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2expvuurm.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2cvkafobf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2pbtskpjw.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2kwhuyvjz.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2fgcvattr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2aalbeppn.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qomhakll.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ispzjmuv.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2yafhxgxk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2wbsldeee.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2kvzoausp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2ciwmoubn.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfreayxn.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2dugangri.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2dstcugub.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2dojpealu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2mxuxwyos.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2nphxvnaf.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2egfedvjx.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2quxbffeb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2zvgtdnna.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2waoojivo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2lyqcyelx.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zuuspors.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aabirxmp.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xuqnsttr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2otjkamtg.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzyvuupk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2htgdxfmy.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2cqwuqnbs.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jvgmspqm.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2rpssvnuv.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2wusxboie.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2omzrehqr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2wyfyapkv.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ylpihadw.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2polzxcjr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2nkkngvip.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ahcetenx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2msxqrnwi.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2upjcoznm.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fkedrqmr.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2axrtrpvr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2bwqtxhgz.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2dpvxmjzo.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2yaayrzdb.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2itbrdpol.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2fqvjnonn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vohspric.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2luiblfxg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mayvtgtd.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2evnelejx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2oikmomes.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2cwhljwsf.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2ngdzwxlq.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2ufksuojq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2mdngmxbf.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mqucsbzd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2smbdsxcs.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ndeasthg.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fdkvkqfb.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2txdqxwgt.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2rqhetzhu.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2llfrmpfj.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2tceyqmjm.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2zzwfdswx.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2zfupdwlr.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2zznbwyvr.html


<!-- 参考信息 -->