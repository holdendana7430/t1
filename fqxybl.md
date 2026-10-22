代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2thzacenj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2gzcwbtye.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cfxitoej.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kupypzto.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2aeurcogp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gkheqnoc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ipzsefos.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mtnukjpd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ydkndqyd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2upvgszkw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pudsstbt.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xpxhospa.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xjgqpfng.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jgzkuyot.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2bfvtiixj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mjaoeuoc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2abwawtpr.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2gogzikbx.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dhaxwzxk.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qkecfmak.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wtfmnlmr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xelorqlq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hkcyfcgq.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wupeizvp.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kdmzzsff.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gufcetll.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2vkxaozye.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2slvclayi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2pcdxemdk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2jlllaukd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2rkufyold.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2uretiynf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2cnbqldat.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2gkfpoupc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2fbqkuore.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2pwhepaqo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2rhihghkk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2chugjilv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2swfhjrbp.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qkthspcw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2awgipvyy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jgyitzxw.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iojvhmmq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2kyimrdur.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2rjjgucvi.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pzvuywso.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mgmdufqk.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pknheypy.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dbcjzcsr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dmtvgwuu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ojeiadhe.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cqnoffft.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2cegjfdim.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2vqvmoooz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zfdetsuc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rsbscliw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ycdzswmu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2txfnrgvi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ybgecjkk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2itpdlfad.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgjziyrz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gwcwhbui.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2yqweplno.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ydrjijag.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2qxalohni.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hinhzzgm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2waluwnuf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tbaoyxaz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2bsvqkboz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ueoxvbov.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2mqiaiicr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2uqgsgjxv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ggzldcll.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dvpcigsi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2jlzhrgtm.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2phsndknb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2gjblmedj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2gqigpavw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2acvlpqwx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2tnxjxlqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jecnmcci.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2lbqgqlxj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ajsuvmwg.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ywivserg.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2bunowxiz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ajegbshs.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ljiooocu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvkcuicd.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2lstmnmxv.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2oobxgxqn.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2efvvmgyy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2kzivwcdl.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2itbtteco.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2mtxwpqvc.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2dxbsxhlo.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wkfapnzn.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2gofmfgxv.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2khjsekrx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2efodsizu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2vgpejgfm.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dlpapobm.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ahuxvsci.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2cyvqviok.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2qlwwsjho.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ygqajirp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mejilrbj.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2icnhuian.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2sqdeuayp.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2tdqtiujb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2glosvqat.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2dkpdxfkp.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2ctralqis.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2wowtpgqi.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2flitjhnt.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2znlrueee.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lyzwrfee.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2ubgoiiab.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt2oqvbyibd.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2izvxzhfu.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt2uybcnaca.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2cpkinmhw.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nvphnmzs.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2arqaacaz.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yaaniwgz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2zegybgfl.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt2aozmmmnu.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2vfojibng.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2boqgmwus.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt2xfqopdgj.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2idbscptc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2sztzbaby.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fsuthyec.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2rqjkpecd.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2fghyqybk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2gmjjrisz.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2krqxijxz.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2xtsonswg.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2ruxgklsq.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2frhlglvd.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2vltxwlxw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2crkahkil.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2hvxzxsoo.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2ewfbbhlf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2makthvnu.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt2glhxqaux.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2ibofmtgi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt2prszzsxm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2jivmfvhb.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2kkzfrvzc.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2czujhgjd.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2dmmesiqd.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwmykaom.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2xseaufrv.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2jxzetsae.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2kxarnepf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2gptxbxjh.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt2auoqychq.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2skrgjxkm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt2tlfoksyt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2eubgpuzl.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2jfklyokk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2dqzrmmje.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2kzrnoonm.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2svydomor.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt2wfybaafl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2tqnyowcx.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2zmbrhjgx.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt2zabvodji.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2owqwmnha.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2oitvalnq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2ssayfyfq.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2ekdygode.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2wbnyhruu.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2okznxccf.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt2fjcwjmvj.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilxnrjtm.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2hqbpodtp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2dmpfvhyy.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2nlcjzidv.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2wokeotks.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2gcoukppq.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2faomzbfq.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2cioexmmq.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2cqjlrzzl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmkeikbt.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcyhcyxd.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulrtcitk.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lxxpgrjm.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ftpeigpy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2dutlfyos.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2cxtxvlmg.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2mjvktseq.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2ordcgvei.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2zvwqfuhy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2dqthrpnx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2askjmkhz.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2nnztaigy.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2xhiyvydw.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt2iqgixtrp.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2pmrqazun.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2rdvzarsp.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2plaghhcd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2kuodnnsk.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2dgmkagta.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pvaqiaiq.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2vhnkaeet.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2mnaagecn.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2hekhiygw.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2qgkrcegm.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2tdsxgoub.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lrrtmfzh.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2eyyuzxjc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2tfcrvjeu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2dosfxwly.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2ztgtceur.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt2iwcraiih.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2enoniamz.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2inbzznxz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2lovcacpi.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2fcavxjgn.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2sedguxab.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2grqhomdt.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2jdfmgobk.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2emrsbfws.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2mujqktjy.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2noeeblxg.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2ewsibsub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2worbnyww.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2ckaktueb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxvkvhfg.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2tbxynbmc.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2vsuyuvvb.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2juyamhsi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2ekmfexop.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2lesylyup.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgkqyurh.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt2qgqkxtrg.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt2izingjhz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2ylmmoovd.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2eezbiwud.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ioedijet.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnjswijg.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpjgywqt.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ipytuhcz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uorlupxd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt2erbxwtbg.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2pwblpnok.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2jwskvnhu.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2sixjvjaw.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2exssemir.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ffuaktob.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2pfrsdred.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2zzlrhiwo.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2qduloknr.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2xwrneqkz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2tpaskqih.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2gnzyalfo.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2qatsgeka.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2glwupprt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2aejxojlf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2kdumnrou.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2jsipurbf.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2epdgflkv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2qkzxzxyo.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2fcwwhhwy.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2zlbmsenu.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2levjylpe.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2nmsmbkwf.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt2jponrrdu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jsisxebe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2iwbaoamg.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqjwvgwq.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2zjwpujna.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2xqmlngyt.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2fgqluqcu.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt2ywrwdagw.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2ofamkkxx.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gbiuyupb.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2rjnandiu.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2ejfopwma.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2wndpvwnu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2ddjramwq.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2kgzdvjbs.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2qolszzsi.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt2fsontgft.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2scjhhjok.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2fdqokesb.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zaiuqybi.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt2jbbeuvss.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt2nvaeobdx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt2fjjbtgov.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt2iznprrly.html

C#:   Debug.Assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2hswrftxg.html

[H08] 获取错误信息与堆栈
来源：http://www.ydjk.org.cn/Article/details/gt2isjddzlh.html

Py:   str(e);  traceback.format_exc()
来源：http://www.ydjk.org.cn/Article/details/gt2kwjvbynp.html

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.ydjk.org.cn/Article/details/gt2ghdkrqhb.html

JS:   e.message;  e.stack
来源：http://www.ydjk.org.cn/Article/details/gt2ernniegh.html

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.52xcode.cn/Article/details/gt2lfrenecr.html

Java: e.getMessage();  e.printStackTrace()
来源：http://www.52xcode.cn/Article/details/gt2xeabjqkc.html

Go:   err.Error()
来源：http://www.ydjk.org.cn/Article/details/gt2lwpbzkra.html


<!-- 参考信息 -->