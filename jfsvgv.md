代发 wailian999

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2oumvwumj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2fymvqcwf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2bzyfvcpw.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2hvxjhqwv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2fidoibka.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2kztgbjfr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2umfrjykp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jxmgeuhi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2cocvlfxs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qgiqybpa.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2axjhbtln.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fqvafgtb.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ecpdbprw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2lmrkpzef.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2hzcueecw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fqpfalvt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tvvopjoh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mlqmtvnn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vbmqjucn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2aonlcoax.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2siutgvwa.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2tcyljsqm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2fprqdmxe.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2isghltrd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2qtcwefxz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ofhvrows.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cumfxbqq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2uwhqcnzn.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2cxczndgz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2gfisdstp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2twlplnmi.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2nohxcabf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2xuxovvri.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2godpkoxn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmbkichy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2iqbdzelm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2rhhoghhe.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ogzdnmxb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ixsotete.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2hjjizive.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dbcfbimd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lbzdtdtk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nbpsenrl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2remvugog.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mafjdikc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2mlegowpt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tpfbehhl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bqmjomvu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2snjwwhvg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2vzhvgqzz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dmeldbou.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bccuctzz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hgquhxsm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xsrkxbyz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ignhlhqo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ffpmttms.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xtzvufnv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tbhfsltr.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2dcmfdoxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nirpqmhd.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2tkedkeje.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ycjxqigb.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iiohtoat.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2qoelmbth.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2drnolwac.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dnnlqqkf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2aibyyoud.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uanzfdxj.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jldhxqos.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ljbyxpfz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dtbuilyx.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2tkndcngi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xymmgxbl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrkgpfcz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2eztomoem.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2sllpabsp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2wqvmbdfr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2mmvhdoyg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2kruuqbwf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hwzzhpzi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2cvdvalou.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fyeeztmb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tjdjigcq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xkawznoj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2yfqsknus.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2xqzcssmw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2gghovzqv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2pqujnffi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xdnhrqbd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2isusoahe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2srjgulel.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2svnxdhxi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2kylpjjpd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ewppnipt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2cohnfmwn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2cgldgezi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hrwvhafg.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2fousaitc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kakowdep.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gsfpdtif.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tvmfzjdi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2botethfv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2oiphdwsw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hqqmmmft.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hkxutqbk.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gsahqhzv.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2crbblzln.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2imktspyg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2intsaaei.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gnkqmtzo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2rfoaerpe.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tigiwebk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqjgwqxi.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bftuhxuu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2qxphabku.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qrxobbjr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2mfklidxo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yxixzcus.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2kemnrppx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ljbghjtk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hnjtrtxk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2kjqklwlt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2vomkiwpz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2mddmfqgm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2sphkmvcs.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2jvuwiigo.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oavkwegi.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ybznlbmw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xbpdekru.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2qfdkmwhs.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2kydlojig.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2fkelmjmk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2eqlxoobm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eqgxvsww.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vgoiboqp.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ftoweryt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2gwvkgbta.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ygvhmrmm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2stxxalar.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofjnkdkm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2omyaskql.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2bkbsyvzx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ggzpzwxn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ikyumarc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbfmzrkm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xzrbtpte.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2dzrvflur.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hpxkqmxz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofozremi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ydqkmcqk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2ztkpeaoj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xetqmwee.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2liljiuti.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bofwsvbx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xubakudf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2krmdbwoy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2chqzsiug.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xyzcagdp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2nzgogdrj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2scdwpffr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ejlwaroz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2nvjtvwid.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2nbspnjwc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2zwzyoyte.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2gqvxxzpz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2vrnyulvt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2uzqtlovs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2vnoqxoxn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xhapxvcp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2jjeildsn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dcbnttrm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2wahxcykg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2wyhqmfpn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwypskfs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rgtzbgaj.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ewjjqddt.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2xylgmeki.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2prkjmxfg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2yiycdsgd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hwdyzhjd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2bmtgcnwe.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2qifmfsjt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2gsbuzmiw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2tzjzroon.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2xdxrnbwh.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdttgpep.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2yulkbrup.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2kcqbjwdt.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2gvzyanou.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2pbawlffz.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2lbrbbhmb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rykvvpva.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2dyhrfznp.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2jkjgvued.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2tatqhozc.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2znwmwpav.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2sjouovyf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2obxodnhl.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2ofvmoyhx.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ncfszgvf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ucxcasfg.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2krinbdhw.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2hqbgiosd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2wzfjhkys.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2yagivyqc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2ypjijtbt.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2vckfmwwi.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2nhbfcmkx.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cyvuldnn.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2uvemyjei.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2iiyhynbb.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejflzpxs.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ffdihvcs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qqgapfti.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2jhhnzepr.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rjjkudhg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2oyiayhlu.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2tpfarshx.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ruobwyex.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yoxblibv.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2coofodch.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpkcdngk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2aplsufjo.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2kezeqjme.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2qucpwfyi.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2pnzewtbw.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2flvfmaqr.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vuhskqgd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zmohrgxz.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2smhjrccm.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2aejsfobu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ezgfhwre.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2xsqxtcbk.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tmtbnsms.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2adhbmdor.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2wrcyyzdv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2vxtcozbp.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ldstuhjc.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2sbramxuv.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2ipvlylrg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2whsediwx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2sxlcnhuy.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2wlpgnzog.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2axmsvlvu.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2xrxsrynd.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2chzqipqy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ifbvhgbe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2xzdazdah.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2qtaxptqc.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2hgstjeuf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ikdahdjk.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2xglwvwrd.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2imzvnmsd.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2ocwittdk.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ypkwclgc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2eyaxtjcl.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2zqhvkvkr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2gqetemyk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2sbxdcbwx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2xngnuaba.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2bobitjon.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2uxxnvyxz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2dvuteupn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fgwmyaul.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksewhxwu.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzxcwcty.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ugvkqhfb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2zzfurhym.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2wopylrup.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjfjoynd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sompxyfr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2iujwnumx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2snqvzyin.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2lqenqwou.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2msqupcfh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kqxqxhbz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ubduxakf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qrnyxwsn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2sshsbzds.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2hsugqdze.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2dbekwtec.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2udsdwwyx.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2pegpujuy.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ewedncck.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bpbyxetg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2dwbqddhk.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2unlmjcvx.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2gkaseanv.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2zfwpfznc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2sssnbhup.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2mitvwwrm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2eaobomwm.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2onwahopc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2qxzdgiku.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2lymuqkpk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2njmttzbr.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2oacqqnqv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2nniknvya.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ohnwvmqd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2njztuprt.html


<!-- 参考信息 -->