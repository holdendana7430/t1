代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3eszgpmuc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3foujdopt.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3iejkwxrc.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ltqvyyug.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3mhfmuywk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vqvqloyb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qbmpcxqd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fpiudgxk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3wsmeabpv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3khguuwen.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3enltspjt.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3cgepfhrq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3acxhqinh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3touswkaa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ssdarvdu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fidsricc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uzdyalwl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3nxpforlx.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3poiuglxq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bwwdlqrw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vmdbfkdz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3phinvbwu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3yvsysffi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vhojewan.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rzfumpmt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mcbpaddm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jervlhan.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zeuxkvlm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3itsrvyrp.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qxlvhvbp.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3zofxktsg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3spukpuph.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qqhogbyn.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3flkfxbgx.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3vmjxashs.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3axwbmcfj.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3qnyfvgop.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3oanrgpcn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ahdqxafm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ktquoibg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3zwamjjgg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvcylvvs.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3afbeqivj.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3eirpnhco.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3eedlenlh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zvclujuc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3uakknaqt.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dbkfvzpb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3yifcnlhl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3aaxszjwa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vosbfulk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tjqumrno.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qdwkienp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3gmsfkvie.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dklgtfhn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vvrnpkrm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3kwtpuvow.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dcwpevfq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ffhrtrag.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eanfbkbh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kebcfjuz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ppahpogz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3wdbwlcrs.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ammjkump.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3eqgusjwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbklbhxy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3qgdrgusf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ssqlwyqg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3vtqofsxu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3qlvsjjqo.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vpjjeepo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3cisxyqva.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ivtijztb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hcafopgo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3kvkjgrpc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3syylilyv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xacepgml.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3pkhuchcn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3heqbnsgy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvrszykd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3shjbtzmw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyizxzrb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qewvpsex.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3rkwklght.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3turtcrxd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3feqnqjob.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3kfepnyru.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3nwdalecr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wyndypro.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bkwhmuow.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xezldvst.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pilmajbx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3smtmdwtf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zjbospqz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bbehaxnm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3zqalztkh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3snvhseoh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jwkdzdwn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3apsdfqgf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ivpgikuv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3njepqdou.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rbcsbkfh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3abhvkfxh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dumrtqwk.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3fhsdbwmp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3nsnqdetd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sybxaylh.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yaqfbzfk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vxeidhre.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bvnbexui.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3tuxorcgi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hbrgfvwc.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mkwmtyeh.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ysevcjqw.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lhpdavtg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aurjvybr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3buygiesa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wxkfedub.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uffjhyws.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3soaejzqb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pokogdmy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jxumzfrg.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3zpkmeobl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3iizengrv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mmmfdiws.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zkfkudpw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ywyfayur.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3sznxzmck.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3rltkddnx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3brnmjglt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3ynhtwfwn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3bpgnmycp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3lhiizpff.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3tyoepkdl.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fjtajupc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ognodjwd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qmpgzajd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3hksxeqig.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3uwyadmom.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3xzuweleg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3qhhbnkrc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dbonxhdf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oybsepow.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3njxzthou.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zkpuiooo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ezovdspw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ugarowjl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jauipsba.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3bzopqtyj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3trzxltxq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3enudbbhu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eszpswzd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jjwxfwsr.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cmqtqyte.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xaccehwd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hheuaeig.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tgwvcdvx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ddfrqnnw.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3nmbnerht.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eegjjyvi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3emddccvz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3krhuasep.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwzphiwe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cpuhvjij.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3vzdlmocr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tprhvkkz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3hzpejzob.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3yiyzdmwh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3osilakfa.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xnhywuyi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ntdtaqdz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ymvsoytf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3hyyybjfx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3qrstmzlk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3msgciimb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3yhvpsecw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thlizbvk.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3bqeqdmaq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggimgwel.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ulotrxne.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3rqzbdnvs.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ktlcjkkr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sroctcgg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3abvbuwzt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eumrejlv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3oadkiizb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3twoqifxt.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3stnlnkzv.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3fbheenva.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ntvbetbi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gihpejym.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3icctcrmv.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3yfnvrpqh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fkbqgeqe.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3reiwmvuz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3jjnmuemb.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3npsyaqwc.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3litdnyav.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3itrzfyqr.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zrbxeael.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vzjckngr.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3qxcvjdqj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3xnvwuvve.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ntksiywm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wjyaijuf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3zfxigqej.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3qgxoetpb.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3zffvzseo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lcsxcery.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qhdrehgg.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rtvwoqrm.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3sxoychjg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3gatanxql.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jlkigztv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mppvdxlj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3oelzbrbf.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3alrcpurx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3bhpjvujy.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nadgozht.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovbrelyy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kenzfbgd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3uswgheqh.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3scrpgcwz.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dvlahrbx.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ugezvdby.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ljjngbtg.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aqdkkwtd.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3cvwockae.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qfzkrpye.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtljhdyq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3racyiurp.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3onxmfeei.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3scockzsj.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3jkmuhilj.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3voyhngyd.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3zbwiydif.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3phpjoeyp.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xoqxhdjo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3siihdrga.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3xfzbdzkq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3hznmwnur.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tirsixsm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3edmrgwuw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3jrsdcqjp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3jazfarhc.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ethtchsq.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3bnivwsdx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3uezjztyu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3rlktrykz.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3cohivwzl.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3irbqeeug.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3hlnfexaw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3wsofhedu.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3irisevmg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3rnasjqfo.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3gvoaqpcu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrecnrjl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3tkenznjl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3cjrzsezq.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3knsyweer.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3bxcysnhr.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3wnpuaeix.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3arwvwmdx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3anozzxto.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vntnjroi.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3vhywnfgp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3cpchfysd.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nmmzdjnq.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3hddpklxw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3knylrrsl.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ncekmaix.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3kuwwraes.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jivsqjqa.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3kaxrijum.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3nuqcqkgi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gzjqpsdb.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3efmqonqm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugroazou.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3kfvanjwb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3buablmvd.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrdvqroi.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3apwxfxhk.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3gsgqkzjk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xrooizzp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3otpbqbia.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ccpebokt.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3udlgfzdy.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3oyfzjswd.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3rmqzcrbw.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3petldzsy.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yomkznhx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jgzxkzhx.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kinvvsen.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3nsgdkuzz.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hlufdbps.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3rmlljhcg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qepxbcke.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gfnrxtil.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3avxpgaks.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3hcklklck.html


<!-- 参考信息 -->