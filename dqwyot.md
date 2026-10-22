代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2futzcsdx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rehbamqg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2swnwsfaj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2brvbfwod.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2tmsbcymr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2uamrcbhv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xrytvtqc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2vqnutwez.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2gliodwvh.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2suinhbsu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2gvmadzkh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2fcuwsxbl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2njzghqmb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zqmpusjp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lcewjgcz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wvcheuqv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ztnqsldh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2zgwkpobd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2eajbvpdt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wntjryzk.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nxbqafca.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gxpbkljb.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2pswcgnwh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2cpuhrgqw.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2yaqyesir.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2bgtaglvw.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2hjjmpaur.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2zajcfuwq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2eivweuxt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mndhpccu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ybbzrplb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvowrcgx.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xzhzgdie.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2xivcezph.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbtmrzqv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2jryjeumm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2hpxodmnj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2aldxctlq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hszacsjl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wjgsgyne.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pnxutqod.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2kblovfnb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2bxaopzkc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sdsvcioa.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ifdwcghv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zlswcthk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ncrbmupp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zpvdlatk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wlfcheob.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ajrcebzg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ftocxadw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hifvrkwi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dsmqlikb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pinegcwo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2nglnvqrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgivzufg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2qcokhayv.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ymfohudc.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ckkixzrb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2pfpjozhf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pcnrnkdg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jlljbddr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2lzonleic.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wtmgtlxh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gkjesyaw.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2htxrtjix.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2vtswjbcg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2vpyenppm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2xabaucrb.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eijsrqrg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jerlthla.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2uatbylag.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2byfhfazs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2mqqjaldz.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2dpczwchs.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2uterdubs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mgylnzrn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2yibsjqad.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tusgfhhz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2noidwiqo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2zqqhhxfx.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ptnoapkn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ypdfcwzf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2gueifskl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vdemoxua.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2dgtjucjw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jfwnsicr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2kbizffxg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2engkgvjg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tweshhah.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2wgbgeleo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2rrippwtb.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2bvryaamd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2lpydgleh.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ucjctfoe.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pxnuuyip.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2olelebgd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ejormmyg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ufqeevqv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nzeswgie.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dodenqfs.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ecicnoxn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nkihzeaj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xscegfpb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ihhnzxku.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eoviydzy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nyszrogv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lvqtonml.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhkmmtqh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mmclltzs.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ltlmhglh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vtegobcd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qswubbvd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2jwciwphv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fksdlbaz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ompirpmt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2bzjrxszp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2mkiwvixb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2jzkoexhf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2llggeota.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2stkzjloo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2hpwzozcd.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2spmrfogd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dhnsxgfu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qfntbnlo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wpbgudwt.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jdhdicqj.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wdwepzcm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2gtplebzu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oskbwbat.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zxnmrosc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mkpbkoxt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qnlojgmj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nlsfliar.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2gsyosvnc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gudmcflo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2gkoirbki.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2tagcgsle.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rsqxxcqd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fbslefjk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2shgawvgd.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bsxjeqtq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2twtkhjjl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dnyeeeyb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bbqpzvot.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mfcqglkn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2fxehqkmn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vfwgvhyu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2yatuuiqs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jvbqdhqn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vtnkgmgn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nmjbejjz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2jzhhekgz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2whgwfrah.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ixmslqev.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jxuffhfv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2yiypgquz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2bmedkbgx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jpnxwyty.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2skypvwln.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2uvsrslpz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2prlljpbm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2opdxlkyb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2eassbhmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsggtpsk.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2fktdwsyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnmxmxtw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ibxfniqq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2bdggxuor.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2gdbzizjl.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hacnxaie.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2kmcnwdmq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2sxtfzvlj.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2itpnsrcp.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2gzdgsiva.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2abolnpgn.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2vytsdyoj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2dqypboty.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2svmitzjw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jlvnzyrf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zzpfcncc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nybwgmjk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2gcfxbayi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2bljpbwqv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zfsurhvt.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2nhylopme.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ztuvlxzo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2oivibrgu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2juglzsam.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2yukcdcwy.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2pmcyhtgn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2ueadjxwq.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xntwiviu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kizwpxua.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2rjpjvksv.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lhgenzho.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyypkdtm.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ytvjgbxi.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rzghxkwd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lppcvrgh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2zofsbesg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2pdphxndl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2yownndkw.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2zscvxmro.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2crnlfhtz.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2gxolxdpt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfytdbzv.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctcgukkb.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2oltlxqtz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2bkxcmxte.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2suigfmyy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmdxrmik.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2fhnwtcwc.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2qjiyaxsn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tmlsuerg.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hegclljz.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztwwqtom.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rwlyyqde.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2qubhakhh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2gtaakoho.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2knutfkmg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2krxkaoki.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2dtjlqgex.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2rmswneem.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2lwcqezoy.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ldkstmcz.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2cqfuhfmj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2lqubqgad.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2mcerctkq.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2uyevgnyq.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2netgccta.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2icntmvgj.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2qydijrql.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2leieszbu.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2lhoabzkc.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bilcctjy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2ylpyhoum.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2fvctltey.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2puzkuznp.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2nkfcalzp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2eriidgne.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt2tbagmwyo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2dthqeydg.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2ktiaqnhr.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mlxsrlsi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2ydygcokz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2ksxhibrk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2obcyrkde.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2xqrllslf.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2slojnrtj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2izevlngc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2npmegbud.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2cmxdyjjp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2ctxhebpt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2btrcywpy.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2dmdnzrmi.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2yaskprjw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2xbjxhyxj.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2vkvnlvvy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2prgbstgf.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2utkluwil.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezirfcty.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cvwpjvge.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dndapiue.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2ocedzakz.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2cmzorfqq.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2buybwlae.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2vghxfwot.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tohujpqt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zychmtrp.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yrtrtkfc.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifbnksrp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2abjrubbh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ejrdahuj.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ngejgpkr.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mnkfnyco.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2stdedvur.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2mewzickk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hvoxobbn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2oxvailpw.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2apgwnlec.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2ngviscux.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2poanslmi.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2qffslgwo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2khzzoknr.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2avhlhfxm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2xscwqwim.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2lgaycjqk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2ovjukbin.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2trwjyhxh.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2aqinetlf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2stzkvqzb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2dlowjttv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2bepffsoa.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ahbpghvq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2srngfsjw.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2benblphn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2itzvskgz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ddvysutj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2mcbnnrww.html


<!-- 参考信息 -->