代发 wailian999

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3sthcxpdw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hkhhipnt.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xnoxjukr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yxgktjnn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3atwplwws.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3fepbibqv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3itqbdxdm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kmxxsxva.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3zepxouam.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gydeiqbc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xogasadd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3bufjvosa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3npxljeiz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pgsvrgcj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3sztcfipl.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ksvvwyie.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3xapzghwc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kecepuls.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3iqzsugme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wanjatbx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fwmvkonh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3fwlvvfnm.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zssxxdls.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3iowwtnpg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ujhnystq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3omvzhpgu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3nnvedzoy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3thkkbnba.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sewqhktb.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3iifhqidd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3xolsgnsg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcboqpcx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uovfbsii.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmvhkvzh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3knobgumb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qwmrawqj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3zlrkezfy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3zdpcowqf.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3axuvpvrm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3byorwend.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3yeszlnhs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xmxsplef.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3khipklrk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3djpywwxa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ufiqosgl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lpqqkcco.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3iktjekci.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3tggijabs.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3niyhwykt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3pewcfcdv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lcajnahs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3acpjhylk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3gikhajek.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3glmyczgp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3xwvxvoav.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3wkzqhbxf.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mtbhgwrt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3rqyziozz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3evtkrnoj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lbzludhl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ztclnypi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3iwykikfu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3uryijtyq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pwvhwrmh.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3drthktsp.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3kvidbmcm.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3batfwzqn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3payndhne.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zciiclax.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pabeauxv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3loxssayd.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zscntcwi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzmwqpax.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bcqdcass.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3brtmlkzk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3irkbcjwv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3phsevgjy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3oknkxtzn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kekbyqnz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mzutoukr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ffxwpvky.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3qdslcwuk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3pwgxcuat.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3snudzkxs.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3oqxwenoo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3sccqeeql.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bbzmtofk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3rrtxkjkm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3dbuctmba.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ydvugedy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3rykqkncu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fioidwhn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3olcqfjur.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lklupcqx.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wpmibfxt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qclkkqbe.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3uqnbhcfq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mevpwocw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3fccwaanv.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wbzswoyd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3aklsojmi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3mibuotzl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ikzuawxv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yfjqeorx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dcngvyxt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bffvfiju.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ubqpoows.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lxtzsjoe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3djdqqocr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3erpgoubz.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3toqqhfqq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iyzrzknj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3kqeiyfgu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zqxbqsxw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bpjhuzsg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hgqpjkus.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3iplruhxk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3szwuhwmb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zxriafwd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3wpoxquba.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3cpjksuot.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3irgzwzpy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3fyjrfblc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ehjfyozf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3bmqvaaxs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3wtntqoek.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3fytvxftc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ugyszhhi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jotwhrya.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3yrhondtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcuaaudb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3vheefxgz.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3tjdrgkej.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwiozhej.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3zkqizyfk.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3utlkodra.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ukwtqfzw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3qfgcolfe.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ahraltmu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nvsnuwtb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3iwxlezos.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3bhycbkxs.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yinnawfo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3uxamnynw.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3klsklymq.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qgydkbdv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3cxdsawbr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3ybdylxuw.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3aegvduno.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rzuzsmcx.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3cjtngulv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jgtmsazn.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sllzxehl.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pflnbpln.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3jymuspmz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3oxvzuvlk.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3jjipsvwg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tgelaojr.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3pdefmxys.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dgnxnwgr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhznhcqr.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3psbyhipv.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3teyodlqr.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3aiwtwkmk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3veghnzmd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pppszfwt.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3opxbkljn.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3xfckvulx.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3vfpzxnuj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yrdhzjxt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tsbccnue.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tugxtkyi.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kvpaclcm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3itzlhheb.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3uvmxynom.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3kiyonccz.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3evavpotw.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3jqaestrn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3slkyvdvi.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxbksakq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gihfdvji.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kuzjajil.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3qguvyrzr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ubbjkhwq.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3zzaiwxbq.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3mdiwtfds.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ayicwrwg.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ylizdsig.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zntvfiyq.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uzpbtsgv.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zfqhfkbf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3bangzgcy.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ggmydnva.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3yomtqafb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3icxgpibp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3wgffrofl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3miuxkhid.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnkznqyq.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnilcagi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3rthzsiss.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3rqgdfjoz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3ahoiewrb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3insdrniv.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3bjsomgoh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3yfnnpqln.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3rwxlgvme.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3fpetnqzq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3obixiark.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3navrjwaj.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3yeairhso.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3kgrtvhkd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ddvnmnsz.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3oogrluye.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3oswtrdua.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fakrhlvn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3fcvbapnj.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ztuylhdj.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3mgeoqnzr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3ssxlifhg.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3rjlaubnz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3rmuehbwm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3alzjirbm.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3tkqmsucb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hzdvcopb.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekhxuqrq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwhhtkbf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xzlzxgoi.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xijibirk.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3jwozmrhv.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3xbnolhwt.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3eravggkp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3sayfhevx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ytjdgmqh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3peizzqjb.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3bnvburar.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3falozkmk.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ucwtannh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3qpfqocjc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3iqlvdaxi.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3tautrjrh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ckdyxsdz.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ztypbnew.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hqdrwmym.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dkbityxb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ddnemdwf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ezfkcjhj.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3padtxtir.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ahejsewn.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3mawsikkn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zejaqovw.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3etnovwop.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3vfqmcyhe.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3lknsnnat.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hzvgeclp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3vpiwipqt.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3iopmgeyh.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3hovqwmty.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qdvtoxph.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3cmtiqxsq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkjalgrx.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3uxkagzgz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3nmtsuyfi.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3nlfmiaye.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3oktryhlp.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3pglwocvn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ffebuyiy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3cpxgrhky.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3tlvfedwp.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3mcimpwji.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3bangrnuu.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zzznmujx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3xnyymztk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3iwbzfrnp.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3zwvxctgl.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ieetybrt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwhknkbi.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3rhhumgjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dokdecgb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3btezsxlu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lrrnnflx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3fisnftyi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3qtauojob.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3plfcfrgr.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3evvteppl.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3jtkilhga.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3grooinxd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3tvunrjnm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3eiquwhps.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3iqpiquop.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3naymognk.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mbhnzruh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cxaxmphh.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3drgzouun.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3hrllbcoi.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3mhwclrek.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3rljtnnro.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ntdnfjjo.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3jkjbksoz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3cqwqjjmw.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3oogmuwym.html


<!-- 参考信息 -->