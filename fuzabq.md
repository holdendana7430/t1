代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2bkbiidch.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2uvtoexfe.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2muhaycdd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2lmatejuc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nurqimzy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2txoddbtk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ykpudags.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2mhpnepzu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2owgcthie.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2oxukznxl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2fkaiatzo.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2rekuwimo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2getluicj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2xwppowpm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xtfngnzv.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qikrbvtf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2tvrexsmi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cctqqwzn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2mclfnazi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ftsgjexr.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2rhrqdbbu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2tdixxfko.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2plfbeocc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eosddztj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yesvpxmm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kcmbwbsd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2zhxzkrcd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fwzccnhr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2igoqkogn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2tohltmrk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnjglcci.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2roaznzip.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pnnzlnzj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oidmdkrn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zjopvmhe.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zsaqyblr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yqhngyre.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rckufwxp.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2qkoqpoqs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2rnjozaiu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qgiezyeh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2etlgrbvm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zchpceui.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2xeqqatvu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2yemhckxr.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ijcyllbt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2rrnernzg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2xmeyrkxa.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2vwcyijkz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2gurwhxkm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sqszrpzf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2mdadfbxe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2kapdnujc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lbxperun.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2cmffwaca.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2myqtyqkg.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2gniucpal.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2weravltb.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lasofesc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2mbczgkoq.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uxelblrn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2udnhicqa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2ymkqzrua.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fdpikrvx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2pabnqdtj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2iynlmsrk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2avqffnbv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zmnywkpp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qmjbhcje.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ofefowjb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2mtsmztmu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gmwlekti.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pbmsdeia.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rgwpqiku.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2nzjpwkkj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nsrmgoyl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2boqgapze.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2blfruitr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjmusnia.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2payhbqno.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qxmgjhwk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hlfvgkrq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qqutrirp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2pzaoaygk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rfxatdlf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2plahbpwl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2auqzkwux.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2trezyjmk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ipunxacc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2wmcgxyen.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2oiyhscir.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2qjitdcxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nayordgi.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2dyvkvgvb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzgkkjop.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2giogwifp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2kicmevwr.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mwwenkmh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2oyexqegj.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2cuadcgqm.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2xgpczflj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2wlujbvti.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2yphdximf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2xjmpmfic.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ghookqqn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2mktalgvo.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2pznyvzqz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dfkikuad.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kgewugsj.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2ashbifue.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2uydlmzkf.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2trcvxhkv.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mymdrrys.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2ugiqkcik.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ppwvgiji.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2omtykwnb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ccxxmryc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2pfmcqjtx.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2mjatsfgs.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2sjswlvgf.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2leyvmpwg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kdxbkvqc.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2qiyzgreq.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2mhwqqvzf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kulfpyyu.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2savblybo.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2unvpggaj.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xvwyxeiz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2ysdlovxq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rmadyjwn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2eklcqgei.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2zfftkezm.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2bopjsvcx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2biaaoxmt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yienaiho.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2encyhaag.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2jzgjqieb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2sbqxfrai.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2lsrukzdu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2vclbyfcs.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2sffgqcci.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2bfhljubw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kvlfnlar.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2vdsigrxq.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2lromxzeb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ezdebggg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2hqrjedzw.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2rrjjsvrw.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2plxwapee.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2wxhnsrid.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2lwzvhydt.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ggelyqsn.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2zdfxuhje.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2diihqufp.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt2ghwjytje.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2fstrqvgs.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2jjazhxro.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2qtwqgczd.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2pzidqjyr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt2mfccifqa.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt2fcgqydjy.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2petkptjb.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2mrrxgtux.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2lnxprwxk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2qsudajqh.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt2norzqwsl.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2yggapxtf.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2hokatcvf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2nwlxjrxi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbanyjub.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2nstuvqjl.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2chqoufur.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2isgdayoo.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2xiybtefv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2jatrybuv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2alkekhpf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2butodxcu.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2jnhczjjg.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2lftqmiac.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2qquglvjh.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lodiosns.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt2wqjyokpq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt2bzmdtjbc.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2qbyxkyqx.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2dxcmfamk.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2ceqtivqc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2tznksyme.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xwvqelfi.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofnzfern.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2sllflrbn.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkrjkghh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2kehdbpmg.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt2wiwnlzgi.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpffpbrv.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt2opkdhjhq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2csqsylxt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vncxvtuq.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2almhltvs.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2gencgzxh.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2suixvrow.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2xbjoibjs.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2opbfhhtc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2vwfhdyvx.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt2pljawhqs.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2dknmendg.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2fdumdkwv.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2spjuntqb.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2tpbcltlw.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2hebtstfl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt2dppargqe.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2qpfssmgw.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2tsfhinit.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt2kyeexvtc.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt2hqfmzjml.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt2pludfpma.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt2mefrjibz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt2jlorfjzc.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2lqidzwxj.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2vufvnvee.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2gdyxonqe.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2pdsqtlmm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2kcnepbkd.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2eidrjegm.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2evnunkqb.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt2lmfpjzrm.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2vaoefamq.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2loexudxw.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2nrcbpyto.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2cgpkeyru.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2abimkblx.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2pgncwhfh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2ayfwwbbv.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2bpultwso.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2chllgbwm.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dhldwozu.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt2kxcstnwp.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2gguoqodj.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2qnuzeoqj.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fscnbnqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mvnjnojq.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2zenbwtss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fzpmbwcz.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2pyjcdexb.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2gtqcjedp.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fdxxiqnx.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2xbesarrr.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2shxgrtbt.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkzhtuzf.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2nirvgwmo.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2holltlog.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2fncdoexv.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2xwuugqdn.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2taasnnkx.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2fecpszzu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ankycgzw.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gsgcwshz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2rmotgarz.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2cdvqdmow.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2qceazmxv.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2zqjfxzmx.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2nqjiibgl.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2agyryscy.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2fejikpkm.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2odzzuhqq.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2fcpvxrxa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2ncntwmya.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2pqiribfr.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2qhmdbsjv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2bhuwmmif.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2lhbsoybs.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2dipsqokt.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2wrzmwqrl.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2wvtwzgot.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2fbnqmtwt.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2izbxfasj.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2cbwpixwy.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2ysyhlnmy.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2uctnakvv.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2xbbgorjr.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2rsaxsfpb.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2vhvmxjyp.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lombkvks.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lobfkrkz.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bybjfogm.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2knhvlpdc.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt2eaelxjqx.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2tdjfhtvc.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ljpruwav.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2zdpgrapd.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xkwhczbu.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2coovfdjn.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2gfnsussi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt2xdbexgzt.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt2vdbntxzp.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt2tfnylwox.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nsgcptsa.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2cdofzlgz.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt2ywmycwqm.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ytnmhtit.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2xagxksza.html


<!-- 参考信息 -->