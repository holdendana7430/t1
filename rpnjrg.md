代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3kwzdjajh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3sensphyq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uqqzgyxw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ksplmjhw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3iacjwqat.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ywtreuen.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ptjboxxv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ymbphavp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3snovnvau.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3cgixxzah.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pmxqpxiz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3plarlwim.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uiclvuqr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kguwgsjc.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3airdlnjx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aneauqbu.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cotrbpfe.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3mefxzpkz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nqoyhlvc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gvtvatla.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cnmgwqqo.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzomuoad.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qfoveqqq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ispnxodt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vwltghuz.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zbhcfabw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3whtmglkp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3uepxdzrl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3oxoapqxz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bgmrkalh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jqjxvvcx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ypxblrxp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3dpwqfcsz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3vyfwrswb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3sztbpifl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3eunctjyz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3arysqbtl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3eqzldoxl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3isqmzzsk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qpdoknnq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ipdijcge.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3odoythyd.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ecttbnsi.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3wappirff.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3cmhyvwcq.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nozbgvtt.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wxgrewak.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3aqwgczwm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bvdgqaej.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nvhuyudf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3pbjmknnw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rihhehug.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3celnlrlq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3jrjwzkex.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ppvwaxhw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jhlccuhn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nehflaey.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svpisxgd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3qegkjbfj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fankwfps.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dbzciezj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3larwszeg.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3pcarxnpp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gqkczuyl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rpbgkujk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3onklrsxu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vgouhdiy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cextfhzf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3zrympraf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gmqlgnip.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3mybwhekq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3urtvtsft.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3slzeqqzu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3bzwxecmg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3jvgtegut.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3danqiepy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3njmzaiqb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3bylbtdyf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3eipisstp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ahruyyxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fuocgipn.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3zrylrpmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gckpuccp.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3mvikckqd.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3snbvrmft.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3shbafwqr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3osxnkqur.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldrcusyh.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3aumjjkgz.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3fogiheyt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3qpzzomfm.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dgjboqbs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3cnslmcpt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3rbeqjudp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3grdxghzv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oshqkuzy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ktzdofmv.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3yqhxghul.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3xcxksydq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3asbxjkok.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3vnjhdcin.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jkxkrrop.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3kzleqaab.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3ieailxvt.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bfhxlvrh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3cmswiqig.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3nbmlvqmw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3wkstatqp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3pzieroyy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ewudgwfm.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3abtzowrr.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3eabzhzsx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3yvpmhxnp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jwzvgxbq.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cemnvhlb.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ydupqrjs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zqtiwhni.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ubuogxkz.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3orfskxke.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3hymqqufc.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ybhsqgwy.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kzawccwl.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hkbjaqtm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzbwcmhd.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mthbwofq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3rzldfgtd.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3fbdnbpzb.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3iitsqqab.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3sogjliqm.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3njoefdqp.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3fptjnwkq.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ycnvfdie.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmoqjyvq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuudcsmd.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3rfxrmgzx.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3uivpekjr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3pjhjfilv.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3dyncbvjt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3ajutmzxd.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3zutwoceh.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jipymmbk.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dagtciza.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xgdfvucp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3mdmjlvay.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3rvvukdsu.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3aibprepb.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3zchziufa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3csuyylpp.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3rxvteqfg.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3dsephmtd.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3sleahglt.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iujtypjm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3emwwsnpz.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3eoburfct.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddutszty.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3zvxkxmhp.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ygxpsytr.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukwuwgys.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3qwsdfnaw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3fjectkwk.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3acfqqhby.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3pbwawdhe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3nzpomxgl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zemleqbc.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3aokemmnm.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3kiiuezka.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3tzwjtqnc.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3mrgsqoei.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3czhfshfx.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3uyhbucqx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3nrnmqdbx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3nodcojdf.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3dpbkgqrd.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3upqzyyyl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3mvbtmhno.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gezerpxo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmgfvvqa.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rwixaxei.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yahkkxdr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3oiqopzxx.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3dbxvjpzq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3oeaxqmpo.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xwsceocr.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3rlfecnny.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mngjkqtv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ifgubkam.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvviiekh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3rqpuejfg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3eevcijxe.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zzfzqsge.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3yqgawduw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3rrumeupy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zhzmlzsj.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yyeguxnh.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ohgmuayf.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3hctdbhug.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3sylvumsq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ueumszaj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3gxkplcoj.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3npochasb.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3tqhwvekc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3zlvwqizl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3uzlmsfcc.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3emdklgeq.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3wfjbvdol.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3uspocdvf.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3mykbcbyx.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3mvzjvwjd.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3xjgjkazr.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3giabqyvx.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3lkzyrddq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymbzushv.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3aqshvkoy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3wyziwwrg.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3jgbjylay.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3wduzpwle.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qmpbrmwd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ptmdjndb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3rhbbejsc.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3lbhsbjil.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3btqotnmv.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3zbuxidua.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3htadykrf.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3hllctksk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3ndploxou.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3kwatqpqs.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cppzgwxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3itwasasw.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3urohdfrg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ayikhbrs.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3vlhywxfs.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3xlogqtwj.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gwhzkjqm.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3mnsfawjt.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3abyjqzne.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3aqmbwebq.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3yhxspyso.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3zijaiewe.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3ukzwanqu.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3sjtobpdc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ksnhsugs.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3jwkqxgfh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3yrrtsdnz.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eekzfpkm.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tevxpcsm.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3aaxaxicp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3ujhbusby.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gptrwsaj.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3pjfizxle.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3jljeharq.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3owwcbloz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fqfcggbj.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wfepssyt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3otusjwcy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3pksiikjc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3fqvxwarm.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3otipmmqa.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3jovmzmji.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3mqdbdycf.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rbhvihib.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3qfnqozwo.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3kvlfpicd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhzyvawz.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3swvdverz.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3taorxbps.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3servbkzf.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3rxqosazw.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3xavhnggd.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ehfaknnq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmuqiaee.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3atsldpwb.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jylkonqm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3tvdxloeh.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3jzszatre.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ovrxzojg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3jaojwpou.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ajbwczce.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3grncbjby.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3olbhzdrx.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3fzvbgyub.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3lnynnxvv.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3zvuzizpe.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3qwklggix.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3pkoecnde.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3yyezdlnf.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3imjyifoc.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3eoewjnoy.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3vhyzfsks.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3axmxplnw.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3lwhlwaea.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3twulahgp.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3zpzletwb.html

C#:   Debug.Assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3wcahbntm.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt3hmpqzuxm.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3pglamfws.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3vepjbplx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt3szyzvogz.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt3ctgchdro.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt3zwyrxlir.html

Go:   err.Error()
来源：http://www.52xcode.cn/Article/details/gt3ypchijdn.html


<!-- 参考信息 -->