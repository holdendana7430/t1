代发 wailian999

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2qqvgccmi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xzmwhics.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ekjkgmkl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mcsvcgtq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2csvbwzns.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jhicsomx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2znmystmr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2ifvqmgup.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2thdyvrfn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qxxtiklq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hfrukftl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hhocxmsn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkklqgjx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2jovvykie.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2gsacptct.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2fbdcvotz.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2tfwbiytp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2erbpcjnn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2rxbtwxed.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ysvlezrp.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wdyzeejj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ivabkrtm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rbstcoly.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wrmotook.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2uqflocuy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2blxyxnoa.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2oeweopze.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ybasvefg.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2faaiulpp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hselmuks.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2nhexraqo.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jvpnhyce.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2oogsfubz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mzwlfacy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2wlresybk.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2etayqisk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2faruadrz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2azxcjxte.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2cducvubs.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2djaqdoto.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2zaqoqtbg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2edauxers.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2raybqcbr.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ozjnsyqq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2megxaiao.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2dsmuaqsx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2icmwhevq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fhukmdxt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xulcwili.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zbqfcpmo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ttddzidi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xmosezyq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2shywfenr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oxnkcadq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gvfwysjr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2smmvleoz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zqspbqir.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gxaszjvi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2dnbpgrav.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rgoxmkiv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jmrsflme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgmxuzuh.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xodptqpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xyiwplkd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2usqxzhkx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2kxtyrxuz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kxneusyi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2pkcghxkk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bdiphubc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mqthhnwg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2zukyfyyu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lhytctse.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cwtssarc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2lricsict.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2cfhckcli.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jnhbwjdj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wjtexszc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zoczmhfk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zybgwhvw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2pskmjwfl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2kahfdijq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2hdxxygko.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2jrmqoizb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ldausnnc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vdgunesf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xwqzkytz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2dlzdwuxy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jstqveuj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2yqntrwrs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2vbbytcjq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2opcvvxwj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2kbokbdxu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2siacojvl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ydtuqktu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2alicidwj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2blfhwpqd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2kywpjjbq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2arbocnod.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2mgllixib.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2xkedkvug.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2kprfcybs.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2igtiyesy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2urzpqnif.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dqvlgblf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ujqwkxun.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eskuzovw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zcicuhnm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bqngaiif.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vaezeeva.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2wwugeoku.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hmvtzgds.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bypaaono.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yannjhbe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2owameqdp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2peegkqag.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zokbdrhg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2brbawzih.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ifavxjsh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ocaqvizo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2plsxkotm.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2bidkynav.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ojkrxywm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2imrjhahs.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2llvaqszd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ccxowbry.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2crbustea.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2fprmguhi.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2qoyqyedq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kshfbzux.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ceacfqpn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kajyhthj.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2tdcaxdcj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wkbtrwvs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2mxlxxprd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2drjzrpnq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2homkvhwg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2jpityuhw.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tqtsutyc.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hpcwjvcq.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hagmcccx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zuanngxv.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fadbztxa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2omkmildy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hicqkqud.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2lyogihgk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2tuwybrto.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mbadlogg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hhapoqvn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ttaligcl.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cizqjdhh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2gajfvvvu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2opiufsit.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aulmkxbb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wawixtvl.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2cuyvplnm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2twybckqd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yeularfv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jbaozgoq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2heyevmyz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2aiixrqqr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2ehizqzxx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fclympab.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2jxwacdep.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jjvmliuh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2emogoeyl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2apbqaiqh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lwragxmo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ethyswwt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2edvawdzb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2stoiyouf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2amnhjgia.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2tvlyyfdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mgzpjqve.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pzeebogg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqvpgyne.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2xuxjvupt.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2gwtzqyxa.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pqyhggws.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2koiuaiov.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2miguvdqi.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xizwzndp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2wkfhsgxu.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2ovptlktf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vmulpons.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2bqpkfckj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2jimrrqlw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pbzcomfy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2akrqpzmi.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dccsxuuo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2pkamjgrk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2wecrbjqr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2kgafdbxw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2rsvwksap.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2auhkmomx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cnzfbvvx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rwmgrypw.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jnzxmtqy.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2ftafxkxe.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2vezxekvt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2yovmkscx.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2foetxysc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2enclqujs.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2cequaiem.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2unipbuxz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yqdcmzao.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mgoibvty.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2orkywzht.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ftyrpgik.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2mtaefqxb.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lgsbxuat.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2fqyfbibm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2hsyupoqu.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2yjvivygd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fznirnrm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xnyvhaez.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2hgtnfgod.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2myoostyr.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2avvrkaaf.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2udqwwssj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fmhkxkax.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2jxxkalze.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2lptaifzq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2suiftumy.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2gqrudbmm.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2snnumqjx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2elxjojey.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qkjkxvcv.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vxzrkggi.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2jbarfpmc.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2bkfpwzfx.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2rociikju.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ysosqnse.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2lthduauk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zofvfrde.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ylnxupri.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2afmvnzek.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2jtrwcqnm.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2owtajzyy.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2tzoposcs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2bdfnrhgj.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2znynfold.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2fltkrhmv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovhigkpc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ajfoxmyi.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2tigbdnch.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2idrrdojs.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2dzdowehe.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2lqbioynb.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2ftlvlchg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2hryusnci.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2calfoupp.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2zdncsogy.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2xjjtxwip.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2atzuouuq.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2ummokrns.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pgfjhyzo.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2cfpvvdgv.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2pgpgshyo.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2hjaqzses.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2pgtlgppx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2ersejrfy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2tekjbgoz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2qfpdzsem.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2usccueem.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2lbzzbniz.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2iluhbiaj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2dbjpdtcj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2xjhrwaux.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2mdkrdafe.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hcradkpn.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ywykhmts.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fxenqpif.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2mlogomjn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgpsjfhb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hlbqiivn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rbycfkpu.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2salchher.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xdjczpat.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2sjeqdcxc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrrcgtnz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rbzuwtsh.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2wfdejyxi.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2iocukmyk.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2fecuphpu.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2bpburjig.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2bsvnbheg.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2sfnoowvd.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2xwfcnkyl.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ielnaukf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2fterbbmz.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2raeauxar.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2gpikylit.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2tqtwyhcr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2lnfqhixz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2fxxtmrch.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2fougvprv.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2uybdqlbn.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zvpkbpmu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2oehtvhdf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2mpovezbk.html


<!-- 参考信息 -->