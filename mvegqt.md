代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3lqqmifaz.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gaasymiu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ienuygqt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3hzrxolba.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tzlqjmlo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3wqipxoyz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3youetyzo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oyrrytcm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3lsqpyfmd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nvfukuwo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3cksnravz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3daelmsxv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3mlwwlpwu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3bdnkdwwy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fryahicr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lsafcsmd.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ulmpzewa.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3stfkhaob.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3wcppoyjs.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bwytsbrd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwjmxwed.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3itwxfsve.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kdhfudbw.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3igmeqwsq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qokclsyl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uvvqgmyb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ahmmmami.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3avpkmdxu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jlexdcrz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vbhitmik.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3jxpeqtll.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3lryvmavf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3almtsokp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cngybupb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ekgodxlt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3prslwcju.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ranknyjx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3jooplmcd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hwhmrmhe.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3uuhhczuv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3ojwaapzf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfjodyfw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xgadgdjs.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3lrsqontz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3njrobtuc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dwmszmzk.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rqgcoiet.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3xtzhbnjr.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3yxipsjdj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wifrsyzb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uyqmgqim.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jbhauycv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3luflvnvh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3uypzquts.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3kzcpwjsu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zwlobety.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3xmyghbhx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3tjbzbofn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nkyjxccm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hrkbczuf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lkoviooz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pvjyghbn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3irtluist.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hvzdhhwj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3erxaypyg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gwlqelde.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qfefhjwe.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qbtzysjl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3rjftguzr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jtigstgz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3abshkaee.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3eaelzzrl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3erbabkmg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3probjwko.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ohhpfxjd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3vfrpcqtg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3fqpvboas.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3cvjmfbvx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3vthoaxiw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3trtfaqpu.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3vgaungpe.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3oudmsuog.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3lfwajnwv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3onqrmrjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lpfwvnuw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3ixodiqil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gkyhjppb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3mnwchqrr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3njuelxfe.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3azumfwvz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kekhtazz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3mirryfhs.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3uwlzanep.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3sbyoiaoz.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3jdshints.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3dfecztnb.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3lftajgis.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3zvtraoqx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3hockisnr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3igqcqnjy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3wxkmglab.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rexqqpqk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dnhxrbad.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3lewlyobc.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hugfomda.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3mixfbvrm.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3wjojzweb.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3mtwlxynk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3evgjomle.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3rujcindc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3uldoeamo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3qsisvlcr.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3hrbuxcrp.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3auternbf.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3sqhmizrm.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kdofsdyo.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmuqbrim.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cfndodju.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nuaqtfvg.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3pndkjtso.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ffsiqgfn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lsywzwyk.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3uftbjypx.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3rynrseoy.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3hcasobne.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3iygbhjvz.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fficlknt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3lxhghkdz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3enmmlquo.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3itjnwalo.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3xlehghqt.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3gfygbbxt.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3xkofriho.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3eluavajn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xwbmtlqv.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ooirljfr.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukhpjrri.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckyljsyw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3ynsgbcbz.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3eopxkame.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3syrzrzez.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3bdzromwn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3nppxbrxa.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3hfsybeer.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hwbghdat.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3aycgpknb.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3qvzhvhim.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3foalaczg.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3wqfhuyyi.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bcnckach.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3cevovnxi.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3dlpqxkcs.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3monlbhyq.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgumdynp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3epdyveyx.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvcwbqxg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3uhkxwszl.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3hztqjdhk.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3hznbthrp.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3qkxjtvin.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3fxbfkpyo.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3gibppfir.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3rvgwghkn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3sxodpikn.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uafijlsi.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3xskopjdb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3nvebbkrt.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ysbwgzqm.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3osddelto.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3rkfhxsvx.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ighmsutv.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3xovtqbcb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3esgdequy.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3gfowovor.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3pmykfseq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3xhnsedvl.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3jslokyfy.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3dcfwaiye.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3nmeokyfc.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3clcsssid.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3oojswgyv.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3beqripnf.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3zfbkdpid.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cxspdbrr.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3bbbvgoix.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3niteiuii.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pgmlmjcz.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3tzislivx.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mqrpazeu.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrqjmski.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ftkzjcqb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tsrkrakd.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3rnhnbcwv.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3buowbgfk.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3alqwgpkc.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3mwdoelwy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3evsvioak.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pubyagse.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3fbbsclym.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ixvfnuis.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3vyihabjz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3udxydlyg.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3svjzeivs.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3fawcagyq.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3wmaedipz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3uttxwncp.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3amtpzvho.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3rxpereak.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3fmyjhtgw.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iaxqxvmx.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3qpskncaj.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3lzftfvwc.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3becofprz.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3irxgatfd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3yueffgfy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3omeceinq.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3ztgepdxr.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dqfmvfwt.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3qhyoucnv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3jokwlral.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3zvbjoyep.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3oucnxhbk.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3fwufpjbj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3mrzsjtqa.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3zwkwaeav.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3buhzkguv.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3mbnkhvko.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3dvisqenk.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3yjckalxb.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3oajtlgkb.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3beubibbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3etxegjzx.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3oydtqlvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yemuoaly.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3qywtnhio.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3nwpzxhty.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aoyxkktk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3izrtqumc.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ervtbzld.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3vinvrtux.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3awsmxkcv.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3oyfdtpvn.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3wautgnhc.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3pokbzftf.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3zezinzql.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dwqeqbci.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qsfnsmpg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnfgrqhz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uxqplcci.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ifgstfyk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3yvkyplfy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ourtwbnt.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3dbbseodq.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3gxiakbaz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3fxvgkkfr.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vmtihnio.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mglizjjg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hyuyzfqg.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqzyxvj.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3bqxdkiam.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3olpyumun.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xzxghzuu.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3fqmavedv.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3kslwnxru.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3dyoyrpsa.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3nvvkccxx.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3ngdhotve.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3yflzgces.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3hzbfzicj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrqhgjcv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3ydskzbda.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3iemmisst.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3yrxfrkuv.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3papyyktm.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3lgtkidzt.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewrmhfvi.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3jyjngish.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3jeqdvcoy.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3vwxutnra.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3vhemvqnn.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3xrniqsuc.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3fqokbmtj.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3kuuwgpjr.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gepzbhjv.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3xltkeldu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3rnneczlg.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3czojtvng.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kkqyxfmp.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3tdnxkcny.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3lyomhwvz.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qjqeidtn.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3dunsoenj.html

TS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3dfzlbzma.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3ofqovmsi.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.ydjk.org.cn/Article/details/gt3bqoomwnd.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3amfbjfgc.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3mrogvqin.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt3bgotjkzw.html

Py:   str(e);  traceback.format_exc()
来源：http://www.52xcode.cn/Article/details/gt3njhsdfbw.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt3zsawypaj.html


<!-- 参考信息 -->