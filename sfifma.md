代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3zemapcxj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kohahrbr.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3iljyoyej.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3pukyxrlh.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3pieykvyz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3qzqzkzes.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3foqfzlne.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3xykabigc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ggxyydyl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3olqhxagl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ckoivlsv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jiaaqzdd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsrasdha.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3aeymtftl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3igkjitag.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3novabifm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3phzgntsi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dgtjqqqp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cevcuqyp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3buaydhiu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3apglubgz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3cktlqkjv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sglmabfs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mayyvgnd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3yeripyoy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ctimknhx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lyuxmgvu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lwpcpdzv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3niorndgg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mcgijdef.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3timoogiw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nqvoesic.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3dknyoyvc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3evyhptxm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3kwoltsyg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ggyhnydv.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3moxopjrh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3botvcrjn.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nfsbhayz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nfxoxacp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kuckdmid.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pmuwsomt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3shtmpumh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ortznsfz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vfhcblrh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3bibxoypj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3pgnaxvpj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3yjvkuwtr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3sllbkrrw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3clkxmdfi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dgimzdnq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3shtkbsqr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3itprzezn.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3lwojjsgl.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qranrepd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sencqlvk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yqxaabbr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jvvafvqy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3iibnslxt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3arbatyta.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3odklqdru.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3dpmhkkms.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3giccqcmm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3yaixzziq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3uhjvsyhg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3vmxmuric.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jwuxmjnd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3epybjpwh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3cfnwnvjj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mcoaelqf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3qviiwqfl.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3lfbcnzmb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3batoywcu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ihmhakef.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fhcyyjii.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3itatbkke.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gkqsegpd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gqlcfiqw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3rghpqifl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xfceomfg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pdqgjrep.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3hdzyhgrp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uexsodot.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oaasjuka.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wowngpod.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqfkoosp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kkplxovw.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxzclxbh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vjpjitdu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3albagovb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3bpwrtqoc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3liwynyiv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3inhvmndf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3aagulapg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wqlljkpo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3pycsxvkt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3wgyszqqy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gmmaxgtl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3cadtwzrw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wywyqehw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jtjgugfg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnadplia.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ntojhbnt.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3akeufvvf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xpmbhxwo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3bdbollvk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3byhvybqe.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xgnjarql.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3mscjajuj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxvaaddi.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sifbjjse.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qvdbnkdi.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jlffdllz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jxumxhcd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3jezivzni.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rxcfvrzm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3ourvjwdc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3iidlvlfb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3svlnxfmk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3srymfuby.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dpdxyjqi.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ypgpldxe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3dyjzozuj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ldspsqpf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eklfgdbs.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lqpigajq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3hsdnvpxc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3foenvkbu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3yhenjvfk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3etgxnguf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3govwllqe.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ryxhgbqw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3xjypggbx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tnhcqgfb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3nyrlsbdk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ekcnkmfr.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ayqbhyya.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3cixrcqmg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3uuexzflm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ygxtkgvu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3zbjblgpi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3slwfvwjj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hjdwskwt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3nqedpgdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3varqxgux.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3utibmaow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdfwruid.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3iqvueced.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ehajbkdt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3nsxbfegs.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3swwwnksx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3befgebzm.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pefasupu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ecwnsdgq.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3oqzwpxuw.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhniybii.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3zvvqnmxi.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3krdikwwc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qiajfpms.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ygggyhkm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlwrhwdk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yxnyqtyz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3jbqikjxf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3hftluyls.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3laopkmpo.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3nrqdtfvt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3veydjpyg.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3trxszcvn.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3urdnfymb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3glhrdlxt.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3stvzcqyv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3amowdsji.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3avzakpgc.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3bplodmwi.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3zkxwliwd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3xvoffagi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ehvllwxv.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3utauetuk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3mlycbvoi.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnraeppq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jkswjztg.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zksweogm.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qfvndoaj.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3zieapluy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3wonjkgcv.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xmquphiq.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3amtbeziy.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kvbvynqy.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzxlhjmo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3lptbbvir.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3igkgdhrd.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3thgjwdkg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3navobgij.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ukgxoqbz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzucdiol.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3xafmtsma.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mrffwnnf.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yqjjemnt.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3nsxpemfu.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3xvtcirkl.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3mrygbyaq.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3xzonhwju.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3htnlgdjm.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uojcfxvk.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gkvpobdd.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3yynfrokt.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3uaguxmpx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3pssymipz.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3wcrjyvmm.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xfdzpzff.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3marmvqbj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3gareolvn.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3usnqgsxx.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3fixnviyl.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3jftnbdzt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3lmtmcpje.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3ozgrqmkx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3yqnaybyi.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sbuhxshv.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3oxheaqhr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3mfospmqj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3leblvjes.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3uvnhvaii.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3qaqhbnmo.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ygdgwabw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3iiqpukcr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3amalfurm.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3mwkooudf.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3abslvgle.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3siajzvul.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3bkukihzb.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3wyfcgrtm.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3oqipxrvr.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3dzmqrwis.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3kbvdjoom.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lrowzoer.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3afqlgtfi.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3vrfgenwp.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3qpycgmjm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ydibudib.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hmrlzvpq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3myoizsld.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mdionbda.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3pvkqbquw.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3rnmpgrgm.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnfwcirq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3tyjkzvsm.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rfdphvie.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzlawmad.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fclhqnlr.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3axoinrpz.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bytkwwrd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3alhvdrsv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dtxmdaav.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3lpbnkrzv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3clwdypfz.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3zsbbavpe.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3viibslbx.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zokdxway.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hzdqzxjc.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3mxahcjvp.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vevnatfj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3npidmuff.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3gcrtmehk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3yqfvvcqt.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3nlokyary.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3zqswrncc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qjbxxfpy.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3dmhzxkjj.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3qlutdbuo.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3qdihfbnb.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3oqkvckgb.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3qcmsontv.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3zmenmvjt.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ksfxtbiw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3beduzvvi.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3uvlrzafs.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oeparpqm.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3mjzeaovb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3dhzvozyz.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3uaogpzoo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3sxnxhdis.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3aukwaoqh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3tjkrbtss.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3kwvgatdj.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3puhdbcdl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ixxbqdxu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3tyazrrni.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3zcllunig.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3bkysyxpf.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3snykyipx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbazkrai.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3clokkuym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upulsfsx.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ssercswp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3pxnxlhzb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3rccbcqbk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fiydzifp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3dmslibhc.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cqigczpg.html


<!-- 参考信息 -->