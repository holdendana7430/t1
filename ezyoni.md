代发 wailian999

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2ombyqunp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2orlkukaz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hxwdupix.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2drvpfxii.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2zlctczjm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2kdwrfabe.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2jfroobgz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2bmwfabbz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pfiujoby.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2plxkayye.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2aimkxdlm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ieleaxwq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zoawyals.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2icahldze.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jwgzqqtd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2zwgsirgi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2hyjdsdcr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2iluicgzs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2tiqwhjhb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qoexzkht.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ntftnuxj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dgrxvikw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ovzpjggp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2kkrlxnbz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dbhinpbg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dueolvxw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2tesxlpbq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2pcaklpqf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zuqhzqlu.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ihsmnjab.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2guieztww.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zxtiinej.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2dxhbiclp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2okihuhkm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2tprqhefw.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2bjbcbxpt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2xonzumir.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ugixczfk.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2serjctbn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2fwipceea.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2rgkhaxbf.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2pplpfajn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ippfmuxa.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2tmpehvwq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2hkgdtxyt.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fdbjotbr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2owbalgij.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cvpwxndy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zmpfcpoy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2xiviyxli.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gvgyjftw.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kmzgnayg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2mthzxjeh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2gybwzzaa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vtjkjmao.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kwtmuxqd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2aznhnaow.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2oanxbday.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dackoshd.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2sqgrqoed.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2sewxsogl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qeezreql.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qoaqcync.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ruhmcqai.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2kqlhwetm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2ardyehag.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kfexfmwm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2kcxmjmqd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ylqdazlw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wdaegvtx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2eerwbjnp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2esovvuzx.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pffvglpj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2ufgfxfaj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ojtgmciq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2vmnqvgmk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kuzkuluv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2weypqcwk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2rrlwxews.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cphxjrfv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2zzprppbh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2xoxjdtbd.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2valtpvqa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2chayajsh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fvogsdys.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2jnwpzymc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mdijsyuz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ggvplzcx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2iabmvcat.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2iflqjinr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2udzuyimi.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2lioajtdr.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sdqtzqvs.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2vzdvcvqb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ooqcxare.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rzrlfckv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2oyragpnp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jxmmryfj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2bsalecbe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2gxazirwb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ggbzgpqq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2gcscxebo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bamaknfv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qoobtgyu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ghbynhlz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mvzxhqwd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vgzfwtcx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rotnpxwq.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cbdlwjyn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2zzhkeglw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dxedzvxa.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2arnfpsct.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2evhusvkc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mfhuxqku.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pzjrhlvs.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2clavbijq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sxcemird.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2knidycsi.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2puzemzli.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2lqgqkemk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pcwvsqcg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2buefeqer.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2izagwoxu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2dieepryn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2sainpjov.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2xjgjbxdq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ffzurlpi.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ddcrllcj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2zckwtigx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlmcbcmf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cxucmciw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fasnpgbi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ltdmglbq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2gnnsghxc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2ugmyofzo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ygpaqgxu.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2ncimeakz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ubutguzh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mdfojtcg.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2jqqyrmpa.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ilypmjma.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gprmygfr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2lydrgqcy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iyezlmwu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2ahefylrt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ihelepco.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjzphwzk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2glihrulj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dwptaiwj.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dadcoizc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2efbtqiyj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ysuimqvq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rrjprfkv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rpdrzrdw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2cysotvad.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hjvbutph.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2znqctrnw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2axasyoac.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gulntcdz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kafszfuo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2dtgipvrl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gfzociwd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2kpqduvuo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2qmhhloth.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2deyzjhln.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2olfrjswy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2nokcfvca.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2fvyuwuzy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2aaeboddi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2emzahfyp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2baqcwggv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2ularvqqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2etpmoiiy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2czqbpxvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gdgmhzmo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2taevhujq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2fomcmded.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2gnikrrol.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnfouzyr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2haansfkv.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2jbrgunuh.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mwegotxp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2fwkdifnc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lwfwhdnz.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2mdlzinyo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2yvhwpnfw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zgnqwqfc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lwewkvco.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2dpbvysgm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2newyxcao.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2qhpcwtmv.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2qetenmha.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hqrgovkl.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2vrjfymiu.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xemvawjt.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2apfuevzd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2zjhxblih.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ibwsgbhv.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2meiicohh.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ihbxecsi.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2jljytfei.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2jayngtfw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2klsircnk.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2npasboek.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrgrtegp.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2fctrrlhx.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2unygzybq.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bksvutic.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2sdepzwfx.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dshvfrzn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2gsvrrvap.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2dtjnekkf.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2ufqeovgd.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rqkrnjad.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2lfoadghk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2nngeyuzw.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2elwccqzn.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2jwwnhrtr.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2lhnbiogm.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vyarnfab.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jkovwgwh.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2xnnpzonf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2pfrsgnob.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2mqsxzhqh.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cadhswfw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ymizcwns.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2ipyyqehx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ibsstvuq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2xxjnknhw.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bbljhima.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2qcslargz.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ihfgwfeb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2zjgvufnm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2dkixosgj.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2kphcdarc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2vimiqdtm.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2dvsmncvj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nhlacxqm.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2kfbrntvj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2voydblgg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxboasmg.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2faopkuah.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2ywumggan.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2qdgoxhvc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2glyedikk.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2cchpyshj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2yahltwsl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2xprwsujl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2aneacpwq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2xvdpkbfr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2kskieyqg.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2azphypti.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yxeubcjr.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2wauqbnzx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2kbelgmyq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2aknwebwb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2arntqfzp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2llixqdte.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2flezrufl.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2kunoopvf.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2tubnulow.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2sjnfpthx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2kjqypwrf.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2gcibjzjq.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2cscvehjw.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2squmoors.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2awjfqcfm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2gferxxes.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2itecgfak.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2oxutmrkz.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2yrcozwes.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2wmddlepn.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2zxsqxytn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2hvnemfgt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2hxgbsulb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2hbxlalej.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uwhijynn.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwdznirt.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwsnzhgo.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2jnozhjua.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2pzbaiydl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2qlpltwwb.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ohkwylyt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2ulopyvww.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2jtmvayki.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qhshhgrh.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2jtsizysm.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2sqdwdide.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gsloqwyd.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2cbfyjbav.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2bqdovidm.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2kyhjviyh.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2mqwczdpq.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2qligmgdy.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2jziuhers.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2twbutmyr.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2uqvpktnz.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jlgsuzuc.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xmjdejka.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2bmhgstfy.html


<!-- 参考信息 -->