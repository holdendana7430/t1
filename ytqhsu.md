代发 wailian999

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3dorovcxf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cemnwugk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3znavbvdg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3koywpvrj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3prpjkfqw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3sxamlpup.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3afttjnjw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3trluchss.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3xufkjbtq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ojqzdnhw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dqsquwju.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fxoiqnbj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3qrxzqrhj.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jbagssvt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3eccteooa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hcedwdsx.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bzjrvgof.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3csuegxac.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3gnudelpu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zmmjqpei.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dfetzwwu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dgyocwfy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gtwasoxb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3cqobdkgv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xzsihltr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ryahogzf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3sexqmend.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mgiwrlcf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3svzvmbkc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3pdswvqkn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3morzvqnu.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3umforaig.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ttycwcms.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ewvsikmo.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3wvscwqlp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3jjczrpqr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3cvbniujq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uflfncaw.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3cgntgnpx.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3azjwqktj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3sjagjcbi.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3kzzhshne.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3iimaomuf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3xpmiiguy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3irnwyxss.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hidgdjaz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3paqlkrmk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3onzdkvav.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qqdspyqu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3diedfpda.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hjlaacrc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vzzidpse.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3zdgktpto.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lnipcmdl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lqxowdma.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ycqnscxl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tieuskgk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3aczmeiek.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3ljofinuh.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fszhwltt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3arovhqmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdoecxkf.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zuhpqhwx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llmhlhtb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3hrrqptfq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3qggphpbr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zjttzwmu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3hqptfzom.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tsdlddnz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fnarrzgs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3luozhefz.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kjyrpvlp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vghabmbx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3orgtnogy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yvwkvyyg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpkvpcnp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhynflyp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hpznkkcj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ykhodubm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3vegxchux.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3nrdtgcru.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3eyxxvcyk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qpbhpxnf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pjafjvze.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yvodxxsc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3orhanlqv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3czoaiyeg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3wcwtvhhw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3rerrpytr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3hpeqvggy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3jllzyvfo.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3emfamjjr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3cnfbaupb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3afcxbilp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eequcpde.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zlizsgpg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3lryfoadf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3sikelmva.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3fiimodwg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mozxszjs.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3rmlxifdn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3uqrexnke.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3boxrflgu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yewdhuvr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cwsksogy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rygdevxl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3uyeihool.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uicuylbs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3risespcz.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hwppzsmd.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3syygmknb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3suwovirk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3shphzvxe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xeoymnrw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bgwrzeit.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3utetudmp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lgynkwzd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3agxyceiz.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3jgfrjckn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3tkcnoxlp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3qihiulpy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wldcgwnv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3jdgrkbqv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3jvcqwqpg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3yjvkvnwd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3raxifgbd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3lqbbznge.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3isafhahz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3zzjhpmyu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3emuhdyei.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3umaynwsd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fxkmbwvh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mizmilju.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xtjuqxqu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oastiixk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eklupocx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3letqsual.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mrbnevjx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fcrepbmq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vkeqxqlm.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3eesgkxbt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3niqwbycf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3rqihfqkf.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3byaksrsd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3rlnaxvvu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3imdpfjcp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3puxpkzkm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pewiqhhz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjsgcyxs.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bynnyyev.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ccfdsagt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3plgaatbd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dfauuppz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qaerswys.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3udixqasl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wfytuvpc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vxmvahci.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ewzgthbj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zsmegnnq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ljefhogj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3bffdwupj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3shwtynyq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xsdjytpy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3hmbvxcbg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3snpwlxyg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3qlklpymm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3hjmbttgy.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3idxhfojw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3eoxzmcdh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3djxsejec.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3rrqzvgew.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3hertttqo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iyamvzkp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3uyeosdow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xuivwpbh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3azvdxkus.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3oiyqyltz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iriiopws.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zqypxodf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlfdpihp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3gzuwidkd.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3laiomgus.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3yhjqkzmm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3cheragon.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3nsymmidt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3bilogqfe.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dlqumvri.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3iyuzqohb.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ouvnjokv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3cszstego.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3yxfdbwor.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ipbnpraq.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3owxcrqri.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3cadsvpaw.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3phbcfinm.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wlmvyvxx.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nfsbkmci.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3vphxbecp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3lmkvephv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3mslirlvy.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3brxagqxp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ucqxlejy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3cmlbnjgv.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3sqkdhbks.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eserjuwl.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oedhnvhn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3blhweqmo.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3npbnbqwo.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vfvajtlg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3dyhnxksq.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lxzhbxtn.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3qsussfuc.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bzdalenp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yqpgnikv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iaegbikw.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3wdvrbukd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nolhzbko.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3fffghpgw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3pmoiywin.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gksyjlfi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3drnxcrtk.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ocpbbhwc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3dutdydyx.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwlvaerh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ljkkumpn.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cjeockdu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ewivlwve.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gtnrmmlv.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3iqqhnene.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3fxbtzgck.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3dfdltkpq.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wofegnia.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3btqmxfur.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nczfkqwr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3douegqpd.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3tluytyjf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3iurzbwtv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3sbdmwpwo.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3ovljhwpc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3llmjorau.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tdkbrnyy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3fhqwiunv.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3kginaebl.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3jkhxkzvj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3mbitpiaj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3yhxwzctf.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhxvehzi.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3equyicxi.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3sxpqeneo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3sninrmfg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ztyfqpti.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3lkjkmgwr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjubfiuj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3srptwkrk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3eoxoqtan.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xowtvcsj.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3rjidcfkp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hogoqiyf.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3betisfrj.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3shzkxmsr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hzmmsedc.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3uxrtlsly.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3cwzntxoo.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rndtxxwn.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3bwgjayxt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3tygqzbre.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3oqdchfog.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmvruldz.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlwiweri.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3ywbczeih.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3cgjfbotg.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3fbqoptnm.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3cfzsnbzn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpoucchf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ycrxdual.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cllxnhub.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgydcptn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnuqtzgt.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cnatxhxw.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3camokyhw.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3mlbijhud.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jrpwuvlw.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3gkklyxii.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3krpeqyes.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3fphavwqi.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ohhhrfyi.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3iaonohhs.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3snyajqia.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tcgcqzkk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3cpnnkfes.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3vpbawasv.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3kznhgtlw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3flcpnjij.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3jfjyjnez.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3swikoqeg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ragykruu.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3dvkzbehf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbbsjwwo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3lprfbmuc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3zcmwuthk.html


<!-- 参考信息 -->