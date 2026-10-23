代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3exfmfhzm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sqmkzckv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3pvjytptl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3sqwnpczr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3sxwuycpg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3quwjunzx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bkhpthsl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3xjblgrdw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nyjxzlws.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3mckoeokj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3loeegukx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ezylnjdt.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3eqqgblnr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jhlumcdj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3gyjptjun.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3kiughjuw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qanwlcbz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3qaoobytb.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nenibmai.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hnumfwoj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hgvergya.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gbjvpgmr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3bnpoyssc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mayhpdph.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uootiprb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3otewowhc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dfqeorfu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fogwavmg.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cishwrkt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3huxfvprb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lsmxlwjz.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3parqtzyr.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nrxxjzav.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fmqkukva.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3sfyhiycz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gcfzteof.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ugefokqx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pfugvhmm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mnjncruj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rhazomjt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3gorfents.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ziftfpqe.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3bxbisybl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3uyppfwmc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ccgctluj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3cfkhljxp.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rtthwbou.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vkrswppm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wyzyoyvh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wzixnvwu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3yunilwgl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3yuljnkfk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3vbutknjm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pfwranus.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kueqvfpu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lemmacic.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xomyglgj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lcevnzyr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3cpzzdwwt.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tvgpwfqx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3urcoekft.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3xzkwpmdn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3twhbefht.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3evsxnxbi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xweygrek.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cuifncil.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3zmeatzgv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bllikjxg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3txweunbt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gqlojxkd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3dxxnxhgh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3obdxvihp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sabtgtdx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iwmxrzsr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cntgdluq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zguzbbji.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3kcxolelw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uxbwrubf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3xnyiiiaj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ocbizfve.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3qnwkzymg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gkmnvceo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3geitjaoc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3bnonuxuk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3sbxuqnde.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3ywzpsopp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3mrfdlceq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fpmqruxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egujixmb.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3hpzdugog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bycgqcvl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3dzzangie.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3njxvelrf.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3qtjtheoj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3noixqxfx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3dzgpycwp.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3muoelxlv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ubrmlwgd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pitsulai.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zilonolu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3gxzupxdf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3hbxusbfg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3psjbcutf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdvwlzou.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3erssthhb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjqxyaff.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ahdgdlcm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ggfngljb.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdwecsgs.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3uartjtts.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3aproklwo.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nyaousuv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3xqqpwavn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3apogvext.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3zjlkcnmp.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3yospdezo.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3qvmoiqei.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3brtmbhss.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3vzjgrvsz.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kfaxrslq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wacjfcwx.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnbuliwn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkrktjct.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ovejyaxk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3hhfqsopj.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3loutmgzh.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ltuvhisa.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3hpkgkfmu.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3uawvmvzu.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qleopskj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3oxytowtz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gosqjzki.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3dmfkpcny.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3xnwgwjso.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xmsnmxqj.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3vtwfxrva.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3ergdosml.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3gwtspuoj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gitwnair.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3tpzbvmea.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kkactdji.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ezagaffw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3hmnoprxi.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tvdoickk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3imnccpil.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3qkxactse.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rfvgqrdi.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xcdxngjm.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ydlutzjq.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mrjjniuq.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3kltlfkpz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3olhqiepq.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3gkfdmffp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3axyxdajv.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3toqctqvy.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3bpmnvqzz.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3aiyeyuqw.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3mwusrzhm.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3wyvnfpga.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3lknrwkhv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3xvfeocxe.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3piaftdkt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vzxvtgga.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3wbudrcrp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3qlzsznzr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3uflvuqwm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3trmssplx.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3cmwseefi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kkftiopy.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3yizrnphf.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3vlmxqihd.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jfilmfek.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3ybxxgvet.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3zrteeeei.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3mgifrtdn.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3jnuorndj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3drodwzgc.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ghnjsqwf.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3epmdwtie.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3odsejahz.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3bkzwylkm.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3eqnozwoq.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3nvglqmhy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ivlblkzg.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3htycxjkq.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3qjjccrfd.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwhhkxog.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3efvlexjb.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3yrobxmjj.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3krgmtsog.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3pkeijgrw.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3eyqarzks.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jhmtpydn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3nzjnsnhz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uyejbyyj.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ekwmfhne.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3mmxesdke.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3howdhuhn.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3oriyoekz.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3jyxluujw.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3mkupqvgx.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3wlkopsfq.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xwkwwhkh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3tfauxkza.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ciituriw.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3laejlmye.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3kwiedwee.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3hzhodndj.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3filmxfdf.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zedidmfz.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3twvgwsdg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3mwsdcwvt.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ziepjwim.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3dqfkmgvy.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3kcfpvygd.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3dekekzsl.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3mnohxtoa.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3hwefcgrv.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qlltxvim.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hempoctj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3klaijgxj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3bhcsfbez.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3veyosagw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3jthsvyyi.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3rxtyyees.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3hvofunrr.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3hjztfwic.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3zxytkrit.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3gqynpfrw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sqcqxdkw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3hgroaypc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3vkjupdpy.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3xknacrwx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3pdzbmzxk.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3vfuacups.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wrdozmga.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wjygxgol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkpxddml.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3ifnrzkiz.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3xhsgdzbl.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3xzfthpww.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gyopjnhp.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3uktbknea.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3cjumjdld.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3phlpstwd.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3voiahsou.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3kibcuavn.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3jycwfcxy.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3drxixpyc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpymboaf.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dtzkkplx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cuambkcg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3minmkvox.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3nyfcyvrc.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3laidcwxe.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xtmjaltt.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3pzejkmwa.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3cgyfihao.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ybjrudca.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3niubxgzo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3swsigpbf.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3dlzjsvod.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3edfygbdr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3jjtahpfg.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wudorgdf.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3elilrvco.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3tgwwdsmy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3yajiqmwz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3mtwyitap.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3katfbdkl.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ecfdasqb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3uvemjvzi.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3mrcfsrby.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3sssjqsnc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3pnzcsgni.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3radapdiw.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3yjjplyrc.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3azjmephx.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ogatkunr.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3vvdghrpk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3cymcnhaw.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3wmrnxoyw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3vwbaotfw.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3uaextybv.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3fgzxisba.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3euugidhb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3mutzgfci.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rzminovb.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3zyryjtge.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3bfggricn.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3zanokawu.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3ugqblspg.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3yedwewyo.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3ppvmpbpd.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qjbdqjiz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3prspvwbf.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3psxxyqxu.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3bhqlhtox.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3dwtxrqai.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3rjtahyzj.html


<!-- 参考信息 -->