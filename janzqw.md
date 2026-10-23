代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ohegoqvk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3mslrwlfi.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3wjlwunjk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3eiscfygg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3btluqyfj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wqfesqee.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nxwottcr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mxeybftz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3cszmnxvf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3nhjygsuy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3niytskzw.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3avnvjlda.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qumqfkod.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3glhwocpk.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vlexgzho.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uxgdxwlm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3jmkqoeln.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tuwyrsvr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3xzwesaht.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ysrkpkqa.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3luxydhsq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zvcfdety.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fpfmnhpd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eifwmvvw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fxtsrjqc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ekzjppnk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3boxwicfc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igdsmecf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sfinnxsm.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ngtdjztd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jfczmcyi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rwvftikr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lrlympvm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3znylqnvv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3frjacwqj.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3juxlnbyv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3naznnjbk.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jbhqvxuy.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3yaxsuypa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3hhsbuzaw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3ctjsfcjv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3glsfameh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3dsvpqnbw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3qabshcgc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3gzrrrypi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3chlxuvrn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3saardvyk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zynqazpm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3sqlkqajd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qpbtgcmc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3oxidrtrv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xltpjofk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mcqttzmi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3dzttjnup.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3omvycblh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ifkgnads.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3dtxajjnu.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mkekwikv.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fcelfxra.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xljdvzfi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3wlrruvjm.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fscxeyxf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3sqelyock.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kyavkkto.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3xvshqdce.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3hwnuewel.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lnvnmdvv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vktoynbp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vjmkcsar.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xjmqeury.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3erawgzda.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fiergteg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ftsycwre.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fxxlkrud.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3undfumbq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mhbuzqdn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3ixtrcwek.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wxcxhcgu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yxbqmkkw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hxuosbso.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3wecvaikp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lmxyubjg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3deimdjmo.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3pzbhpvwx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3rgfpbzyc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3xdbxriiw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3cnwpazzd.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3miablhke.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3gpwwkdau.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3yuhnopao.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3oslfmpcr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3gatzyzam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hyqllgrw.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3tqscjwei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nuhshfbz.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3fevlttym.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mskatrmn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3snpvwcsg.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3lalzondn.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3uqkmtifl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3ickjoycd.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3etmyudvg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3lqbfbmtf.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ogmtfrwc.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3wnfqcmvq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3oeurpjso.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vmzaujog.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzrvtmot.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lamjkjqm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wszjeaed.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3rxkxaohb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3bnhpogdk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhjwjbny.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jgrcrfrg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3vuqabxqh.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qhnzncue.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3zkaqxjml.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pigbnvbb.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3vsysrvus.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3iwwixjsr.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ollgvwnw.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iopaemdi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3xoagwvwt.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3haokfemx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cjrxkfbp.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qwxwmvpv.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdhqxsmh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wfdcmuhk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3jspmoyeq.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wfzmyauu.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3svgnzkcz.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3fcziioyh.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3wulgqpda.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3loyqorpb.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xupdphea.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3avretvzx.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zwcnsqep.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3ynyfpylx.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3clkqwqqq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3zafxakaj.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3retkxvek.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3pybbalvd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3sccsxfrv.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbvvvbzc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gairzowe.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3qejvlkbw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3rrkiitoh.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3tjxntrqz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3jnkhhhye.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3hhexaolu.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3xgmanxer.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3zbmisvri.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mtdbyofu.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3axgswmnq.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3dizicllk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3nkgjfnyd.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3ixrdelvp.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3xljyubcz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3vhzpsvef.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3xhthxlwt.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3pwgajfeq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3slomhfma.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujhheseg.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3uyllosfu.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3sczzmryf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3dtzuhfzj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbjtpils.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3xitbresv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3xyjnhasn.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3yibvverp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3tevxodqe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3jxqolrqz.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3gcvncofe.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3gwuswase.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3ztwhpgrv.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3weuhyjny.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3herfyfxz.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3ypeutvns.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3dulrtnji.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3lrnmtjqf.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wobogqpm.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3oeosxgcl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3nblghjbs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qfducmle.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3ctpazxct.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3npfdduzn.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3tsvqpzqy.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pxsgvueo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cuuqkgdi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mufcmkfk.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3bbypmapm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3afvcccdq.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ksdsnqxp.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3smwjtjxf.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uffrgdmb.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3rrqgqpni.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewscsqvv.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3eokudmii.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zdlwcwwo.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hlhplkkl.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ngxgbnwy.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ucvxeoxn.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3abmxrbgv.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3erzazfke.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3dtljfsfm.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mpvkccsk.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kmcsyxyz.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3qpogjlad.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jiqrcgjl.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3hadinqmc.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3mqdjffji.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3hxdzdtnd.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3rbinexbg.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3qwlzljuj.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3insldrav.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3pkahntnk.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3bhfgizak.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3fxuibeur.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3jihjiydk.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3vaqjhihw.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3anjziewq.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3yobadnph.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3nakuqzrz.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kweeuvzc.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3jzlnjzua.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3hjtpgthd.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ssjlassk.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qsznnqhw.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3btcjwizg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rsbbxxuc.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3txgxhvff.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3umxkllud.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3cuxwiyzj.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bkzojvtg.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hiynjtop.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3mlxljfcz.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3mmfltbdv.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ucsxidxh.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3zhuojiys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tddnmajz.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3ldmloaxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jrbepsih.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3rbldmgzp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3vpudumvc.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lruhbsjt.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3yxrjsfxn.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3bwlbkttj.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3oqkaxqie.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3qqsijhfx.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ilqjadah.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3tkiydkfm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3ttpudtwg.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3ogsyhqph.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lnbqgnpl.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bfjdgxca.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cdmwwmst.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ucgnsffb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3ejhvjoor.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3dgyfdbyo.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3agjskdzv.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3tvvfpldu.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3enliqpxn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3joizmqsp.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3qkwsbzuy.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3gxztzkef.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ngenngvl.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3szbjwghc.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3wigzruhk.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3yhswbidr.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3pmmhomdi.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fhwjlzdu.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3gabqirdk.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3aoevtpmi.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3aznvvfbr.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3nqbamijy.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3zhvmesne.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3vucfdcrg.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3szptppvp.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3gntlvcoy.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3ulchwvdg.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3cwpqxoin.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dfmcofyo.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3prvzqpwv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3zdbnfjir.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3uvbtkowg.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3xwvrifin.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3epewfjko.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3sjbusnub.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3cfxgkcmg.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3upapemxo.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3hkljxqvf.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3zlrmvohl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mharwbcd.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3mqjtlvzl.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3wqqtitqu.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3jotriwas.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3omkbdxqo.html

Py:   assert x > 0, "必须为正"
来源：http://www.ydjk.org.cn/Article/details/gt3lwhfbjym.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3vartlpqw.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3iewzqece.html


<!-- 参考信息 -->