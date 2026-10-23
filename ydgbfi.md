代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3thrloukd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3piccoibi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3eubyrtzr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3keajfpkd.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3hxrxldbh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vrkimgzq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pfelrkce.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ghomsube.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3piyorgze.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3lwjdxutr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dsrrdegg.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3vjdufwdt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xhddzktr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nbjzbjdg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3yeryfnuk.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nmureoen.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3cguiuzcu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dzvqeecs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3sxpojdfm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3asjdykds.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3gtvefcia.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3rqwmdxeo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rmxatejb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zlciqpyf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3smqbzvws.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qouanopy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3pirsdkev.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hpyqoprp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rjnatvcm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rzzjwihx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qjvmspof.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3bzntzwyb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwvzfzra.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wherjfav.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wvpvctqf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uefmywcr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3utnkmufu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3yokkucjm.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3momvgeta.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bwusqwva.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3utqkfqpa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tgnnvxgp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3zfsvtvle.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qohnruaa.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3roiskami.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3gqgrcrap.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3lhkdveag.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3lgmiwxwf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ejlpbnji.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ooqolbpe.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zhhmgfca.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3uyufglub.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3gebumkjg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3stlpwecg.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lkzznwhv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3rdjfezsm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3yvinihmg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ngguumey.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aokzuzae.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qzqqfkyy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3babavibl.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kpebvenx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3zlcdoyzi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjwllshn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3dypewple.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3aysluuly.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bpfhzddx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gtmxqlnu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nkmcnmoo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3berbinev.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ecfccyio.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xccldrgl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kwcrrsxk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3shoflrda.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3reukbyix.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kvtvdrpw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kuiyvffe.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3baazzpyl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dfvfcoip.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3uvphrmit.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3orunrfkk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xwqgwsiv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3gueeenss.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3sebeyumd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3jxxuerct.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3slrzmjww.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3kwjtmpij.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3bqkzactr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3brzihtmm.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3wwylpszt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3lkhikxbc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3gfkcdatt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpvxyrdu.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3kruaxcuj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfcpmbay.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3upluxpaq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xbhcerbu.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsajyfkh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmpmajaw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3lnxfyyzd.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bgwvleex.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3coibismy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3wrchgwcv.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3daquneep.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3hbarmkya.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3jtcwbvse.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3irkhgwil.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gcocmosa.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3oqycroxb.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kczzgnqu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3rwujkaix.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3flvqdigu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bcoicvhx.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3sxusdzuf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hwmdsihv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3feqhfnlr.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fzfpiitj.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ufrjciae.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3dabwftth.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3rbqmagkq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3wnfssrna.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3nrhbtecg.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3sifycoda.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ovxuxbqq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pwjpvprh.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdhdnswd.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3thoftgtf.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dcaiojmn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ybxcznyu.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3ebkknqwe.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3klvunevj.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3kgnyiduv.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3wumzigon.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3svbwshjv.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rictzlvl.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ukawotfv.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sscylcuq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3vxlgukuv.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3vhnzbaeh.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3amqpklws.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3aqmwbzls.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3zenlvwlm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yvagqddk.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3zjidoiwq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ucmsusst.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nchlurdm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3qquxalsr.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ypeefmgk.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3rbkdwpbz.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3lfvgyznv.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3rpcjpfyp.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3uiqkmrug.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3uhnfbcva.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xbzgavyq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3gnuhoehi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3zbxvxnyf.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3vmewxzdj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3llujpdel.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3ewfdqaji.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3kzhvzncg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzdweqkj.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3sefzzqma.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3bqimzkox.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uastfpfc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3gevyifud.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3imuroryt.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3greeqhlh.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3jrjvudgx.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3akivzurc.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3syavmifv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wxtfosbi.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3kihygiih.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3trjgfqvg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3qbiwkjrv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3kxuqdwar.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3rvpocryx.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3vtdlefox.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3sebosbpy.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3auwnipfe.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3vrrvnxrb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3lpntksob.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3chzhmbwv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3nyqchare.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qyrjiwuf.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3tzbpddtz.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3nsjximtw.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3bzdatdok.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zmntymtp.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3icpiamdx.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3itymycwg.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dsjelweb.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fjmqaklo.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3ftjvrrsj.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3unqfpdyw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3uancgnbe.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3wdhtljoj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3lfrrtmxr.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bofarxbk.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kctrdslw.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3skgxylpr.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3kewzbkeu.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3zmphecvo.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3rsfqbwhw.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3fneuzgfl.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3sqcjyoif.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gjxwelcz.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xnmvuwla.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qpwpnriu.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3xauxnvaz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3lxuvaflf.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3fmygpnue.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3ienssbnk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3tbgybnfg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3flttmngh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3qhzqczsx.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3emvbhsmd.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3vabgurgv.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3hidowyxv.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3txvgiavv.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3pafldmtg.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3mombeumx.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3celsviss.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3olmoyoqq.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3udmildht.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ucmasntv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3zbgpgjuj.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3zwtyfxsi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3hhvshfld.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3zrsipbtz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fefarkip.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3izbmqqjd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3bekxhxyp.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3caqftqgz.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sfeykpnr.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3ixotvxdl.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3dpocpwtt.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3qemwwigz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3dlstynpe.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3iodztzxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zxieafut.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wwfafhnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3slhrtlny.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3mgdwmdhj.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3warrmwcx.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3stsgmook.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3pzrzyzma.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3umvhbclj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3umoawfet.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3ijhlrwfa.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3oacvanem.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3wuymsvvi.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3odbshyzv.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3bhttnpsj.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zcuymzyi.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fxtkxtgy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jazcafom.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kxrkumsx.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ebqdlijd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3pzwuonmz.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbfjbtsw.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3crpphwvc.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3fwosraxp.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jizjrcma.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3cecmzimv.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3nwelysvu.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3vjbojfpe.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3auivuapy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3uyyfblvj.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oicctxqi.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3cpbaodtq.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3twsgtbou.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3fdvtvtkt.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3egpuvtzs.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhxjjuxp.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wclfqvgy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3dlfyccrx.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3rzjlqcnx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3fnezsvwm.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3nhhchidl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3zjvywhea.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3eiwpamyi.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3novrlkol.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3kxxpfbxu.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ufhrrcqk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3gprtcmts.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3mztekrgt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyripntj.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3vshcteny.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3ccerzvbc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3baezhksh.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lunvgsbb.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3ljnnisbc.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3qaazxqfm.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3kvizdaqv.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3buobjsjx.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3girxrqsc.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3dfuycsuy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3vzjnspyg.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3jxqydfbm.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3ebxgndsz.html


<!-- 参考信息 -->