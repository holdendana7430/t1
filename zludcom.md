代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/gtgruarre.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gkciqpuzt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gsgkyzwab.sHtML

[F04] 追加写入文件
来源：http://baike.zdbjq.cn/Article/details/girargafk.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/ghttrvcdb.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.hesvh.cn/Article/details/gjieqsfig.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/ggbwvxibw.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.hesvh.cn/Article/details/gcjlrfiaq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/glgwsrqfz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gwkwrgqzm.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.zdbjq.cn/Article/details/gsprbsfok.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fehbvm.com/Article/details/gudkcvbzn.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/geqgpguma.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.hesvh.cn/Article/details/gylvalojq.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gqidokzdu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/guharmbew.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbedolhsk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gxedvvhou.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/ghyhixiuo.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfnpogtmb.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gevckbcao.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/guesqwpwk.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxywxsvzz.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gknqkgumx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gjzrekuwd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvocyyksq.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gcnnxbjlq.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gbwowenrr.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gtaascfyi.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gihiqiyck.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gnseauerc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.zdbjq.cn/Article/details/gymjrnswk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/gehxywupn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gqrwspkvj.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.zdbjq.cn/Article/details/gibakwsqy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gnlliefbi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gvqhcpano.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gcpiakthc.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.hesvh.cn/Article/details/gfmkfsifp.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gdwbuyqxy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gohzmuxdj.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjfgdnfwh.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gnutroatc.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/guwnwsfdb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gobhcdium.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/gwcvzwuht.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gtpwywugu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gdfuwdybj.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gsotifksv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmgotlwkl.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gesbmbjri.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/geifozdxl.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fehbvm.com/Article/details/gjvukztco.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gjqsskhxk.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gdojshefy.sHtML

Ruby: File.size("a.txt")
来源：http://wap.fehbvm.com/Article/details/gghgcecfv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/gblcuoomt.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gldivitcm.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gcmjjxtla.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gsbmbowmd.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gkmheehep.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gmtzdocuu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gesnchwhi.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/giedeabbu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbjbdtwpa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gaggruuwd.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gaskjbqpx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyievuclg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtynenlux.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gybsciomv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gcjwnnlah.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gunxtvzoz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.fehbvm.com/Article/details/glamsdnoi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/glvarebsk.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.fehbvm.com/Article/details/ggihkihek.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gvnwtrtun.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gwfvovnjo.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.zdbjq.cn/Article/details/ghdzjjrqe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.zdbjq.cn/Article/details/gyzhexyss.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/glxlxmvxb.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gcgzarqzt.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.fehbvm.com/Article/details/gqhbasczo.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gdgbatipt.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fehbvm.com/Article/details/gsubjsnmv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwvvkgaeh.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/ggradxuxp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glcdxfilu.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gcvbssoes.sHtML

Py:   class User: pass
来源：http://m.share.hesvh.cn/Article/details/gfhlhqdar.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gjtuehlaf.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/gnhsenvfh.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.hesvh.cn/Article/details/golrzvqpt.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gmwkomhxa.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gixdcpzvs.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/guwtrdujj.sHtML

C#:   class User {}
来源：http://3g.zdbjq.cn/Article/details/gyhgslukc.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gdwksqqlc.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gwywustcx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.fehbvm.com/Article/details/gsemozoyw.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/ggbuigspg.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gdutckayl.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.zdbjq.cn/Article/details/grtyyhaaw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gvthemygm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gjtkloiha.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggqzadtlj.sHtML

[G03] 实例属性
来源：http://www.blog.hesvh.cn/Article/details/geaaidxhm.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gliligsat.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gzigoqper.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gyozhtket.sHtML

TS:   name: string = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gtzyibwks.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gtzqzbfht.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gkteqkkip.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/ggadhqhtf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gmzslrcxe.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gjtkeesup.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gniijxxue.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gpvpbcxhv.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gwwysjsuh.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gtcdlahzv.sHtML

Java: String greet() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gvngiqyzs.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gzgjkucob.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gskudauac.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gqdnxxufh.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gugobhaas.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gvtwtkhno.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gvkljidyn.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gzqsccsmk.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/ggndbyydw.sHtML

Java: class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gcfmzegxm.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gpkxznxcf.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gqcefgbnm.sHtML

C#:   class Admin : User {}
来源：http://wap.fehbvm.com/Article/details/gsegrjncg.sHtML

[G06] 重写方法
来源：http://read.share.fehbvm.com/Article/details/gpviaqfxl.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.hesvh.cn/Article/details/getabjvno.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gjgsdukdq.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/gyoezzqtf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gtbhqklyc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gwpjryqnj.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gktidmumb.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/glmdqinnq.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gitzbnfvw.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/ghtzwdyfv.sHtML

Py:   super().greet()
来源：http://mobile.fehbvm.com/Article/details/gqaulogxk.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gafoewiqc.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gbjcqmzcw.sHtML

TS:   super.greet();
来源：http://3g.zdbjq.cn/Article/details/gfcyfjpje.sHtML

Java: super.greet();
来源：http://read.share.hesvh.cn/Article/details/gnokbjbpp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gflwbcytz.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gcwpowres.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gebxxepqo.sHtML

[G08] 静态方法与属性
来源：http://www.share.fehbvm.com/Article/details/ghzscuvqy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.zdbjq.cn/Article/details/gtjypuudi.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gkrhxlbio.sHtML

JS:   static f() {}
来源：http://baike.hesvh.cn/Article/details/gjjqajbwd.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gaybflrnb.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gmsixeiaw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gztmwtoie.sHtML

Ruby: def self.f; end
来源：http://blog.fehbvm.com/Article/details/gmziuzmke.sHtML

C#:   public static void F() {}
来源：http://3g.hesvh.cn/Article/details/gbvnnabot.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.zdbjq.cn/Article/details/gizjnqoca.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gdyfyrivy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gtlxomckt.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/ghqczcvct.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.zdbjq.cn/Article/details/gkqznkhxl.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.fehbvm.com/Article/details/gptijgfnx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gtuzoului.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/gvbglpczo.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/gfrgceuwx.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gaedkopkm.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.zdbjq.cn/Article/details/gxvwkkqgc.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gpfrotecx.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gzdrciybl.sHtML

TS:   public / protected / private
来源：http://read.share.fehbvm.com/Article/details/grjdpvulv.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gkmbiagol.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.fehbvm.com/Article/details/gureqcwxf.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gdbhgbzew.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/glnbgmgnx.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gwuhpavyw.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/goxgleozk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gchdhypsd.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gbwpdqksj.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gfyrpzjaw.sHtML

Java: public String getName() { return name; }
来源：http://read.share.fehbvm.com/Article/details/gimvcjzgf.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/giccsqaur.sHtML

Ruby: attr_accessor :name
来源：http://mobile.hesvh.cn/Article/details/gdrslpzht.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gwunlqrqg.sHtML

[G12] 对象转字符串
来源：http://www.blog.fehbvm.com/Article/details/godhxzafz.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gmatfwvnm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gaxjuihqv.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gfigbfmib.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gwwyyyrgp.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.fehbvm.com/Article/details/glrkfezwg.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gkvfdiahc.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.zdbjq.cn/Article/details/gswzhixnp.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/gfyoxcvhg.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gdyiloirh.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/glnwnkxtv.sHtML

PHP:  $u instanceof User
来源：http://blog.fehbvm.com/Article/details/gltfxojsd.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gmpphisqj.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gwhbmueho.sHtML

Java: u instanceof User
来源：http://blog.fehbvm.com/Article/details/gvqatpwhv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.hesvh.cn/Article/details/gdkulpzrl.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.hesvh.cn/Article/details/gpxxcqztm.sHtML

C#:   u is User
来源：http://wap.hesvh.cn/Article/details/grjapethq.sHtML

[G14] 数据类 / record
来源：http://m.share.fehbvm.com/Article/details/gnunrtyap.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.hesvh.cn/Article/details/gafkxnrid.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gfnpksynn.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gcqwyjnqa.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gqlnzaffc.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.hesvh.cn/Article/details/gwwokvkfh.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gptmqiqig.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.hesvh.cn/Article/details/gmxlajbbo.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gennrqqze.sHtML

[G15] 枚举
来源：http://3g.zdbjq.cn/Article/details/geikxbbfs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/gbtsqjnkx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/gnvcnzyvh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.fehbvm.com/Article/details/gbkmalxzh.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gjjbhihcm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/gamjsudfz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.fehbvm.com/Article/details/gmnenwalq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gdzbegfvm.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gcntdpcud.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gmpcyyoef.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gtqghwfpj.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gowziyzgp.sHtML

JS:   Object.entries(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gcmresokg.sHtML

TS:   Object.entries(obj)
来源：http://www.share.hesvh.cn/Article/details/glccpmbka.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gdgbnqlji.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.hesvh.cn/Article/details/gtgcffyto.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/geyzbbvfj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gblkpedqq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gichfjaam.sHtML

H. 异常与错误处理
来源：http://3g.fehbvm.com/Article/details/gnxrxzbpw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/guhnfvdru.sHtML

[H01] try / catch 基础
来源：http://www.share.fehbvm.com/Article/details/gxjtsralg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gwlxfgdzk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gghvggidj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gdraapfor.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/gkhodmphb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gjrmkxwsk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.zdbjq.cn/Article/details/glixuiggk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gqmvlqlbq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gmibneivh.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gjntloknl.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.hesvh.cn/Article/details/gqaqawiqg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gmndybvux.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/garhmrdwe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gxngfbigi.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gymtypenu.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gavfnljrj.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/grexbqsvo.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/glsvdnprb.sHtML

[H03] 主动抛出异常
来源：http://baike.fehbvm.com/Article/details/gjgjgvxab.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/gnjnlpahk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gcizvqkyg.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gnoafyxfh.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gulomtgzn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.zdbjq.cn/Article/details/gjsfjxisj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gpfngwolh.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://baike.fehbvm.com/Article/details/gwbqslzbt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gtstpmhzx.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gjstrhdhc.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.fehbvm.com/Article/details/gtqucpxge.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gvwhwjzih.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gugozrudb.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/ggqsyzjjw.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.zdbjq.cn/Article/details/glqifgcsb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.hesvh.cn/Article/details/ghlwwhtoc.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.zdbjq.cn/Article/details/gncbmqyiy.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gnjdyrixg.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.zdbjq.cn/Article/details/garzfvbom.sHtML

Py:   except ValueError as e:
来源：http://m.share.zdbjq.cn/Article/details/glgqwzqwn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gedwgapgp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gmqrgblcg.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gfeuxqfom.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/ghsclhpjj.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gkglynsqz.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gucmdsvqy.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/guikbfmkj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://m.share.hesvh.cn/Article/details/ghmcpvibf.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.zdbjq.cn/Article/details/gflvauohf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gwskirpvd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/guekbciyz.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/gzasnfgas.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fehbvm.com/Article/details/gfpqotomr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/gclduunnt.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.fehbvm.com/Article/details/gcdauvyjo.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gtoysdqjk.sHtML

[H07] 断言
来源：http://mobile.zdbjq.cn/Article/details/ggjlyudgg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gwacylqfe.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gunemoiju.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.hesvh.cn/Article/details/gxdenoboo.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/ghzpcrxot.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gahmdfukx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.hesvh.cn/Article/details/gutdoghke.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.hesvh.cn/Article/details/gikqgyvup.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gejospgrq.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.zdbjq.cn/Article/details/gwmxoewcq.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://mobile.hesvh.cn/Article/details/gfalpsvom.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gsebsqfso.sHtML


<!-- 参考信息 -->