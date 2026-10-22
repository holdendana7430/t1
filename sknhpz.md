代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fywkwcil.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2ijtkrrck.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2byooewjq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bddbipil.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tvnfiagc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2wqhpzemt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2gtgeykun.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2bbeknnld.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hunwdqkv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2kogidzmo.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jbuodsxj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2llabvfll.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rjotqerx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2oytdqzgq.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2mpbzlkoj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pdvmlkcq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qxxgndoy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2etpqhtds.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2blbeyipw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nxzhtopx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ebkgivot.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xiyyspbj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rtcqxdua.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wwezmdwv.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ahtxpliw.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kerzwahl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2lnuymvzq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2gbqkdxsq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2cjfqcigt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2weecpdnq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2stlgjiug.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2kowdkeed.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2lhqzumxc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2owdpbctu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2lenfezsc.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2bwbmzdls.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2bwnoqhip.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2nmswqlxa.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dfdxzvvv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2rsnfxcof.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2kzegwpeh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2dojiccsp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cgtqcfci.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2udcsihhj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qcvcaulr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2azzupceb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yvbrvzat.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uorfchby.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2dmyuehmm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lipzjzag.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2efxasffc.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rouadixd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2fooinebr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2nfnsajyf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kfhjvmov.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vkmivsuw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2shcsicak.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ksclbzfj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2loaubnwx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fsevvfyx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vbmkawzx.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2icveazlu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2tlaxqygf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xktqfxch.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2neyfhhaf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tghjruiz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ndskcbqk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2sfhseyxu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2sytopfsy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yvhvkjqe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2lpoezhyg.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2tjqwahdw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2fjcwnuzq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2crizhesr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2yvtbscnc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2gmdjrsle.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2euydtkgj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2gxmubamv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ypeikipj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2jczbeddw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vjnwmzbu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2mbikikaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2twahrgzx.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2qfehxulj.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2aifdckjm.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mopqbwcl.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2upheonrk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2dgnqguxt.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2utwxspou.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ajhkypvb.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2khodrvcg.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2gdfqyrhs.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zxtnwsgb.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2tgmrwqax.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owmgpyzm.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ygtgzcwn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2kmarnpaz.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lptkkmjn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2gcztsgvx.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2yysjuiul.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rbprzyqf.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2matugbbr.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ufcjknol.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2btiykvso.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2vmezmluf.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2dlcrgbbf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2plisxjur.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2cljrozih.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2difqnfkr.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2yhnyzbow.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2yyrymgev.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2nfdroddc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2ucilkhgj.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2rvvpatah.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2ejsndtpb.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pvmwxnrs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2lnarhuqa.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nnzmxmaj.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2xaewkpuo.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2geyqtbad.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2wxvhyqrh.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ollovfzc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2goaxbvrk.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2dvlleldl.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2fyatnsww.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2mlxvmrzy.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ijskecgz.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2yzujgjwb.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2hkuuyvom.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2iyqhpvoh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsskynjc.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2zactiyrq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kcfdmpjp.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2oxkwzipn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2uucgoixs.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2vqjcgaxf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xdtabznh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2cmwghdmg.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2tlfjxgcc.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2mjozpirf.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2qwoztbhy.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2dwbgevju.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mxtxxzgw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2uwtjnbai.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2oiupkaow.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2wizfkemu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2lcidlihs.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2fdjhaulq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2cthrjanl.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2jvkthrhh.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2tsmgsreu.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2vrxbvsse.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2mefcsgoy.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2ifritbvd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2fiyrxueu.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2rsdednxl.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2frvrrabj.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnvkbjki.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2ltrxbtpl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2xwynfleb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2maxucopz.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2ucuxdluo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2oivbqciu.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2psluwpss.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2twbjpjlu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2mhbsgyhd.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2jhnelskw.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2twviqjys.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2egjuzjxt.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2iqszxrhr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2adwqfjil.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2iyandyle.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2jawlafiy.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2inmbjuie.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2oribjxxx.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uovvgbll.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2wepuquxx.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ekonfegi.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2cmudonho.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2yspngqnt.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2lklnxhji.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlmmnzog.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2itefhqzk.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2ukbcenja.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2cjpuefsw.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2yvrisalx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpdcqnjs.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2qmmnoiqc.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2akybnxyv.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2pkzrooof.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2rbxjtvmv.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2tixjorte.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2vmcaikcm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2whuqmoij.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2kdfjrdzr.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2xtcvdsyn.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2llzlnfdj.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2tupnzpcu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2qlnklshk.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2qqwshujw.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2hrgpbbsn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2cnojscmj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2nxgrkwjl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2qgdednjg.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2aegocmyj.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mmrbsbcn.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2brfnujxi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2wcgcvlra.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2pjsairor.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zutwcavk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2ghqxyxqm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2hemjfqyl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2rlbflktv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dgtraust.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2jgtjdybl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2etjssssd.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2nqgbapbn.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2xpucopuw.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2jnsxgbqq.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2sudqskwy.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2rlturvnk.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tfhxbtqc.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2tdoryzye.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2zkxznprh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2zuzorjdn.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2ezolfguq.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gavdefkn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zlvmdbgr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2iznjnqrs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yrwvfsyb.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2axzkblaa.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2ztqxqfdq.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jwgehsec.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2yjnzczlo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2kzcnxfqx.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2xfvbjxej.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2jogukquo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2oioctutd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2cmgbltsk.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2sibjaxip.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ialifwua.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqkyisud.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dsijjstj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdkhwybk.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vpptgfuq.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2aqasrtpt.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2inrbaiwt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mvdnllwf.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2yaqweuaa.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt2jstmpvch.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zotfuutz.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ieytfutd.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2whnwsrnv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2cdjrhhbk.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt2yaarghbs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2zjbjwmxq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2sshkvpii.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt2tfzitybq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zpexdbfy.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ccwkeljf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2sizfyjah.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2atoalqbh.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2hvesnfdo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2wwntjmen.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2xfkcjdha.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt2zfhjudtx.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2aokouroo.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2bpntyiep.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2gccylwve.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtvtbwvj.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vndkpsdu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aagigkrm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2eaajhium.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2wgiqpobh.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2cmcgxrpd.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2swidtqcy.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2lsxzxzpg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vqqipxjx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2pqmswrof.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2wpscgxhn.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2nnlubjgl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2voujxcyk.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2xbqsoutm.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2kdpfzkyo.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2eokizbsa.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2gakqnyfm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ijciwjpx.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2gffjqqtx.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2vkimokxg.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2mijzuunv.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2ifnmacjw.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt2jugkbpza.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2wqashhdp.html

[H08] 获取错误信息与堆栈
来源：http://www.52xcode.cn/Article/details/gt2oiurkncw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2ocivayry.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2crcwdksx.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2jpkdoawd.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.ydjk.org.cn/Article/details/gt2uvesbocn.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.ydjk.org.cn/Article/details/gt2aftutmfv.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2xlslvobi.html


<!-- 参考信息 -->