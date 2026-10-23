代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3urhqvggw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ekjpdnzs.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3yvnrfvjj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3pdvxyuvr.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xhcllvmo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3pkohnfer.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mtgzxzkx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xxthnfwv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3byiyqyhk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3assbtgqy.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qnztbewm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3oubhxfaq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3eqdyccmw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3imiodiyl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3djtkepfe.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dwhyrwwt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hielerph.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ffdoxnjg.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3unpzvsrg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3fewucxwe.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3kwgjadqn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3shmkcnho.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3mqjjhlpq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pxbawtfn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ctmsrhpb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mrxgubzj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ofiohrth.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cagxtghn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zqzagijz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pjcnpqvz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3xwucegfz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vxppttlo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gmthxkwp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qzyhfxcw.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3rivafsal.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ujlqpfqo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3euadlzgq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3wielkrei.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3vnpkpkrw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3edimzzdi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3spkahmyz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3wlyswntv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjxpemwd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3unzkenys.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hxljtwdp.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3xviqfadl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ykydltep.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jdbibhgg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3vbzrauft.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3sdcmdvhd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ensyahgv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fgoaqbln.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vbwuiypd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3pbkecdfo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hgmfondx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gcbcyiqh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3bamsbfih.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jvriwwws.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jziaorae.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sepiekmq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gzxuxgor.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ztwaksbl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ibacolle.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vtnzlnow.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3eucfojuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ffrpopxn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3kbwtcnat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugfqwbjw.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3sdmxewax.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3welufrzb.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3evljomoe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3gzvetecv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3seilvjhc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fnyotvgf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3swnsbbcu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3emacyypo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qxpayvpl.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3wffxcjgi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3fhefyytu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3qbdzboix.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mncllgzc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3tnqycdcj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tsmuxdqe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3vybqdrpo.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3byvtlmce.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3chooupod.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3oqzspmbr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fygnsgvp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ypiydgeh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3djnmwoga.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rjheplzj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3utrlncgn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3dartzunu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qzyubnzu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jvpfoarv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3kaafumvr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3izqpufkm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3netniqxt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hgtllili.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qygebbln.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3lvywfpva.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gujdnwmj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3dlmoyvan.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3wuqufcld.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gzsiucqv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3dganehio.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3blpjzocx.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mhnyxngu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rspjqjqo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pwmvtoec.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3tsadwrpj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cljyuxfz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3emnnsysp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vhylalgm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tfyvicnz.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oebuezpa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tffqqnvl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3grmmqfhp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uoaedixk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cngfshdd.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3quqwtpfk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xcdxdfor.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hdolchnv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3zcokjsec.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nhsfaoxi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ktcoqukn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3olmbxgzj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3kfypaqlb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3jtbmzpbu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3lnegonjf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ftoldfpv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3uzoixqtl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3emmuknam.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3yawjxgtc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vljhllwv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3aggonirc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3cyvayosp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qmnysvud.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nliutqfc.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wybvknqu.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ztknnpzr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bhshhoek.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eewzfptt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3smznoktx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gkgncctz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sojedecm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wbstrrud.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwlekdxf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3egsnpkii.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ehiiwcsq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3egdjvjol.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rpanpklk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wdlrhonx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pmrnriyi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3rttbtssn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dssszulg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3evvmdwmw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hagilorz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3rkhmnlir.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxdziezo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3liyfgice.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nqcuwmde.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tjajices.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zfepgjxl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ygtskdyp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qlcrkesz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3akatdqji.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3otmcpoei.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ziwdsjld.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xdqzhktu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3kpsfccol.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3gqmbblbm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3skccelmf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3hggsomhz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3julgrvpp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3zhidihbn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fjbetcau.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3dsexnrkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vaqxhons.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3nzlicfix.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dyvxtnbz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3glyxpvtt.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rlbwjuyd.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3yohcfqsh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzmaxfoy.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3zocwfuil.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3izfiqcob.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zzuksvfp.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3kkeucxes.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3khalfggg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjirytpd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dygbiaud.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vkromkeh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kjrhsxmt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3tupelbcf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ytydtmay.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qddebojl.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3fchpjsli.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3syrdfmiw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3lkiccnrd.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3iyqdokzx.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3bpydvvar.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3opfjguso.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ppdyznct.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3urdyaovz.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3rfsodghr.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ckvorktn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3giwumzhm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hbiuloeh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzsipqvh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ttuouhae.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gaulajwd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3rqhizvfq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3aseqwgnk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3jhepwfbo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3pumusujm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ynexxjen.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wdvldvba.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3opovkjgr.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hyarskwn.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vmwrpbkd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3kgqgfdea.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lsjcmyul.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhwztgaa.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3frpultrk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3wwvwyycl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dntsmyzc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3pcrjlymw.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ddthywvu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vedllios.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3nkoptxxv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3jcflrfmw.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3nfmghpsn.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3gvlxsddm.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3chunmpzp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ykmtczyu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3sspdnvwq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nvnmqxwv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3oklwwlgz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3hqpuomnz.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3avtchgxf.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gpcvtoil.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3pzohtegf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3urulfokb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3lobxdaia.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3cwfsvphf.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3imxhvfbl.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyeryoxt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3mgkhuthb.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3xsonbqmm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3dtzobbdy.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3zqrlkpdp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3roodvewv.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzipmgql.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3doyctvwd.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pektunzj.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vlodwdoo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3lzarcbwb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3itpzjmwn.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jbfdjwjr.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3qzdbrbxi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3cduilvzf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nrdavvai.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3vdcgkbcb.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3biqikhyt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3aotutves.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3wocitaeb.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ukhpwxfr.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ejgbdqtz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3kzujxkqw.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3nqaevcks.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ragjqlfy.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3vwhgbahd.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwsbocft.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpixalgf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pbbhznrp.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3bdyzgeyp.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3oqqkykjk.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vwknqifo.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3fmdyivta.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3icwttekk.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3beafpntm.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eowaxswi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3wnxuldgl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gjbwegyi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3btahivli.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3wwjnkeko.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3cugphrsd.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3mddwkyum.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jofsuvyw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tssvuvwx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bbokynld.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3gwngnxjr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3kmdagsfy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3rshghtqb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3qhsorrlm.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3jjnbbved.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3wjxrlqas.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3jufnokzl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3vlvhqxyr.html


<!-- 参考信息 -->