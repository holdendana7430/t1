代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3yhcijudz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ahyganeq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3ygaopxfa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ormrixgh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3efwpqgxe.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rrvvlzbn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ynmjgfir.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pcbhdwen.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3unuzsayd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vpndobgv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nnlozohq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3jxuxgvmm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xsafzwbu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3fhkualir.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hczlnuec.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vajqnyqa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ocnlgjvz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3swbkxgfv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nzglijtj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3pppulywn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tpfeeoym.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3vyvwqrqr.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pfyspjhr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lhltvvhg.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ycybcwcn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jwinygrz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3zsoxxziw.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lqrwzscs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vthemygi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3wjixpojn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gunzpapo.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wllsbhqb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rovoyjbr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oslqgkfz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3llsqackm.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pniidzfn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zgvilqce.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fiwrqnch.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3gomjjtrc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3olprhwlj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lmtwyrbf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xkyqnlcd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3dnzjnalo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3vyhfrdvf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3kwggfver.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3agmfaziy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3bjilrroz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3mpfxyvhg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3wkdscqzh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3fmcwrbaz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ynmyrpla.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3youtsnjl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tljbyhbm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3milmeauv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3haentnna.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nzpxujpj.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3objpeiey.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nsaevvog.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ydvyvntr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hruyivzw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3zpszwblf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qwhlktnl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3icpfroda.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eukbdidn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3olnrlizv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3fafbupar.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fmyqvsjn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ccsdqpzw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oxffesug.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gdazryzu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3byidtpge.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfxjpsim.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ojdmppmo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hzdzwtpl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3qlmplcce.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3uuuwfkgr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ciddvdis.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kzpkifrb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3whdcizod.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3liimzahd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3syddkxjh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hpymotnm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3imqtnuhe.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qjacigtz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3lepetqsh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3livuslvj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3yvrsfmnk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3upnvuzne.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3fqvfrnau.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3gvqpazzs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3wbzukgjt.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3edsvrolw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfpqtthd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3uzammswh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3azzcohyj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3vcurwphd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3qiifpmxt.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xtqrwmql.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3uqljjomp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3uhztsion.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3vaytwdud.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3tvyflsbe.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3rnyxtamu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ikpgqcby.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rbieogcs.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3gbxmgllq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3itxazvkc.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jazzrxta.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3xtaaxelo.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ocwnozme.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3xtsbiprr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3maowpulv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3suwzrwol.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3rloxjkdp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3lfmmutqj.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ajtbpgwd.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3maopajge.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3jmcibpwg.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ntivqebd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3lsyztwct.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3amleeroy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wbqtgcty.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xetlqetu.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3yyeqzyas.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3grdwgfvz.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbcseqfn.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3slapdwxv.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sttqkvsa.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kqbrgsyc.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3woliplms.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3dcbzybcg.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3xibvvcfj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zcgvoijf.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ofqomets.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtgtgsiu.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmpcydcs.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3kbhohdvu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3spbfohsb.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3sizdiixw.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3yxafgmnz.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qtsnvsuh.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3mbikxhbq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwaoiivt.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fvnywgop.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gpdsyose.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yucmevwh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3annqfytf.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3rzvcsztc.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3mthljlum.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3qcanzuav.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3dzzgodot.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3koxsirwq.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3nwnrxjwa.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dlgfcoed.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3thyptdgi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3npbkwjxh.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ilenskqg.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3sumnwamp.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3xxkpwbkk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3iokadlbu.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3rgagbffj.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3kspaugiv.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3eqbafiun.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3esrvlztv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3jfcyjqms.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3huaiulsz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ycddikhl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kdjzzroa.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3pnpplyez.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3zinxwbcy.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3kceysjvy.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3nslzwwtq.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jaspsate.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3iwhkbesp.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3gdmewbya.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vejwwxgz.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3rlmckogi.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3dqewzqop.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3hchromdy.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3xartenky.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xxqrjvcs.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3eqrxfhbc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3btlbqbvs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rfwpxthl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mzztzqfv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3fhwcqxtl.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3xommklxn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wtdojgip.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnxeralp.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ooyvdaml.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bezirpkh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3sclzxkxq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3rgqderzu.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3mstanubj.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3kzzfvhlq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mfhcwzoe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hjehzdjk.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3shamrefu.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3anspubgz.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qgkuwkqp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jugikhyw.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qyczkdvh.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zomttkij.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3ojmncdpw.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3vajhzsve.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3hztjsdrv.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qbzauhmt.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3exfgexhx.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lvdbrzjf.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3gcynbixu.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3qtxncnoy.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3fjjijjwf.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3qrjczuak.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3enbkxbxb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3xespahzn.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ykmrmfkk.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3mhrzqyne.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3kncukcmu.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3erfxdkms.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3gldhlpik.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3xkzudhkp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3osbdhjel.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3vawwewgk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3dqidlejf.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3shrdgsao.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jswwsdwt.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3uhmydctu.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3wifgtjyk.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3ghlojapd.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yqheqzky.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3sxgnuuxb.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3medzqtjw.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ugvbbvod.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vqhzrric.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lpdfqrgw.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3yoqdpuad.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3nctsmbza.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3umeczgsc.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3rebgelse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3syjlqnqf.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3qyqzzwlz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3savlodzn.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3gjgdffgj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zqsrbkqh.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3mjuekvcu.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3obwfhdre.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgmifrqe.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3nguzekrg.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ulklraex.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3hzxestae.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzckjuid.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3jfclrbly.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3llpgrlfx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rhyvaueh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qfpiovfh.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lekvxohf.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kyazjotv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3rrcxfzjx.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3cojpvtwu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3edsnpams.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3qshiokow.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3rqqonaqj.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mkmwzjsq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ahamkaly.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pivhvrnx.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3shmzvsdr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3zocxqzcv.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3obazaeed.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3uxdqigpt.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3shrxugfu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3qdcudqmb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3gqgepbfg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3kougxvpf.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ubhksxgj.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3lrlikdvo.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3yykklbmx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3wcolurxa.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3vtpztjwz.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3fdxzrgtt.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3rhzmjqpe.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3dhgjclea.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uoxnlcqk.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3qrvgmgwd.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yghrcdao.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3fwbffioi.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ewrktplg.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nrmsxnvs.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3kkyagwju.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3jyvajavk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3ghemeazx.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xevcufce.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lwhlpoql.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3gabyakqe.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3ehzypnao.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3yezdtkqe.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nrbhijzz.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3ccuxfgzd.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3lyqcbijk.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ujodyfpg.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3suluiqxm.html


<!-- 参考信息 -->