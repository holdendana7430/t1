代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gtqlwgsgb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gntdcegoo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.zdbjq.cn/Article/details/gnnvfenme.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.zdbjq.cn/Article/details/gjjgfqaip.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gjsxuunzi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/grbofjtxb.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.hesvh.cn/Article/details/gnverqwul.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdfpebpqd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gvhaxdjlt.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.zdbjq.cn/Article/details/glwpjbkfe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gvehsghlc.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gshowghiv.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gdizkowlu.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gdqhsuxtk.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gzmrorpmm.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gimjarpyn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqleggoxv.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/ggfzjfrsk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gjijwyusm.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gexdcbiiv.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/guvmipydu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gtjibhdzs.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gmulepjhm.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gxrzgpbdv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gsqrjbyhw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gkxulgsmu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gtdqvfswh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gdfnixdyh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/ggcmuzcpk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.hesvh.cn/Article/details/goeoqlvvy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/ghhbfccdt.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gxvfpqazq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gyeqhqnyy.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gxprqkqhz.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gahecjgle.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gpjdaugex.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gpztegqyv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.hesvh.cn/Article/details/gypueynub.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gokwxbbjk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gnqebfdty.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/grntqwutt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gzcaucjva.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gtzxlbfod.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gwfwxsjst.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gmhmajbqq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/ggxmspjlj.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gxzziloat.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwkuvnxrn.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gpnvnevxn.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gphaxchqu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gseywlkfk.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gdjjxuwpm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/guiecptjg.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glgowaxzw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.hesvh.cn/Article/details/glfnaiwmm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqqbasfgn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gozhbyqvp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/ghlgqykjb.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gwycpbspj.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/goggfpaxq.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gnvesmruf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gjxkwkhjq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzxackuek.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gmnigoioe.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.zdbjq.cn/Article/details/grbjgzeqe.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gluehcbod.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gehvfayvg.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/gjkokcatg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gvnweljgk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gfchryaue.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/goysprlsw.sHtML

TS:   // 同上
来源：http://blog.hesvh.cn/Article/details/gjhsvqoqf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/ggquvplky.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.hesvh.cn/Article/details/gsgivlnyk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/gcvthnnxz.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.hesvh.cn/Article/details/gucdmtamp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gcxbaodhe.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/gvvbgoywc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/govifpqqs.sHtML

[G01] 定义类
来源：http://wap.hesvh.cn/Article/details/guugjcixw.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gtjhtkgis.sHtML

PHP:  class User {}
来源：http://m.share.zdbjq.cn/Article/details/geuyvwqud.sHtML

JS:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gsozqoxff.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.hesvh.cn/Article/details/gcaupafqn.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gefngugtp.sHtML

Go:   type User struct { Name string }
来源：http://blog.hesvh.cn/Article/details/gkzoydiqb.sHtML

Ruby: class User; end
来源：http://www.m.share.hesvh.cn/Article/details/gyazdcegw.sHtML

C#:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/gzxjaoezf.sHtML

[G02] 构造函数
来源：http://www.blog.fehbvm.com/Article/details/gtdemtega.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.fehbvm.com/Article/details/gzeqytfau.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gmdvvaujx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gqfamughs.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gdoubrfzj.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gfyojutaw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gxsxbswwu.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gsokmhftf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghdswadml.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/gzxooiyqu.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gdcthdgfq.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/grkravpef.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/ghlurjgkk.sHtML

TS:   name: string = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gdudhttth.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gwadzfyyu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/giqbovuvr.sHtML

Ruby: @name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gmfdgsude.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gysnhsfnn.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gatlfzimq.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gpvqafrpw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/geyephgsi.sHtML

JS:   greet() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/ghephzrnh.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gtugcbeiy.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gppklqzcu.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/goqgnfsip.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gsepxzztk.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gkuyzwraw.sHtML

[G05] 继承
来源：http://read.share.zdbjq.cn/Article/details/gnebsuknf.sHtML

Py:   class Admin(User): pass
来源：http://blog.hesvh.cn/Article/details/gbagjmguy.sHtML

PHP:  class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gaaiiugtz.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/ggoynnldx.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gjcarwzej.sHtML

Java: class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/giliueulz.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/gawfxfuto.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.fehbvm.com/Article/details/gxeynpzfs.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gftegybtv.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gazhtjdwa.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.fehbvm.com/Article/details/gidqbrbiz.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/gyhckoble.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.zdbjq.cn/Article/details/goeqbwphf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gzblxgwrp.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/gaownyvap.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/gckbizfrl.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/ghelbqpah.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gcnnabbqn.sHtML

[G07] 调用父类方法
来源：http://m.share.zdbjq.cn/Article/details/gzxyhicyk.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/glcxzvfda.sHtML

PHP:  parent::greet();
来源：http://www.share.zdbjq.cn/Article/details/gffoyhbbj.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/giatxmday.sHtML

TS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gqadudbge.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/givsddofg.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gnntrraio.sHtML

Ruby: super
来源：http://m.share.zdbjq.cn/Article/details/gnrzxoeuf.sHtML

C#:   base.Greet();
来源：http://mobile.fehbvm.com/Article/details/gnlpsevmg.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gxblicknz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gngopvkto.sHtML

PHP:  public static function f() {}
来源：http://baike.fehbvm.com/Article/details/gslyddjff.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gficwqbgx.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/grxcbbksb.sHtML

Java: static void f() {}
来源：http://3g.zdbjq.cn/Article/details/gglyntzeb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.share.hesvh.cn/Article/details/gncujnrgh.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gseeshkmm.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gzxwmqgzq.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gosfufxhg.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.zdbjq.cn/Article/details/germwiiue.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.zdbjq.cn/Article/details/gkcpbcbfh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gasmyqhob.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/ghxwijede.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/gifqkdvxk.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.m.share.fehbvm.com/Article/details/guowkoouj.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.zdbjq.cn/Article/details/gywmqxjed.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.fehbvm.com/Article/details/guexvfdmq.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gsphnbtwc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://m.share.hesvh.cn/Article/details/gwzgewvhv.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gvnduxmtd.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/givffxnnj.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/godnzkhyd.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/grzemxgkl.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gchsfkngy.sHtML

Ruby: public / protected / private
来源：http://mobile.fehbvm.com/Article/details/gxkzvrhkd.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gqjireiob.sHtML

[G11] getter / setter
来源：http://www.share.hesvh.cn/Article/details/gblfznnlk.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.fehbvm.com/Article/details/glwbkpvwe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gyoiicsuj.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gvjzzcwef.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.fehbvm.com/Article/details/grpzrqfgl.sHtML

Java: public String getName() { return name; }
来源：http://blog.fehbvm.com/Article/details/glrbcwyct.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/glcvnogxl.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gajdhqdfz.sHtML

C#:   public string Name { get; set; }
来源：http://baike.hesvh.cn/Article/details/gkcygyzvp.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gqooeejtu.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gydzlegck.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gtbdnkfqv.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/ghosjpvrg.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/gysfqiwiw.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/geocpfozi.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gttxzevoa.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gmyqbhvpb.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.fehbvm.com/Article/details/gfhbcfhyg.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gargvcdxq.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/gmqiaudms.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gjpnngnsc.sHtML

JS:   u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gxrvblvzw.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gnwljesff.sHtML

Java: u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gnelbspnv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/giefgmoru.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gcetmxpjl.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gghzlubrb.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gxrbmnaht.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gprkfosox.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.fehbvm.com/Article/details/gevtyerlq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.m.share.zdbjq.cn/Article/details/gqedqmmgc.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gzmdstoxk.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gqnpbrkle.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.zdbjq.cn/Article/details/gghmwkdcd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.share.hesvh.cn/Article/details/gmvzcnqtx.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/gchpyimyt.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/grptdacdn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gcafarnzj.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gbvbbiwkk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gmaauuxap.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gjpdnydee.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gvevjhalq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.hesvh.cn/Article/details/gsefaxtpd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gbggllybh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gnelphhix.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gxlvaqnzy.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gpouawtqs.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gkmuulbsk.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gybiilqiq.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gekevkvmr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.hesvh.cn/Article/details/gztrhfeic.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gvzznemtn.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gmjtwjsfj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gtghygege.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/glyysewar.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gbsvpiatl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/guabwurgy.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gknycafiw.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/guutajtop.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gaefcstno.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gxouqkgeu.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/ggcepsxwh.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gnpchmfki.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.zdbjq.cn/Article/details/gpwrfofvy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gvhsmceyy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/gbcachecb.sHtML

[H02] finally / ensure 收尾
来源：http://3g.zdbjq.cn/Article/details/gwsyaqwph.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gjmrxwfkd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/ghzydpymt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/grzmhffjj.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gplqluxna.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/ghciuljqu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gvcvpkbcn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.zdbjq.cn/Article/details/gxqxtvvek.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gkidaccrf.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gpchjtnty.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gjbyewsgy.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gjfrlqjzk.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gyvvnxvzl.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gokolrpyh.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gsqjhgdxo.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/grfhzpqmt.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gglkpzfqo.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gmdaerrxy.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gfjalfdmy.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gwghraaru.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gchuzducb.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gyyotfvpx.sHtML

TS:   class MyError extends Error {}
来源：http://baike.zdbjq.cn/Article/details/gxpcpexxb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/ggocnnybj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gohxeuzxf.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gkdbctrbv.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/ginxmnvrz.sHtML

[H05] 捕获特定类型
来源：http://www.blog.zdbjq.cn/Article/details/gmkhqhdml.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gbovlmyfi.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.hesvh.cn/Article/details/glrmzkjfx.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.zdbjq.cn/Article/details/gpysqpcbd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/glrdepdcw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.zdbjq.cn/Article/details/gppgzzwqt.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.fehbvm.com/Article/details/gvbgfsrbq.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gqltrogwb.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/ghrlfdewh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gmbdbfvgh.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.fehbvm.com/Article/details/ghonsbuoq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gbiyzvlxi.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gpcsmgolv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.hesvh.cn/Article/details/gwrhgvnsn.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/goopanxui.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.hesvh.cn/Article/details/gzrpewbmd.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.fehbvm.com/Article/details/gavgotvyn.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.hesvh.cn/Article/details/gfbdazxmc.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/gnifmmowr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://3g.hesvh.cn/Article/details/gkehtjubd.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gcqwomlsb.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gfxqdoexe.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gfpzlhcrw.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/gxviqtuwp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.m.share.zdbjq.cn/Article/details/gmcpbwocr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.zdbjq.cn/Article/details/ghcfqvntn.sHtML

C#:   Debug.Assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gzzqkanuu.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.blog.hesvh.cn/Article/details/gwjrlnowl.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gqbtvsiyp.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gisyforxl.sHtML

JS:   e.message;  e.stack
来源：http://www.share.hesvh.cn/Article/details/greulitug.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.fehbvm.com/Article/details/gtbmhldov.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://wap.hesvh.cn/Article/details/gaimfaqbd.sHtML

Go:   err.Error()
来源：http://blog.fehbvm.com/Article/details/gsijxzzdm.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gkpdzjjof.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.share.zdbjq.cn/Article/details/gfrkxpzdt.sHtML

[H09] 带错误码的异常
来源：http://mobile.fehbvm.com/Article/details/gzapsywaz.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://m.share.zdbjq.cn/Article/details/gkqlicesy.sHtML


<!-- 参考信息 -->