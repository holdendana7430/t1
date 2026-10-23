代发 wailian999

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rjwcyioi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3iwidkdky.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3otdcnjco.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3pcuaijwg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3qrogvjfp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3qcccmhxu.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3hslzbsyb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wiobuuti.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3halzxfms.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uoypmoji.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3uqhczcwl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wizvyejo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cobaucby.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pxohtjyo.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vdkyyflx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ixrqncyc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3vobdrepo.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3vmtubnvj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3trdldcaj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wdgilubx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3msqaelwq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hpmvrmhe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3amymvnuy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3urthapxx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3twhguslx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ibwsvmeh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3eogoeqys.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3evmkdnpu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fjuynkfg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3gshdmhsb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3zfiarhil.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lobxrcvu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3mkiqmcwn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3pzddlmai.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3cmuqkszp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3ukhfilae.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ntgvmudu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3psghebmp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3uduxfkfj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kofyqtka.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3mprwelmr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3qrzibimz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3idiedgen.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3sjgsmugu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3tyscitof.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nanqoixj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ulzpdzss.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lpqfvhyl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nmmcchrt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3loxpzjij.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3asjihgfi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xluleiqd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3donpqxyn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jqnwqqdw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3yeztimvt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bhgtheqs.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3xiuqkotz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ctrifzpx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3nnknlzcj.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tsvqpzwm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3opjtmfna.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cnlsxwsk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3pqzjsfof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtypnnab.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3czdwhkap.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3gcqhmbrz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uegazdhf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3hopfutai.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lgossuff.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3weulaofe.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3sgnewrse.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3viffnomr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oxomzvau.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3qjnbcyrt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ypumfqwn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3xdecvxsb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ypztklov.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3agsotvwm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3olggpomy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3siwqwmoh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3segtoqrn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3wlehximm.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3hdykcenu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zmplgbzx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fztjzfft.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nmixzehp.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pitizpsr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ugfgdoke.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fcxtsjaj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3dbfufqmu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mcjalmpq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3kgrgryhq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hbjjyuam.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3iaqlnyyo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uyjvbaky.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bofuytfg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3lcfcwkji.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ijukpuap.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3rewjtyry.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ayyovcnm.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3xzonaeku.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3nqahkwdu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zvbfhalz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ykwladxy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qgunjlyl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vzcnnsbo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3yojsrnbu.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3udjdjujl.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3malmtpoe.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3efvnilcm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bgncjrwv.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3amchfygh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wwmdzwsj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kueaaoso.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ztwkmfcw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sjfgvqbt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3chojshtx.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qgxufvak.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3klvgyqnj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3awhupwir.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ccxnmtox.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mftlvucy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mwvrxfsk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3dbjcpege.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mjmwbbre.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3abrkjbfm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3seqzuarc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rucdvfra.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yiqyejmc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3gpxnylct.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zfstwdhj.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yvrokgtx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ysiwdfih.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kevhkjhm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ufluolfm.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3daxztekr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3psjepsxm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3psjepfzz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nofgsnxk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zmwhfttl.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vqbztfaz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bdykwcpl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3jizottgq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3owrlyszf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3rvyhpgws.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3sucgsggk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cazbzbdm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gdmzlasy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tyrwszsd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pyasdosc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ymuxzfro.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ioextdfj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ppbwifbu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3giqpmigt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3tdpadptk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mapzuvxx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ioxkkqag.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3avkffjxd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yjixpjav.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bncsloty.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3azyykbmb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wuqblbcz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3fdihcqhj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ikxekmtq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3thuezaub.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jgsvdsgc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3xbqwcooj.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sljwyypz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3xwhtnidb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3oeluozyu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3scyvwmdt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3lhahjfmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktiyoxom.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3lqgmhcxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snuygevn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3gkpjquio.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3hxoerpgn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3isbeanea.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3nyymxjxu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3eerrrgnp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3svgzcyuz.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3yfbylbpi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3baioswse.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3kusiwwxd.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qkulmkua.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tqsvxrfv.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uaismplc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dygctgfd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bwlsnztt.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qpnfynfy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3xgtvqtvx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3fwixckfe.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vvfxfkmh.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vgzzntef.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ztsutzwz.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wumlcyoa.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hsmtrtpj.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3uhjdcgcj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3pihykzfd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3jyeptnfs.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3twwsydqf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iskezoiw.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3ajjvgfau.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3oxmttsjj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eyorquot.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xeykznkr.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nfqjklez.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ijarimgd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gmwszcln.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gcebxdbe.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ouofjnxr.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3uwvxdikg.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3kbyhecmp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3meaxxytg.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jllssgio.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3vjkjoxqt.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3obzgqffl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3uhdcxgrv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gjdgcmhv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3bdkuzzdp.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3cfkgjatk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3bwoefxqj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sweuvnsl.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xmxresdo.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lvrwfhiv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dgtzhura.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3fwfmwdqc.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3zxkxwrft.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3amsqsxoe.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xdzxxfgi.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3blhimkgw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3zyczcmaf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3njdemrhz.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xabdgitr.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ljaanymk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3jekppeeh.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ifvgyypb.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3kahepovv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ryxyttwo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3wqzgkxfv.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3iionsxib.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3noibkwge.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsnujxrx.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3pjnbyguv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3nmuoudak.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3lgljpwzh.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kyxfbusq.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3npskhrxg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3acarpmdo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3zgstojvj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3mjvitxqw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvlopvos.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sernmdmq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3giolzjfz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3oxtcegug.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3oohzruud.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3yvjtkdra.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3xvdtvpzi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rdpgzgqp.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ngozjate.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wazdkzje.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3lebwcisz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3kvbvunko.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xzmqnryg.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3umcxygxs.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3bhcyvbal.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3ypxpltbt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rcggmddb.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3eixlgskk.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3izempoif.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bgvntsyz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3pnzubbwc.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3pnvkpqub.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qtntzqxz.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3jxjmflxz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3wdshvlck.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uoezmzce.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xincakah.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hohubuwm.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ntgpgdsf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3bweotvwi.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3mptbauqf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ynldzzmr.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ecupgypc.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3lznysnrm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xewdiwmr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nsadtesa.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cvysphle.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3qrovgmva.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hbmzvxue.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3bngjgseg.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3imuvvock.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3vgokiylb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3bjyyvgiu.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3bduiqvjz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3rflycvfe.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3yvpfefop.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3flljsydo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ncwukilz.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3avhvbbls.html


<!-- 参考信息 -->