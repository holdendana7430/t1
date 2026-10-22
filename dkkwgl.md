代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2pjtdcdrz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2hmmaxwvx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2stjcmild.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2jkdisoma.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jxokkukj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2eiicusyc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xrdsmrbn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2twrwzhmi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2nxznliih.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2myzknugv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2johnqknd.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2bvgciohf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2izuxdikn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2oxjqhpsh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2offiauhg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zsbpclfw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2awawnevh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2epxisnis.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2irjrzzda.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2sdwfegbu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2aeleaqqw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2czkqsvzn.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bfdqaqut.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wrmnucyn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mpfvbfli.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fyczthqg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ucurydhl.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2onfstzer.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lkvrvpim.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dmreezlx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wnpngusi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2woattxrp.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ldwzlhhr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2paglfgoo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hrchzkmc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2peaourmn.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2isagojck.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nttsbywb.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2vzlrbdyc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2fbegjaxs.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ftuvhpst.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ktzcacef.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mdkdlcmz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xfddlbdi.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2jgwyjiag.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2oqllrxmd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2uihxetsx.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2jcwwmgem.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2cmsvcqvd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2dtdtdeaj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gsoovzei.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bjmnwjdo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2flgvqkuh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yqjxlsai.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2iwnmixuq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xebscnag.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2pkpjfaoz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ffqigplb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jewxlgwv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2iciuxqqm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2skhwjotc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2skqjcxcb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2nwspcsie.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2txaryjkd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2jpplwjht.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2bpmxjcow.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wdvmvnao.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gmwqqdzd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hsphvvdw.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hwfgoevu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2sjdsgsxd.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2glkyhqrr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ejfzjquh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2meewpbue.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2cglnzqsv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2tefesivj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2agsejrpu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xhejmvna.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nmgcwtpv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rnabgfgx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qulchsek.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2epdkwabn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2tzhaqzfh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2drilrruz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2gxpunpug.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2dmxutdam.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2hipnegef.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fdoljzfo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2bsuuhbas.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2szbstimd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2kzfnhaqp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2agtplcoj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jxwychxe.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2plxniuko.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ynzwoxax.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2uaggufzl.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2stdodogn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bycneage.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hthksrck.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2lpdlqevl.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2joklhnfu.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2hrxywriw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tyslwuqs.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xoibhaxc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2vpvjoebm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2zcazleqj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2dxxernlg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vlmwbfoc.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2nwregbez.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2gropcbqc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2clltxehz.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2egueofbj.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qbzuywhs.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2kkehtgjb.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2deomuffn.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mqxonxbl.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2khijuqxc.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2drbuaeqm.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2dgtxwvym.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2skhmyvim.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2ggyfoxvb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2cxithwya.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2sjrvdjtm.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2plpvnzso.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbcccssq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ajlhjjsr.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2wreaifig.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkckfros.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2llgewmzs.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vtpjgebv.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt2smkpmfep.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2omuvuczm.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2xlyzhepc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gfmcbcpj.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2poocikmp.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2ualgqzni.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2zaoqigca.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2qboadbhe.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt2bimldvwx.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt2auqjrvjk.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2wcmrqdiz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt2ahcfugja.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2ajeeipwp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2knabuvpr.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2cyuipjeu.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnyjwwxx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt2sifzybdx.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt2olmdlyxr.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt2jgkbltsh.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2bhraqnsc.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt2omixesge.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt2ykisrwlo.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2jamzwubu.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2mhqtzoec.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2auywmsnh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt2chbpnemk.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2ykouryrr.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2gxzjbryy.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2vexkkdqn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2tekzlbee.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2thbgopzs.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2imsnuijh.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt2udokkjyi.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2ebkgjdeq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt2warujxth.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2mtawaafj.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt2mxacofib.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt2esucjrou.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2ybjrjzzx.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2flktgxwu.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2jsyowjnt.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt2vjqmsklb.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt2bqsgoybt.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt2kbyswtgl.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt2alzujsvv.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt2nqqxorxu.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2btoqequg.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt2pnjfcxtp.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt2oxiutpdd.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2bfjaefai.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2lubzdoqy.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2tefledtr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2nwnrdhxy.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2vsjfeebj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt2yqwlnqcv.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt2jgexrrtr.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2ossvnhfl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eleiqnnr.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbskbsnq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxaniejs.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2vnoczbob.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2eotpuycq.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2acvopiif.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt2grqdtzxc.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2noxvhljg.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2lnaotfhv.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhbbydyh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2pztxodan.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjxkzqdi.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2tcbzghhy.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2tufwxihk.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2dmtdgmvv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2ifznjlae.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2qtizypct.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt2jjnewfii.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2fukahonw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2uscuywnh.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2qgdpgcdo.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2lggjwlsc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2gnvxdlez.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2vhzedfej.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt2kppgatry.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2rhllqfpo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2yarrnysk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2bppjsiqa.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2gedzkckc.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2ufwlztzt.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2kfhywvmf.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2xfuvcowf.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt2vxdsyqek.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt2osdtrfke.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt2dkoijuls.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt2exvzhrxy.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt2wjwrkric.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2bhhvqqnv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2gddgttso.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2msgjizrl.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2xswhhkju.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt2dclhgclg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2ejiilfoe.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt2cmzztonn.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt2wxqmvkvg.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt2kgfkcmyr.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pcdoklni.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2nqnssdkq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2emuuumry.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt2kipmwuvz.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt2mspdtndy.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kjtmkwkb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ptcswyrh.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2pddkgfbx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klapvhhc.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt2urvonhpe.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt2bkvotahg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ofityrpp.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2oqnzirew.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnzjwbdn.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2jromohpn.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2sglcjypw.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2mfqsyatd.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt2nkwsabld.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2debbpuwd.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2ynnjfwpa.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2dmdeumes.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ycywnuhv.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2miubinei.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2adsxdjeb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2kulspmye.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt2gjyoynzr.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2alkjhgpn.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2acsswrji.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2ivzigkqi.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2sgsvxfci.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2hmmuriam.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2muknhpat.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2kpgntfpl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2czzzrujw.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt2nxypqghi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2rwddnzyn.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2wqryqyvr.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt2zwgwxftb.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2ctauohdf.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2bvkxgtre.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt2uksdljqb.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt2fiyzukox.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt2kaoadbro.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt2wbtdqyxx.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2rmuunerk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2dqlmfzik.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt2wjpfvvmh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt2aohfekps.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt2larxzmim.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mohedhhf.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hmrbhsqh.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt2yhztomnd.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt2yyaijwvk.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt2fukbrhok.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt2ahluofps.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt2lnqwooob.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2npreahqg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt2cilbynsw.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt2nlztoebq.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt2jffvcgnn.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt2cbmpqamz.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt2wgdzuehx.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt2uvjafpmy.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt2tqjmueev.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt2eahcotql.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt2mdyhnzpu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt2ftvtwjfs.html


<!-- 参考信息 -->