代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3upctgzeh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3iwqgbntn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3havrnibd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3nwocrbau.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nwevpewj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3pnkzanko.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fwmbbgba.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ljyzhiln.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ihrupntv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3voteuvep.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ktgtwzej.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vwvrymdi.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3zhwpdrkv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3sweozepu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mjlwatzi.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3echwkaho.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pmdlytco.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rugstahp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3bcvfatko.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svdtcpyw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3evjnoqbg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3vedxlerx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lzkpjxdn.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qixogqfu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvhnsreq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ykoiiabn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hgvemkqi.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yrjybccs.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xkjdmwlo.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3noioxcsg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3syjfrjvk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pxtbnstw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hxfvlxay.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rceehgti.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3raqoynut.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3kzmzvhql.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3mraspokl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3iteoyxed.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3uexiyrof.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ibpcgqqz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3zrlnktjp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3vflnuwtf.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qzkkwyxr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3uhyvhlfe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mogjpifn.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jiafygyt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3mdjrxggq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3oiqhbxvv.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ucvmwmpo.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3togyjpfo.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3guqhveqn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3nutupjnx.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3emjjqwtw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jbxwfbty.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3henyqvmk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ilfiwvdp.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3pjhivgvs.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ianouhmz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cramfivo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3eqxogbed.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3apridzag.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rxpzekhp.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3zauaydcf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qkucdtme.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cfcpxiie.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nfdnebmm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3mlviwxxw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3cvxhqvrq.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3bgdtqdqc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ljxnmxne.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3vnqpmjzz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fqvwinlw.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3clioggrc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wxjzvymv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3zfemavjx.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3osorpgfu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3icjcroiv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3grzchdwp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3mkphrmhf.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3awllrvwz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3gyvejpdk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3whdkbobd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3rcivpqoh.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3teqxzfcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzmhueck.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3lyrsviwv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3keihzzod.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3uqfdgkjv.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3raxxuasb.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlylfbzo.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxryhroy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3rgsqnddf.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zgwtmdlh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3eeexsaaj.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3irimdqwr.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tpxmyosj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3kjjkmiyw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3zuyrieqm.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ixknsnwe.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3idulutet.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmameyrz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3dgchdmmb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3vzbjxmyj.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3emtstxjr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bhsanxgi.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3okzmporo.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rbwpbqdx.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3umzxszaz.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bmbpjzon.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3rujdhscx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ifsbfpru.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ajyhvlaa.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3eztwmvjn.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ovrrjuwq.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3pdheajvo.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ndgxjrek.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3mdtgrghk.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3crhvzeeu.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3iofklvcn.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfgezgtd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3llfxuwxq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dhlngiwq.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nsqvejsr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3pceyqkgy.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jkwnhujj.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cxaryzas.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tjeptomh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqdjnaam.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gccpgwgu.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3klzyualt.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3rvjbjwre.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3grycnplk.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3jvvwwpgp.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3ofimltvf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zudklwzw.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lbtabxww.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3unxdgiaz.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oipzfmng.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3otyijrno.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3dkcvzcvj.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3syjgviqh.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3aahshfdr.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3mfnhkrea.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3vfmpkgpp.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3sycdciur.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bkwbvrex.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xblncfsl.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3durypiny.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3uyhueiog.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3vatmfvkw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3jrwkhvmt.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3bmlwkusq.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhgugqpw.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdfikdnr.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3hekdosjk.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3bldrtusq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3gdfagwux.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3gskcdfoy.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ajowlpjn.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3podlzkka.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3ephuymuy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3qzbpyvhv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3wjitvpiv.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3qszdkfxs.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3ntedrgpg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3tobiclzd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3vkntsrxa.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3mshzjptm.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3hfvqaqxq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3lxthlrzt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3xfpodjnu.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3nejpkshx.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3lrulplrs.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3aeyjeyjt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3pwaalwrc.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3kmpqvamb.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3epnujjhw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3kqicheqv.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3jheprdoj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpagmtog.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3fwlfokhv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hwdssvye.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzprevjt.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3flekcjje.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3iahyancn.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqgpopfi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bbbpdeal.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3elxdafyr.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzzmqwpo.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqgxfxvc.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3manrtbxo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkawrilg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3scmdbeai.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3kwoeaozw.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ztawbiux.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3zdyrtlmk.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3cdltfnrg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3liqksvsc.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vicmvqfr.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3smitvost.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fxsdwzpc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hstgbwyn.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3ojoiacsp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xcaabynm.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3hadtkgax.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3chkhrnij.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ffprqnuf.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3kzsymngf.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3ylqfkphy.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3stgqkfrp.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3uylnbcqy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3fqosipjh.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3vykwmmhp.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3cbxwwchb.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jwxiyqtm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbtszfew.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3rvupcrgy.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3fkjwgetr.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3hsehbqvb.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3rnvmhugo.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3dyojvplv.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ajbcsqdu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3ydteykxe.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3arltmcdn.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3vcokmfwn.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3midpkkhi.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xrzbxiiq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3foqnjufl.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3hlcfjbyb.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3jljwsvot.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ieqfofke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pmcanzzk.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3lkbccmdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3shkrjbzh.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3bscdjyrv.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3pilvcxce.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3catagmig.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qfyunmwo.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3hmithkqz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ksudllez.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3pitlyvhq.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3qrunvqhl.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxykdvis.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3ecqvxxqe.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3intcratc.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wkittmcd.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3clayxntb.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3exhhkiin.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzhytvxu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3uelyczjj.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3qotbcqac.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ypjaxomt.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3ivhvliqk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3jgavblko.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yfutlgwi.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bdgmarvm.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3hvacdhis.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qovspwwq.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3fcsqoymu.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3tdhmaxyy.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3iuarkpmt.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3rbsyhwco.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3rqwmgnoh.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hhuzomvt.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3utzhcelq.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3hssicltd.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3amoxvvya.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3cfeelspq.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3vuxylawu.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3jpvzspqo.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3zrclxupt.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3wsckjqba.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3vyrfdxzs.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3xoaqjbny.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vigkdzjc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3mwzavcfy.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3uzbswkvb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3vrpxrjnr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pzbnefpn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3alkdhnhf.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3bhjokdym.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3bxepvqqj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gddejzij.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3nteldfax.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3aihxewbz.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3erbzgxuz.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3yqmqwydg.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3xkmtqbkl.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3mrclpkgo.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3kmowrllv.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3rsrvjoaa.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nmtvinrw.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ifchvefe.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3emhrnfot.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3ykamozwc.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3hjnwqtrf.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3nfnmmtte.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3kmmjjyvl.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt3xxxmxzgc.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3jqcvekjb.html


<!-- 参考信息 -->