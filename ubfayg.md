代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nhsdzubg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vdgviygr.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3lmykgvsb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fhoibkzn.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kaaojlso.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3nbcdzysy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3cuwapuse.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3esbntuao.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3blmcupcx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3rwatobwq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3axdhgkpn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3juimldcy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ofonbroq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3kzcjwqly.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3nrpzmqer.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3bnxcmuhs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ytoiaknj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3bpzrlfrw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bupibjow.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3liuovucs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3dhbsmdku.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3shqxwcem.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3oouirhxa.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3hmvleizp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qnzgbcpe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3wvffuuuf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3szbvupvu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3auvfpiuz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3qyrvbwab.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3kqrxroja.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3qxxlxisi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3stgyhgbj.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3ntgomrvz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3bfxokliv.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bicheymo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sosctpez.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rsftjftm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nxemffqc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3tbahqysu.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vctvogvj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vypzddxk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3wosxeeqt.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3siklclwe.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xslsihac.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dlncvpgm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3onshepsb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wqhgmwap.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lqdoiara.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3heibfobw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ljnvjcxb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3kuikttnl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xfgshinz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cmpxtqhe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3uugjosti.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mjqxtnug.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3tfjlxptw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3hjksikcg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3poeqirja.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3pfpphtlt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ujhbgmgu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3issggjqp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3egrlofsu.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3aqlflelk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tjsugmbg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3raoxgasr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ujxjrpzx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3iynivqcc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nrjykzfn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3enriptsk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lmknkfjd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gdnxcuhx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lbuudbmn.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3oribmqfh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pizddnsv.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qxaqtazi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gidkgbtt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3iijddcfj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3ysggytvl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cnqrhzcg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3inoixxha.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iumzgzym.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3anunedrc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3gzyywwki.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qfuautrd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vjadnuiw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qqzjlmaq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3fifbtplz.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sknpfycg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lvgmnsmh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqlluwdm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yaiwbodx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gzytdzuh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ykvhlmeo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wismdxgy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3csgrndaz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3hxqokjro.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3vftlvhae.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3xqwwpycq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3igfngdxu.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ahdxiqtp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3fcirozhg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3jntdinfe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3xjjiliyb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3zjerexvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eujeuorp.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3varmnwgq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yglemrxm.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3xczypwxg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3jeqfnbrf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sgojfiyn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tniznxuu.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3bbuqkrkg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwooiaov.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3stlmixbu.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3tkjpktzb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jfxhtxcx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3hcdfuccu.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3fbffclvq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3wofevqrz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jnimiffl.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mjuwsnnl.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dohmkcit.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3phhsxcqt.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3dtnsyicx.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gfnujkme.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3fsdzalxt.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3tddjmmkc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ubrylwqr.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ocmxkpuk.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3rgequhzp.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ypfxrhfx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3dqmsirct.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vbvobeab.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3cnmfxhfq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3riuakvtm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wsxmnhst.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jaxubqjr.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qlndujuq.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qbnjxoau.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kypfaodh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ptivzgqp.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3itswdfuk.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3wzhtqzjw.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3ccdxxjpy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3sclsmjch.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xssqpnvf.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zaumdhlk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oivimkjf.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dhcflhoc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3rfhmzpui.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3tkfbviwy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ztydyjnb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3wxllxxnf.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3cphrtrcl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3chbkqoka.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ltabbcwa.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3snuezcwa.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlbjvqhs.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3paufkrhy.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3zykkclgy.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3pndmpmxr.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3stpwkwpz.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3pwvtxckx.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3joyfrulc.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wuqfbkpe.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ezkcsejx.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zpofbkde.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3gsvcxtuq.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3zqvyvurj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mgerjtiz.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3fnosckeb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3mbkgeaar.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3oivautbo.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3nndkxwub.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3llnzahhd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3vpwhzeux.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3gyrufcgw.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3kehtyiwg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3nvmmgbki.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qwoyptmj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3cwcusbjy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3nhwblzkc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3erwshvrw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3lzktcfgg.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpxvyvxb.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3hpfcpckt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3rchskccw.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cimmorit.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3bwsxswme.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3cuweevxi.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ndfmrlsc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3hpvqtxvh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3njadwrbr.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dtjvlsjb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3npabwvlg.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qhurkirp.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3kajttzen.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3rnpyybzu.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3bjttglct.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjerjzdf.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sdltyays.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yeaxiipy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3lwwoknbz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3qtbkqemx.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3hlhggnkx.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3acmlpgey.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gydtfszz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3sprvocpn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3drzxmdja.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpazkksg.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xrtjnrct.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ucpnxfcf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3tyakjdab.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yohkgpuf.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ahtchvul.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3omgyabel.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3ojugmskd.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dubpkqtp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cysbiprt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mbnfpntb.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3zrcvshne.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3khvyoluw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3qgzxpjff.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3dvkivojr.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3sosgwzuv.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3nxesxygl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3vbausifb.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3tkonzpip.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3uyswgbkh.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3ogrfsibj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3ddvvllon.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3iexqomee.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3keaniegq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3trusevfl.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3viegzngq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3jsdwqipm.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3qyxcjfio.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3libkmfup.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3juquweug.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3gicyenfv.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3bqjrmivs.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3sbpfrkvf.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3pwcjodce.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3zofofgvs.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3nhkkfddl.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3viczbwvl.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3idjvkkna.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3oshymqmv.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3qtgcvbwx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3aqjqvwgc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3sczsyrgy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fenwptzk.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3cqyenbye.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yuezabks.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3ogudocus.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3rlgplvwr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xpygiotn.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3awrkczqi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3zfncjzzs.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3aegdgief.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3kcngdoch.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3caqdmxar.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyfzgfvv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3mgiuxfed.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3obttlbwd.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3epjlhqrc.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3umvkzyjk.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qykbewuv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tyixuxdd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3jyslopku.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3xdzzehsu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xsiprtuj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qcsbfiwc.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3bhgetgfr.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uwrvzxrk.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3efnnolvl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3odsoiypf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3dpddhpnr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3povpbndw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3zixbwnnn.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wrcifcfg.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3sglthrfn.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3btfrzodd.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ylkkyckv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3bjeixiky.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3iljwksyn.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3zrjjbaki.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3vcwxwifl.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3qsfrmcbk.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ugykuvge.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3fmsrvuha.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3mqrzlvlc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3drvxblap.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3kvhmufdy.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3zilgqkvs.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qsddbpxw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3cubgnrwf.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3yvvarlvf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lickfbzn.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3mpdvzfsk.html


<!-- 参考信息 -->