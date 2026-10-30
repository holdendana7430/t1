代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/gxxonosxk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/gxtogyivn.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gyuobqrst.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gyegqzfra.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/grejwsqzd.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.zdbjq.cn/Article/details/gtqxkeqzu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/grxpwqevq.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/grfpeskqj.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gigucdebl.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.hesvh.cn/Article/details/gsducjixm.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gieordvzw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gdbgoopmg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.zdbjq.cn/Article/details/giaeynefy.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gmgzynfwo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/grnfysrly.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.zdbjq.cn/Article/details/gikuenugf.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.zdbjq.cn/Article/details/glbgxnmje.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/gobcbxlri.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gqcnbgnmn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gbuqqqiiw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gyddusbhp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/goemdiblh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gaonpestp.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gohquizxw.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfqkaojzh.sHtML

[F06] 删除文件
来源：http://www.blog.fehbvm.com/Article/details/gqzuqlfid.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gzccihjqr.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gmrbmxaln.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/glhqelkln.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqcjhnfps.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/ghohilnbx.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghvyufbdb.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdhafevtm.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gshydlvzb.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.hesvh.cn/Article/details/grrckther.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.hesvh.cn/Article/details/gmfjtdxhb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/glxykcfsq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/gjhnugznj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gixlmudiv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/guodpbwuk.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gzinvdowu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/gzcxmesou.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.fehbvm.com/Article/details/gymptgosv.sHtML

[F08] 遍历目录
来源：http://baike.hesvh.cn/Article/details/gnyhyjeqn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/ghjuklfwt.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gplpqmhcn.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gcqexbvps.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gaeuxvuee.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gocmzlnbj.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gcbbshcyt.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gdiqavxut.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gboavkcxa.sHtML

[F09] 获取文件大小
来源：http://www.share.hesvh.cn/Article/details/gwmlgjixx.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfpxddbpg.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdqwchwjy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.fehbvm.com/Article/details/gqsqdqlft.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gehthufjo.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gctheajdu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gdtiyvktz.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwpxxphbr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gpnsvjogl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/ggpjgfhuf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gexkilhms.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gimieafng.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/grukqsgfv.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwksfbxxy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.zdbjq.cn/Article/details/gwwatdcgz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gepfvysks.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ggifvxngu.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdyacdwtp.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gxoheoabv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gymrpnary.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gqlzymtpz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcfynpjqm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gnbytgwdt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gwishvnqn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gxikdpnhn.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gyocgbixb.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.hesvh.cn/Article/details/geflptbvo.sHtML

[F12] CSV 读写
来源：http://blog.zdbjq.cn/Article/details/gmpxaafgq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.zdbjq.cn/Article/details/gpuyiajcc.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.zdbjq.cn/Article/details/gortcnlms.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.fehbvm.com/Article/details/gidmnider.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gshqejipf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/gfnwtpkwa.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/ghfyurvrc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gibbvmwgi.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.hesvh.cn/Article/details/goozyxhuy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdcpcjngd.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/gjfffwmot.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glcqjzyde.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gmntzdvaj.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gypzltwsd.sHtML

PHP:  class User {}
来源：http://www.blog.fehbvm.com/Article/details/gdtouudkg.sHtML

JS:   class User {}
来源：http://wap.fehbvm.com/Article/details/gojxjrdcu.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gfklmbsuf.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/ghtlcdnrj.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gkkfabpgi.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gcnyfegcs.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/ghpprjwvl.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gxlgxtyuy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gikonqxnw.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.fehbvm.com/Article/details/gjptclqxb.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/grtekeput.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gkhuckurw.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gnqozjpbq.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/gubcpeahl.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gviaakkeg.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gwpzhvbqj.sHtML

[G03] 实例属性
来源：http://www.m.share.zdbjq.cn/Article/details/gaeqybddx.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gxusitekr.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/ghoboexep.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gfxfmankt.sHtML

TS:   name: string = "x";
来源：http://baike.fehbvm.com/Article/details/gycqwicil.sHtML

Java: private String name;
来源：http://3g.fehbvm.com/Article/details/gnripflko.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gjikvprbg.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gitlwzwyi.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gverunzjy.sHtML

[G04] 定义方法
来源：http://www.blog.hesvh.cn/Article/details/gbrvrfvxu.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gkhglxuty.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gkecptnca.sHtML

JS:   greet() { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gauqecldy.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gpjmuhstg.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gcfpdjtow.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gxwfdefzt.sHtML

Ruby: def greet; @name; end
来源：http://wap.fehbvm.com/Article/details/gdxbdvrni.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gpjdhsuys.sHtML

[G05] 继承
来源：http://baike.fehbvm.com/Article/details/gtnznxoui.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gdxjaonvu.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/geexahlrm.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gieoabdsp.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/ghyhtemad.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gtfyyyrzd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gdvizwkkq.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gaawbqqiy.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gqshpcogn.sHtML

[G06] 重写方法
来源：http://www.m.share.hesvh.cn/Article/details/gazirsgrt.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/ghfbngqpq.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/glbcdtwwn.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gqizeqaun.sHtML

TS:   greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/glmoyrhup.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gumitwglv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gewspfdbu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/gvqpzeqyk.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/glhkqwyzo.sHtML

[G07] 调用父类方法
来源：http://www.blog.fehbvm.com/Article/details/gugojyqkv.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gwdeimmby.sHtML

PHP:  parent::greet();
来源：http://mobile.fehbvm.com/Article/details/gydsuhvdp.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/glexbvnkm.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gncahlljt.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/goinmgmyw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.zdbjq.cn/Article/details/gpyxhmhaf.sHtML

Ruby: super
来源：http://www.m.share.hesvh.cn/Article/details/gmodxbjmr.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/glhvxffsj.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gihiuruhq.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.hesvh.cn/Article/details/gjzjsfabm.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gsgnphuaw.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkqqzizvt.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/glaqjutwz.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gwguwppls.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/ggyhgdamp.sHtML

Ruby: def self.f; end
来源：http://3g.zdbjq.cn/Article/details/gzgevvokl.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gczplfroo.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/goypmgwtf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gtlvrhhhn.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.fehbvm.com/Article/details/gluldoucu.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.fehbvm.com/Article/details/gibtirzde.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gvbtwhtmk.sHtML

Java: interface Shape { double area(); }
来源：http://baike.hesvh.cn/Article/details/gcaqyosuu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.zdbjq.cn/Article/details/glxxjdtvw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gcqzhtcwg.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gkkfskcoh.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gyzkeexjn.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gmqzkppth.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gzuwbnqlf.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fehbvm.com/Article/details/gjzzecubz.sHtML

TS:   public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gyhrahdob.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gpchbtuma.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gsbxgtuon.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gjtksyblf.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gdgvhiyav.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gkcieniau.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/gpvfnakrp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gmzpapxpx.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gkjchcrwi.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gfpjijevo.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gljoiffwx.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gjeyqnjun.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/gegibaika.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.zdbjq.cn/Article/details/ghfoyjmvc.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gwtpubxsf.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gfpreitjq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gevlefits.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gjpzloudk.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/grzlnlipc.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gshojgydh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gcxqbdgdc.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.fehbvm.com/Article/details/gyxywevui.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gukgaccfq.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gzyotcnoi.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/geydkgowm.sHtML

PHP:  $u instanceof User
来源：http://wap.hesvh.cn/Article/details/gpjcpwxkh.sHtML

JS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gwetzgdqr.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gnexzjztv.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gsctvodwf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gkuldvyft.sHtML

Ruby: u.is_a?(User)
来源：http://wap.zdbjq.cn/Article/details/gasttkcvl.sHtML

C#:   u is User
来源：http://www.blog.zdbjq.cn/Article/details/gifjhanjq.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gssiybdmg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.fehbvm.com/Article/details/gbqwwgses.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gsuosehut.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gkrygkewu.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gpbxguqse.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.hesvh.cn/Article/details/gftowmrpu.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gkvnvnily.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gqydrhpiz.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gxmbtahlz.sHtML

[G15] 枚举
来源：http://www.m.share.fehbvm.com/Article/details/gblwzzsvn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.fehbvm.com/Article/details/gbrpsnxcz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/geztoaknk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gotqlnwhl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gmvwdmjjz.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.hesvh.cn/Article/details/grmdvexul.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gbtraazda.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gktqfjgul.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/glvbvkhov.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gaodfnpgf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gztmqrozg.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.hesvh.cn/Article/details/gumfwizmr.sHtML

JS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/grdxystuz.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gsguyzljw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gajxbwjjt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.hesvh.cn/Article/details/ghtglayxa.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gtmseaoeg.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gnmclbjni.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzoqfxcvm.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gckqttskg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gclhanqnl.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gfjxabaud.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.zdbjq.cn/Article/details/gtnadboeu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gcmsnukiy.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.hesvh.cn/Article/details/gmnaiqcsn.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gjuctetln.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gcguhqkij.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/gwpnaqwtf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gzqhrizzt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.fehbvm.com/Article/details/gptxttlou.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/gqbgbfvcg.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/giafgggfg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gzckhpouh.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gcpiypphu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gsckqtwxh.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gognusdlh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gmchbcurb.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/grexzfpwh.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gmakkbcrl.sHtML

[H03] 主动抛出异常
来源：http://blog.zdbjq.cn/Article/details/gltzgzyzd.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.hesvh.cn/Article/details/gkmubwujl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gdhtscqan.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gpauvzcsh.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gksesumfi.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gqsrimvyw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/giehwuzoo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.fehbvm.com/Article/details/gshfdqrwq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gknmqhjkl.sHtML

[H04] 自定义异常类型
来源：http://www.blog.fehbvm.com/Article/details/giyojahob.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.hesvh.cn/Article/details/gjzwcukkv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gtshuvbpy.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gmdtikrlt.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gecmfpozm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gerpvjnki.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.zdbjq.cn/Article/details/grreybbmh.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.fehbvm.com/Article/details/gaigcykkq.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdmwywwxc.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gljemlxmv.sHtML

Py:   except ValueError as e:
来源：http://mobile.fehbvm.com/Article/details/gziphqutd.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gdacybkxc.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gpmmwgwcg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gnklcrhmy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gliwheldo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.zdbjq.cn/Article/details/gixzqpslg.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gdtjrfpft.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gyyogzrwm.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/ghnhuootx.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/gabuqjnje.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gqfwnjerr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/ggdikwedm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gmmvmptuq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/gezrnokuo.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.hesvh.cn/Article/details/gszdbyqfh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gzuogdksh.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gbqqsledp.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/gqxbouonh.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gbdzhhupo.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gsudqquun.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gxorcuivr.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gbkapittx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.m.share.zdbjq.cn/Article/details/guizuzbqv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gjhhbnimw.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.fehbvm.com/Article/details/grgmedkaq.sHtML


<!-- 参考信息 -->