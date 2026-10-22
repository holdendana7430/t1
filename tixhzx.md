代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fbfuhysc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vzmxspze.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2hdhqyuyc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fealfexm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2renbhthq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2lfqiewgu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zibzlcwy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2brdofkrn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lgteroll.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zigmujfb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kfvtjlbb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2kxqyimxx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2ihtwqhmd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2tpbeylvu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2omcndxvv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ysulqccx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2efumazim.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2focsopal.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wpixepnc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2uimddkum.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2ycttldxz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2myneevfi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2zomxaiob.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2cyhsstti.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rwbhmdvl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2caqwzsho.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bdetfnjw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2squpbxus.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ceorajcl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2zwrzzlfq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ajlmebxk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2wxbhfpnh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2attamjfi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2kzktufzc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yukhyzrg.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bjgxwaud.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hckztwjo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ggjcdwck.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2fqesqodg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2avkxmlms.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pddgrjpg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2vmraxllw.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hdivizlm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gjoyptls.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2myrljeiw.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mrvguqdj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wqeagsjk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sbzpqiof.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ewxtymtq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2otjgfbxx.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2corwehnl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nhesdaev.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2dqqwlxsy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2bodwihmb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qyvekpwb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2hfmzbzsm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2rpwofegr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2eslpkbey.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2xwjtwaut.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ulahmzcl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2tcjsqogj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2svarzhht.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2fwxypmfd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dvaqbims.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2mrogemhp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2pusjvnes.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2epybcazo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2pyaizret.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2hesbpymf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lprwrsfu.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qyxgbgnc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2axxmatiw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wwvioisi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eutwooet.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ohabjrpt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehtwcrwy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2krwvyeij.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2wmvofvqt.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2awfyavsw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kuaixist.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2carphsib.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uhbdedit.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2sdtmopfo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2umunozye.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhvpmgzl.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cshcfslt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2woneqxfw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qvqvtoan.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nuioxajl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxtzkvdo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qgkbrgkv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2cxiogujs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jpjwhldc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2obvlssex.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2xnlnpwyj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2jjzfyvmv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2kgwrgxpn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2zbysowvt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2aqbnvuuq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gzfkcrbg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2grfxdfuh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ilghmxmw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2urrlyibl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2rrjlwskx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzxmqxfh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2pdixuvpw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bzolikbu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2gcbxjyiy.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2crxscnfb.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2hocxkkoc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mpvzayoy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwqjgvtg.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yybyywjn.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2mmzjrfwd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2rnhfcyce.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2axstklno.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2jmwsfnbk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2mqwfdmin.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2hhyjopir.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbckhayf.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xgvdiehr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2uxhiqjla.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2vgihnlnn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dtkgwjll.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ngchgpmb.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2zanvfqiz.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2skixqixa.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2cmvegxib.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2ibissnwh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2oektujly.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2syozgpjt.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2npzexzbu.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2dvgliovy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2nmyanfun.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qqzyjrud.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2reehbuui.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2whdclbxj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rzjwimuc.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgleihyo.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvseznyf.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2gllyajae.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2snzhtmox.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2mydxtowf.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2lzjeynhl.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2blnxeftg.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zrczyzhk.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ajzmrhrn.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ctviuvln.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2arqxtuvf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2jdkmsmjz.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hpdjkfvz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2nnhkxhmm.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2ltihthfs.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2mauiowgc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tucbmisr.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2axmktezw.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2edvulbnw.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bblkwdln.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2hoztvckx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2ykzohwwa.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2nnenlvyf.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt2jknxfpaj.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2cvzdcqwu.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zpyoopkb.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2epxefusq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2sridffyv.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mdjlfpbr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2ucrotoeu.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2zwocnbkd.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2tbjdgxxt.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2wzynmvhb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2vhfnqjkb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2ojejvuyk.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2ijgpngzv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2nmgfpyiw.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2cfuhpkgr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2lvanbpus.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2xsbmbnxs.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2avdvjgxd.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2giazohhf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2kyzwubde.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2nesosbgm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2gyqxbgxw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2bwfledbd.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2spbmcary.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xppcgxgs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2zzqaxesy.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2vprhfoyb.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2sioeglhh.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2snxnrbpz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2nbbxvoab.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2rshhinbc.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2taczrtxt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2ghavvmzb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2cecbvphb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2qvxfuwko.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2tprimsqn.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2qurmqdvy.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2mjddxkyl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2wpmezqnt.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2jrelwrxz.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2freqqfdm.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ghiiwqxv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2fyrwxrks.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2anvglwqj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2abzvlmrj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2fykgyznp.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2wazkruht.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ewegjphl.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mhaelpjj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2qttgxiiw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qfegnymx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2nwafbdbl.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2ttbdoqpq.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2mmfrwmke.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2nhfgffbi.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2auaykqpp.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2ecuscrnu.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2wgxqijsl.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2tlvavrco.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2rxzhlqxe.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2wqhmukaq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2sbovfaro.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2mykhehij.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2aeirtfau.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2icncwnjr.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2bnjqotkl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2pyajqvul.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2hitynpqk.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2qwgoxore.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt2xadpbhon.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2ddnegrzu.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2kuutpgyo.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2qhzdsico.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2tdhispir.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kwwkksoq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2hesltcly.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2yjckwtvp.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2rysbxgnp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2wcuzxrwp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2srlsoxnm.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2mrgotzlq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2haadbxyp.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2xgylthki.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2qdfrtgkr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zxxxsinh.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2zvwnnvpn.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2tcddsreg.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2kjxxcdmu.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2ztvxthlh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xmueoguj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uasrhzjz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2xerlmkvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zmnxfzsc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2wykosyfd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2yyuqsras.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2mbftbgwf.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2alpsklxq.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gbqddgzd.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2aehcbqyx.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2ugoummuy.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2ojkaimig.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmdblulx.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2tevdlall.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt2inkvlvzm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gcnlivai.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nueeidyz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wshvefqm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2hpkbluwi.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2yqpuprlf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2jlsekrlu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2luuooodo.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2xbigjsql.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2ubfyejoh.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bwkdnsyv.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hbadeqdo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2eqvwujtg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rdnororr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2nwfcnmoy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2fuiatusp.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ldakmypq.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2rqbqhsnl.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2dwtudpen.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fgcrmvzg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2leeifety.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2cwzbkrlx.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2bqhjsvjz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2anrhjmqu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2droznojh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhnstxng.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt2evakrege.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2depcyejj.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2vvmpqppo.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jafqarao.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qharuaio.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2rpgdrsno.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt2fwqwdkot.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2kriorbhu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2fddvwoce.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2xyixiyqt.html


<!-- 参考信息 -->