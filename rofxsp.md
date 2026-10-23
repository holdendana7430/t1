代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3gjktlyqa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3zyeakrlj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3onhdnjyn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3woewsvfy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3yyoomicp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ptpipood.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ibfzdvvs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ftpxhtcp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3oqrstuep.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wtdibmoj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kdzpqxep.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ewurmpfy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cdqmcaji.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3wgcbbhkk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vxlvtxtw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ezoilfcw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3hfcsfxvx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3wqangfgc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3vaxclfqo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3qkbasopv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zvrpnfsl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3qnpbrshh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cwbdsfks.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zesjwawy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hvrdktea.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yrcwyfxr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3frugcgsl.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lvjlmkhr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mrucbmyq.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hvsqresj.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dwuhtasl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fvuxmwrt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ptrevqfe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zvzlimrt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zqahbtsu.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uusdtugq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lpqekkdd.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rbnvbuic.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kpllnuxe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3vvwrfpgj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3taqzcjqs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vogvewbk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fnqzclmv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rrrreziy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3vjyaqjsb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ckvudvcz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3syhxmlqi.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3lcqewmds.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3yidryuqq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3wwfwqojk.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3svhznorx.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3beubhaiz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3yzofdwuy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ibcsprmq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3iwfionzi.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nnrmooho.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3uogxbmvh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rsqstjzb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ezbuglpj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mvkbzbmu.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cfytzuat.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rkpjjoxi.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3kskwtxhd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3icgowplo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3fgglksqw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3qpltlunw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gqphbxeq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mvochoqz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ivrjvqsk.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qtyswflh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3fouxpxux.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3binwljas.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uhmsnjpj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cdgwclvx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3uzzkxndm.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xpxjaxli.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3uchnnidj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ybhjkmbe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3altyusev.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3uiwdmkvx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3sdyjstft.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ffektwmn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3nxvpvegu.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3pywtjvmx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3itafrhac.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ziwcrbxs.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3hswedifm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3fqijjmqr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3easqnhbt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zahjfbja.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3grkkturr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3kczmjehc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gtdeuhln.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3sfhpvgdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yffwwjlw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3fxvthiwc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ammlvcae.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3lgsmgtba.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yyqpzpuy.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofukbjvk.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qazdatan.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3ycjtaluf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fcxxdxyd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xdqijhbj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3nxudjtpm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3ukkjwcuw.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3gwqdxzrw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zgghbkow.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzduivui.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gwqhsckq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3pqhuztax.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3qteqiwgm.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vhsplxpz.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3hjnqjooa.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3rqlpyqlj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rxxzvdbb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3hvmkjnih.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3hjbwidwn.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3foloncwu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3bbhtzgaz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ckljvpne.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3nsxuheik.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3jiqpvpma.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3vdlqzsfv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvmazvtw.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wabsjefk.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3dvjicyla.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zpitovsg.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ayebxvav.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3aswyujpl.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3mhrkaaji.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3acqacadp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ofqnnolt.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3seycexwe.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3jbghhfdk.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlikkham.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yuyiswzj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3lfbbpoie.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3fnixllqy.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgmimwvo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3dnacbkes.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3wkephulw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bwyzctqz.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qjjdnlvq.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3snvgtauv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3oawzgjxg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.52xcode.cn/Article/details/gt3mgenxzon.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tskxsdlf.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ktasayoe.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3rhpblimg.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3fiixhgag.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3pfjvvnjw.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hciltzbi.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3dsatmsys.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xrpyfcsf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3egveasqb.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ujprsooj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3muxfkwgs.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3imijlplz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3sedyrhbf.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3mixzmuwk.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ocfbtjid.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ysbmecef.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3tkmqyddm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3geyxixqq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3omehafkg.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ackvqhui.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3tjvyplji.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3omgkppgy.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3cziwbawv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3boyihntc.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3wbcuhlzf.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3oyupuxde.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3ylesddnj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3litjazld.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrnhpght.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3qjyesgqn.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qnqrwmkh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3uzxmyqeh.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3ywhzptru.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3rhpzxsdh.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3iqbrunjr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3hmgzeqcb.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3ytjnmaua.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3tiurcwrt.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3agkpyddc.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3arzfwhaf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zhozvtdc.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ymvwcmvh.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jhthduos.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vjtzwwpn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3nuahoyrr.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3tsmglzrm.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ehdoustf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3amxysdao.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ukzrytyw.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvfzgftf.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3qhrmfwgj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uwnqaxzl.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qevhaigp.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jxjbzfhj.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rprbwsyd.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zkfntdal.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3absdcmiy.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3mrhjaknu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ffnpoppp.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3kpacimxx.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ayssygmr.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ipqzjhbk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3ckimhmml.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3nfyvypyh.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3mdefhwdh.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3nggbtqcz.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3uswybtlk.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3avekjfrg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3tdgbeagd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3bfvxyloa.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3qoxmvnkm.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3rshivvpw.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3ymwznfsn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3dbotlrcc.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3syzlzque.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3jzreomfk.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3fhaotgif.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3ldtnpxcv.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3kezkqmsu.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3ggvbzbof.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3pdhwinzs.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3zcrimmno.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uxthyvpu.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3pymfwxyj.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3xadgtyxz.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3dqitkxnq.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ofhxnltx.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vfmdhant.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3dloxhkmq.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wzkllflz.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3nelkfqdt.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3qtpdpzpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iaksuuuf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3lfgdjmnx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mlghyeyd.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3weagfjlu.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zezmoact.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3prrpsljy.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3idrweafi.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fdmxelgq.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3edchryhy.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3xidwxtcz.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3vkflhker.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3encglmts.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wzcralfh.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3xqryfxln.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymevcxif.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dqfsjkqy.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lrjwalpp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3grskjqko.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3xmjftqqn.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3klgipiqy.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ghttpwjx.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3yprdsayj.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3anpweoxa.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kmkwkfei.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3loudzagq.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xkvnlfba.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qsryaxuy.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3ladahaxq.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3bxzlquxv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3oiadnbli.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3xrdrsfdk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3krozcnht.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ikfantvm.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3rsnxfdhd.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3vituuqso.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3noqestzc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3ierqzmoj.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3pnyhudxr.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3zoaxqqsu.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3phehbxdy.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3aihaxljv.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3popikbvg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3mlntiapf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zsdrmdjc.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sckpcjsn.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3kpdocngb.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3ojsvjjsu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3lxryumgs.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3puvuemlx.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3wwlfxdon.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3vnrlzwxe.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3yphdizmm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3mwjkfmtm.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3tnwploxl.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3wbtpvbuf.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3kjdqiwcy.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3bhgdjvid.html

[H07] 断言
来源：http://www.52xcode.cn/Article/details/gt3enjgaddg.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3qvqniwpg.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oatpnplu.html

JS:   console.assert(x > 0);
来源：http://www.52xcode.cn/Article/details/gt3atsfklpu.html


<!-- 参考信息 -->