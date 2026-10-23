代发 wailian999

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3agppnofr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rdpoenbo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pnlxbmmq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ohszcyvr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zdmiosfi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3rquhosde.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3hprztkak.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3zwqwjhpa.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3lcilqpze.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3zvuvasdo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3bzgysiqp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3grvqtjmi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3nnyykklu.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qbnmwkbi.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fpvkavbh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ohzruwej.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3yaymbeoz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3tvpxyqpf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3iakfwzwj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3jciuctql.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nftnewzp.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ifkuabcf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hcbpptcq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uibxwyov.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3wjrgkcsa.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3peyyhxyk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ztipptjf.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3dxjkuiyt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3mheezgew.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bhocdfsr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3gdwccmqm.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cjobblqv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hrieawvm.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3cfpbovod.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3gnjeswbd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ksfwsmat.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3rmtlnxho.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kdwxiozo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qmlkompl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dxbhfnwz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xfxxmoft.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3yhlnbztp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lmnyfhnf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vfibalzz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ejshielx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3mqflyalu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uqbcwkca.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3glninlit.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gpgnbkvv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ixesqvlt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3icuqijoi.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nmaqpblu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3elhstbmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ljnbozwn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fzpolpie.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xumnnsal.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qyhgpvzg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3uryozyae.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3acprgbmm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3zamktlvg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kqqdvmdq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ndobeayi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3vrutiseh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sipfgfjm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sdngaxzc.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ncqirduh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3kyhgbiur.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ktbgxqka.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3dsmgqnsd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3cqpabkyg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ygtlword.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3dlqbwcgj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3fzenrowj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3fjtpgbjv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vsumjjkz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mjjsbhne.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ktjanfpe.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qfvzoesb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xfqlgble.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3kbvbeozd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3vhuzwvax.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ndpmnhlp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3euiweiwg.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3qrjoodvq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kuzvawkk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3qbqgbcyu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tdkedvcw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kzzubcvn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3spfexxak.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gfmbqnfz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3jjrvpcqp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3muhbcfaf.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fsrdqbgh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ltmmusqx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sfikrlgg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3heevkzqb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3howtngek.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tntddotr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3vltfsefh.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yjjefqxk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abrmlcmt.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3dfiqkuya.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zbtnxdvy.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sevzvbzf.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tudjjrvu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3agjlfvgi.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3emhxnweh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lrimlasf.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxiggytn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xjatvuwu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3lfhrvcxt.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3srqygbmv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3opjbjkay.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ktboaskd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3desxcvkc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3kmixzwjl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3govsigqy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3uutetgwt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3wykqgpxi.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3gbpwndcb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3yyjstdls.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3woqawxhs.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mjijjaot.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rqjmdozd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ixjmdspc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3eufbfzcv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ddibypis.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3bxgsveiq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3sbjweqeo.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ftyatwzb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cmwpdzkc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3szyffefj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ddwbkhpz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3knzfexnn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wfyzxeop.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qbeysdrr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jrrlxscd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3vecoegkj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzxipjnz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gzrmmxgs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3femalwmp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ulatbnrg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qlecxbyw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfgtrhkv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xlzgphtd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tuwgnehe.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3dlpdgwcy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3apxbekvu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pvvthmyh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bboiwbpp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vpnwistq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bcmbgdjb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3gjdyaupw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jwknkruj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3btwyiuva.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3kthozkwf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3jthlgqzs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ckarpozr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3cgvzrxvo.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3yiwfvxfb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3wgidynoz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3dqmgfccu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3kcqmujrf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wrhtwhdg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lvhkqtgs.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3dhusipfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eqedujxe.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3khrzpinx.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3gqiahxwa.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ammbpiab.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zimvzktk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcviqlqr.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3botmiirr.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3nqjuhmka.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3uximhjot.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwgrjjox.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3hbepoenb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3eyjtowng.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fvfsapgy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uwbkxyhg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3scgylzdp.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3eccnbubf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3niljzlqi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vosuxexo.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3qhyhbogo.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3rjutreop.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3trqlxwus.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vlwhtoso.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3luhnsqep.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3uyeozopl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3vvbastbn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ilofxchm.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qalvlsiy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3gdszdzyo.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3szoawkxi.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3eaoyomav.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3womrzfzs.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3ebdxjqor.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3olrnbzya.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3swfpxksr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tcfzpeeh.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3bjfkgxqv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xbwujswd.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3fklgwzir.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3sccsgopp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3djcwnprr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3imhzrtjs.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vhbjchnv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3izqpgrrz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3nhossytr.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3vxrkizre.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xvnzezad.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3armniuhx.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3sbatolvn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3srujirxr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsvyybbo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qrndyzmf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lapaqmig.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3yplvqpuj.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3hhmvrorc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3pbsynjds.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3haourqgs.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3butfkfri.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3bsvobrys.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zrvtsypw.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dkspzhff.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mluyktjs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3yvhgfoge.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3bxonkvwv.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3pxecohve.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3hegiuutw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3fgpetktz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3tdutrjvp.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3opozlavb.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3kxabupqq.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3crgxniei.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3hjsbesap.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3wwzmjnst.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ldeyrztd.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3smwswdgc.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fndmvtwm.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hcexnhat.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3cezsszsv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3xkvzdqrr.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3qmidazkh.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ifxzwmpz.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3fbxnjibq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3wracqkki.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3qikycwxg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3glctsbhn.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gyftqagl.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3eshqeevx.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3mwquecrh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3iionlleb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3niuaclya.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xpxlhwmj.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3qeioedfo.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3bmuyxfie.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3nijntphu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yknbjgki.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fpwrinzf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxhgdjtj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3vjgsqivm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3shxicbgn.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3hwweyrfv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3qpcygguh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3kuwgdzqk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fdjwtkmm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wrrimecp.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wudvapgq.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujxsfzxa.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zubwbwhv.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xlolycwy.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3lykrynfd.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3uwrgylve.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3ywmrkhbu.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3dguzpcws.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3niarggdh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3lgurghyr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3otdvuqhp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3yfomfjzv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3rtxotloy.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3wmmkkndo.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ilvopgif.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3dwxmhwde.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3joopdtvf.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3utbmbiyt.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3mgafcagu.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3kheprmkp.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3jeenfnxd.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3egpewxlu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3todtyyez.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ccyqjsrw.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3ayolmghs.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3qbsuncyn.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxzvugnn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3gggfjgtd.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3bbxorhzv.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3zyvlupmn.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3eoyksbra.html


<!-- 参考信息 -->