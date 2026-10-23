代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nyghxmbg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3mrrcfvwx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lzaxqcvq.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3lpceytrc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3mnfuzxcc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bliycfnz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3wykppnau.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3bqacqqtx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ggpkxtpc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3skbnylkv.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3dkjkwoaf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3mdchquny.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3fsqupdtd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kqlylqxq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dnhpqyek.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3crydonzm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ajnffkbv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3rgmiubto.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rtyaaafr.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3lztmqyfw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3efvzxejk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ruzevfet.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3annkyycm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3pxjbovmw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3omdajcra.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3skldxeta.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3guqxjtzn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3hhkhfwva.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3zdieeknb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ypwktjuh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3sergxzde.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3wttengig.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qwbsvfsf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3snpmvnpd.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3znyumwdd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3vkrfubgp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3cizupgfm.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3akglbzmq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3qdhchdvb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3xiofzjjf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3xtqplvvr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gztfdart.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ferkduxv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bnphmmbc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3mkniayir.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3agzyuzkx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ousroxuf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3shjjdpyf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3vqkpdiut.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uwbailkr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dbsrimri.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fujtyexb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nzrrkyor.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3lztaqhcq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yeuakqys.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ssaubhfw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3vwdxltys.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3upbsnfoo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qjyalddk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3gpbridxn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gpqixtlw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bkeajltl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3mfownupl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ltuywskq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3mzsfhhki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvbvnvjt.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3lrtdhunb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rvwwrmej.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3uyyytfje.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3zrrofeti.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xrgirjgw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3xnzvyakj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3crvptucp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rwgythoj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3zwtxdolu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxlsutsm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kaxdwpaj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3gmowiqwc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3pqmdnqsc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3uvepedxt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ecxzzexr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3awyhvpag.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dwasvydm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3rnodcxus.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ssqsywuy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3wzbzrwro.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3bsfkipsz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3dlihuylo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pbjkrgdl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3efuylpik.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3yevuxdyi.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3klyzrbgv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3hygimjhc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3fovddfav.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hnosonst.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gocxevwk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hjgwwpic.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3zydoztqe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tspodcsg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qrykdwhd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ihcgrhey.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nmkzcnvu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3dwpmgqml.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wzfxzldg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3vnvbvhup.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3rnifihqo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zkhgkceq.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iaxwyqra.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ikrbcuph.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hazyptzy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3cyfuhsrd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kucydmnj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ubftcflv.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3jjxngscq.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fbeydrog.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3owyjqkuz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oduxbnvg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3puqsdmay.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fyuxqsof.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3datfaihr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vvborwub.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vcvjeohj.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xopimjlv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xgnmpiel.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uqbbhynn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3qjmgwodh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hednkdjc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3fseuhhhv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3dkprtsma.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3dxscjxor.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3ozcghxda.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3ufpvabwi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3wqohicyl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3koslczzk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3hbndrjiv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gsiajhlq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3arrfdcct.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rimaofod.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3dpvdimvh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hfcqlsld.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3cvijxthw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vmpvjhld.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ktlynuzq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bmmokhpo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qbktydew.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3chgiyufk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3vjivproa.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qogeurbn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jyzketlq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ugkfjjsj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bmcsvgsj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vvpdtsbc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bfwxwgjj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pstezieo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3nirewfzr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jgqxgemc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3letpctrx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3afnenyvk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xpbqrscc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uktamzpp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3tcjwgcrq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rysewbua.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yippbpbv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rhfgdciz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3brckletc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hcyfxvsl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3bcicmpzp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3sxmottzq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3sxzbbmzp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xprfoojg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3atapbbss.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3osybtzki.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3azjyshle.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3yhhworot.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ewuhhdxn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3bypqtvfm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iiifalka.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3fizwuezi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rujwtvhx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3mpcqcfxq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xxukunpm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3zwcgfmdl.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pvjwxqtr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3noipsutc.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zmcrldap.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ksxrwjnl.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rxppnmtz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3iimgamca.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3rjgzwtoc.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3xaymbuvj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uwknofgs.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdspdabh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3xvymtibh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fxqtptar.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3xbcmfzrq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3tbvcminq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgaknvbw.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3olfdjaka.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kdbhfoad.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3beniaojc.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qgikshbz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3qzfpzrkf.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3tchynrpi.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3rimrdfoq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jiksland.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3icqpvgfe.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3gudxvsxq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3ypkagyxi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zizgedsl.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ziclktmo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqgdswke.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fgcysndy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mchdgwmo.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3oynrhgqv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hlvpjrwq.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3voxnizte.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3xnuolizj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rnxisvnq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vwhfiulv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kqtowshn.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwqvrtma.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3tawfyyaq.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3vwwotfza.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cidhgkkz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hwlzoazg.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3nvxbiuom.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldltgcmu.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrsyrblm.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtsmuxvi.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehnfbzfh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3exvzjytr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3siuickxz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3nuevekkk.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3rjwwufke.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3wqmeythr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3tfxtxrum.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xmqhmhnr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mxksmhoi.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lcdpmdti.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3udbwrrab.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3gqniessd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3oymmrsem.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3nxqxdooi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3pnhqmbga.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zoncxypj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mgzvbthn.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwtgxjfm.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wojfjije.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3fqcgujyv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3pdpnhabm.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ahdmzjkt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ohotrnrd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3efwaboup.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3fymelqhv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3dipjgrvi.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3pfxgiowg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxenmrfb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3niszxtuf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3zsedrfjk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3jvhtmzen.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3ugrttjva.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ciiekrxp.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hcyckoyx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3fdqsvxri.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3vpscudfu.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3zibghgpb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ixbprsyj.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3sssbrxec.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3kndwbbax.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3blkvdpbq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xbuwvimy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3gkgjfsta.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nxocmsbh.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cxbxprds.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ajjqqgha.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3vjovbybj.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3bjlyjfqv.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3mauemwjw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oezulyyo.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3qbjampsq.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ijmyzujl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3lfaxofnd.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3srvrrjhi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rqlzcueq.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dymrkpuv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3fjoqnoik.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3irerpbgt.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3uwslgael.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3hyyjvpyg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wgvxgkgb.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kkssnxko.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3xxykterd.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3onzwpchc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3nulgiuzn.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3fjlgdsxh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3loddabpr.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3xgguzswl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3mravkuwo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3xrowbcwi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3lfiybjap.html


<!-- 参考信息 -->