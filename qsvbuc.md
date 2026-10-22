代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2zhqmxudx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2epdbemiu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ofagqlow.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2oqwvjcnx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2meqbiwbj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zixdgbdd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fylyeqxi.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2tcvbdxhw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qbssjkmc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2yxxyvubs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ciwwsatu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qljrgxtd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2dmkshwlh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oufstpvx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2xdpenqob.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ptznmibh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2duxhqvdk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ohlvxyvk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rbbethpi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tgzgmcdk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mzbvnpxn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2keyznhxc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2enfurddy.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gfrickov.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zkrodjhe.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2qfepdaxq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uxnfacio.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2waddnoiq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rdibwlgc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2frcmvend.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cinhwtyo.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jkcjvkck.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2trhtmufs.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2otozqysi.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2orpmzjqy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2hhnnsktx.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2mturjuom.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2roiircpr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2zaywrwqk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2saqgxmkp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2grovzgya.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jlfhphbs.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2ucjaxfey.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2nlwkmdfo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2ivagikqv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwsxkujk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2elmtczte.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dltmzgwm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kkftmmlz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mxkfnteb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2hbjnbrhm.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ncleqswj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2vvokheib.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxujrbpr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gobbifem.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2eolqtyol.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fdtxtava.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tdmybhbp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2twmwqzve.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dcfotnod.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2qycgiqti.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2dcftgjpd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qnbhqitd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fnnzrept.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chaqxdth.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jtitlxhi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2lkrauxhj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2okzpceqv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2paopcyjy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wsldammx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2impvfwpx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2flmzaxwz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2pbnbieyd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxmaavdf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kjxwkowt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bxsfjeye.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2rvxalgnz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2manturxg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2wdrcrpct.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2aqotfndn.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2qiyklzed.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2lbqhdxtp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2gbqxfjhb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2yfyrrjvj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2wvinopvx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2buhypgoe.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2yuheegga.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2evdfufeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jecbuwiu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2zbkykddh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yzexdguz.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2cswuuwhc.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2vvifjnoq.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjftkstc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ywmjjluj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzmpcyyq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wzwbbbgf.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2tshaying.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2bgypfhfg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ikovoapb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2siwamlqp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2wlackfcx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2psmpghxt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjfowndh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2uiaxzzuw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2cbjpuqla.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2pkyrfzyp.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mbjvwfjd.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2zjtgycbv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2peazcowb.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rtsvvjtw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2objzikdi.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2tthmewnf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2pmlwwyfv.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2azdcntnf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2nyhbxsgo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2oywrjcfr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2nclsebis.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2ghaoovmg.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2motavmnu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtwzlanu.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2nlrdjvwr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2dooterxv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2aemrqwvn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rzigxmmw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2lrgnlxyv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vnodkszx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2jhfrftrr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2scaocske.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gadbytmp.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nfqbyiug.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hvvvacbb.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hjndkpus.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xdhksqws.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2hgtlrhqs.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2tmpulnjn.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2aigeedxt.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2lceuwkwu.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cuopgoin.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdsvmrtu.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gosdwkif.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zkchibxh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2fxecxpzk.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2lqvrazar.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2odlpulyy.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2jivlqvnu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2edmmxrpq.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2rtybjujn.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2tnyuxokm.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gwoepqce.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2cebtxvzn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2znwatqal.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2hdkvirvw.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt2qxplbykh.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2mugdpksi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2xhcawiao.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpidtguy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjoaceya.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2veagqvri.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2twetxfyq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2tayaclzt.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2sqhgqhle.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2ufxgdujm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2psiciqmr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2rmdkqnpa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2aajkkerr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2stzausul.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2tkmsgqyh.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2zxylkoet.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2pfqvaldd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2fxktegrd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2tmvgjfki.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2hxhcrsfc.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2oduarxdz.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2uyshwgdx.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2wkhukfxp.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2viowwcaz.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2yrlcmygu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2hhzzptfz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2wpqnuinu.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2gewlkizr.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2lozuntob.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2ixzvggyu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgagfzzp.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2xhjhdmwb.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2tjnjhzyu.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdulqrwe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2rpdbhpms.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2yvqykchb.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2fwhyqsus.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rcikibpk.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2axotixka.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkbyysip.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2newmapoc.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2razbbvwa.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2xwuchvap.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ihuyfpkj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mexuhwmu.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ergnkrgl.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2mvwvztml.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ijlxheka.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2rprzfeue.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2mlwgkfqq.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2jdbqhgqo.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2gholbeds.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2hugrmbqn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2indwqzbw.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2bqzwvagt.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2rthcvkhs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2gvtxbykm.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ipuspzam.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2vpasbrtz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2yevkoprz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2ijcqpmto.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2tlbowwlm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2jkmwqeql.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2dkzfyxtv.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ivgwhcvn.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2yhjdewde.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2jqfqodlv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2itmyasfm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dhiiebrm.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt2ilihrjmo.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2cvivlpig.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2pyjqyzbo.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2uezidixa.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2pafkescf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2hxriqygb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2bksmiycf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2aksofrie.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2mkgseuru.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2jdveruqh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2krfxwhfz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2xabmmkaq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2rvgtcujm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2epqsngea.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2dbvxowev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lumoomfj.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2fyaylvyv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2gysigpdx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mcfbsvfz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2gxupqzar.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2vxgusvog.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2icfxrxhg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2udsuutaf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2yysiuffo.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2njtxpcqt.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt2salmbxgv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2qowqsbzm.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fqkjbouw.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ktkrbnwe.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2oivgqghd.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2mqfzhcfv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2woqlzzrf.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2delvqxqu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2etddcwdm.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt2jjktusfn.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2yipubbzk.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2wpkdhngz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qcmrchyb.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cccvwmgr.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2buqmeuva.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2ymfstebg.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2djvpqriv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bqfrqwtg.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2fvnccnlx.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2fztbeegu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2caugixnz.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2qiwhlgzm.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wcpxxnzr.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2eokbejud.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2yhfjhzkr.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2bfzxxowh.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2uudttjih.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2mgiegtgq.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2kzasyfgs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2obozzthw.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfquedet.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2fxllpbnb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt2uydaqwmj.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2ggknlmht.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2dtecwpep.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dosnqbdu.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2vbkohnxt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt2calpizwp.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2zyfioosj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2dhrjidaa.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2gkvlmzzj.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2qgbadjla.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2kmfozjws.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2cwxsugky.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2mlwvrvyy.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2ilhizrzu.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2rboyxvpw.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2qbqpslxp.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ugvxcpql.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vvxjrnlj.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2fvzhrpze.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2byoedomb.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2izeddqia.html


<!-- 参考信息 -->