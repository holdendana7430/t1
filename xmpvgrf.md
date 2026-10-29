代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gjvpjttfq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gapmwzyks.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gmaortdcp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/guivkkezv.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gcvwyxraj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gxcfuciwd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.hesvh.cn/Article/details/gcuiajwnw.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gaqqyaloq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gglguxjuq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.hesvh.cn/Article/details/giabzjequ.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/glbmvuuog.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.zdbjq.cn/Article/details/gluqcqvqj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.zdbjq.cn/Article/details/gkasduvqn.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gswsxvqvz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gpcqaqabw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gglfghgoa.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gxndkfcrf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/ghfylbthr.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gjxlhdlpc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gdfvzjzsx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdehlemdr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gnuzrgovd.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gqdgncjmk.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.hesvh.cn/Article/details/gqqtgxwyx.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcxxagpgu.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/gtbjibuhe.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/geumtzruh.sHtML

PHP:  unlink("a.txt");
来源：http://3g.fehbvm.com/Article/details/gpfuphhpb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gaatgpzio.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gknxixlgr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gyxnzxnmd.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gydrfpacd.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghjxvnxvu.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/garupvofa.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.zdbjq.cn/Article/details/gcipbunrv.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gilpzqnnb.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gfspqotfl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gcmqougeo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gvyqkzicr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gqjcmfnep.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gthrdrbyt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gfnaacthe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.hesvh.cn/Article/details/gaxxedddq.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gmmqgrphg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gvpemoyzu.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gtahgoqfr.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gehzkvsqr.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/ggiycousm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.hesvh.cn/Article/details/grtkffdhl.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gufyqerfd.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.hesvh.cn/Article/details/glklxtsvk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gzcknwgso.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gdncpduis.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbdvyjoqg.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gabhxgdra.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gcgvdmrpx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/ggejihgwe.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/gjhlwwflt.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gjtmlekjh.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gcveijkmr.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gpvzykdrc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.fehbvm.com/Article/details/gcstadazy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/guweivhiq.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gmwtyzoku.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gycwtnssa.sHtML

TS:   path.extname("a.txt")
来源：http://3g.hesvh.cn/Article/details/gerqcbklp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/gtnadrbig.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gudpnwrsd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkrlsagwn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gycdigncn.sHtML

[F11] 复制与移动文件
来源：http://wap.zdbjq.cn/Article/details/guwiakodc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gupqmwsun.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gkjcdordx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gofrulgfh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/guqszsxcb.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.hesvh.cn/Article/details/glaypbhvr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gfnuzzrvl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwjpyyksr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.fehbvm.com/Article/details/gbcwxmkui.sHtML

[F12] CSV 读写
来源：http://www.m.share.hesvh.cn/Article/details/gtdeqelmc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.fehbvm.com/Article/details/gpgzqnjam.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fehbvm.com/Article/details/gwmgoqghx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gtxagumdv.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/gafsaxcco.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/glirkbmue.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gnqumhqjp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fehbvm.com/Article/details/gdoetuqyl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/gwarqetlg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/givqhzqgc.sHtML

G. 面向对象
来源：http://m.share.zdbjq.cn/Article/details/gtnxxuloo.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/glnsvuxdo.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gdehljpxp.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gjjyjdisl.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/giyoabzis.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gwvoyxlcy.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gkimdyrrl.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/gdmvybulk.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gvaurjtwx.sHtML

Ruby: class User; end
来源：http://mobile.hesvh.cn/Article/details/gbmufdvbw.sHtML

C#:   class User {}
来源：http://3g.hesvh.cn/Article/details/ghbijozxj.sHtML

[G02] 构造函数
来源：http://www.share.fehbvm.com/Article/details/gamjojlue.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gocbsarhx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gzruzkynk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gdmybjrbe.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gvrxmbwne.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gqoadrzck.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.blog.fehbvm.com/Article/details/gqbqbmimy.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gcusspkin.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.hesvh.cn/Article/details/gccgpsbmb.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gheleoflc.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gmmkafgcs.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fehbvm.com/Article/details/gpmloturv.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/grnrrwjmj.sHtML

TS:   name: string = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gkmknjthr.sHtML

Java: private String name;
来源：http://blog.hesvh.cn/Article/details/gcvuqqjuo.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/gwowatanc.sHtML

Ruby: @name = "x"
来源：http://3g.zdbjq.cn/Article/details/gtuogiwid.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gxkaxnbkv.sHtML

[G04] 定义方法
来源：http://www.share.hesvh.cn/Article/details/gekpjyzrj.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gkwcmvbgo.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gstluxgwa.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gsuapxcik.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gjxasdomm.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gqskhdlwv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gvinzouzm.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/geazebtpd.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gnysanjat.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gzjymdmaw.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gjqbsvqfo.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gunpfagob.sHtML

JS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gabgihyuo.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/gjhgrevca.sHtML

Java: class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/glolecokp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gsabxsrdv.sHtML

Ruby: class Admin < User; end
来源：http://blog.fehbvm.com/Article/details/gdfuijhqk.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gywogricf.sHtML

[G06] 重写方法
来源：http://read.share.hesvh.cn/Article/details/gkjmliyth.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.zdbjq.cn/Article/details/gwzvtisql.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gcgeiebyy.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gbbjzostq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gspgiihaj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gbfoytrmd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.hesvh.cn/Article/details/gzvaqgutu.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/grrqeoqcr.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.fehbvm.com/Article/details/gepcgdtwx.sHtML

[G07] 调用父类方法
来源：http://m.share.hesvh.cn/Article/details/gagssfknk.sHtML

Py:   super().greet()
来源：http://baike.hesvh.cn/Article/details/gxirsdymh.sHtML

PHP:  parent::greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gbbnjames.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gdjsjxynv.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gqodoczkh.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gzomeakog.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://m.share.hesvh.cn/Article/details/gdcqttixk.sHtML

Ruby: super
来源：http://www.share.fehbvm.com/Article/details/gjisfbwua.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gioppfvot.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gnglmmqtg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gxczfafkl.sHtML

PHP:  public static function f() {}
来源：http://www.share.fehbvm.com/Article/details/gbatwvtgd.sHtML

JS:   static f() {}
来源：http://blog.hesvh.cn/Article/details/ggwznuvtr.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gbklbvzre.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gozmxwrhb.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.zdbjq.cn/Article/details/gbtgunori.sHtML

Ruby: def self.f; end
来源：http://mobile.hesvh.cn/Article/details/gfcgnzppb.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/gaxmkyybh.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gnqtlwnza.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.hesvh.cn/Article/details/gymiywjxs.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gdfxncbyo.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.fehbvm.com/Article/details/gehhebzhk.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.zdbjq.cn/Article/details/gnjhmzhvp.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.zdbjq.cn/Article/details/grpaabaef.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://read.share.fehbvm.com/Article/details/gferzkpgz.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/grntrjdeh.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gjndwcqia.sHtML

[G10] 访问控制
来源：http://www.blog.zdbjq.cn/Article/details/gzqqieqrr.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gqpitxaif.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gxlxxinsa.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/ghwueiygy.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gbrwzxxas.sHtML

Java: public / protected / private / 默认包级
来源：http://www.m.share.zdbjq.cn/Article/details/gyjspdzet.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.hesvh.cn/Article/details/gxnzblawt.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gzszvfprj.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/gpzonvpwq.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gfdnrhmcc.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.hesvh.cn/Article/details/ggwwgjrjb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gvmhbcfth.sHtML

JS:   get name() { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gmnpohmka.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.fehbvm.com/Article/details/gmvusyztk.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/ghvishxjq.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/gxyrvnemt.sHtML

Ruby: attr_accessor :name
来源：http://read.share.fehbvm.com/Article/details/gosvguanf.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/glctuockb.sHtML

[G12] 对象转字符串
来源：http://mobile.zdbjq.cn/Article/details/gutzhgjoh.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.zdbjq.cn/Article/details/gzfjdprns.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/ggcbjaksv.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gvhtebopk.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gebjqcyho.sHtML

Java: @Override public String toString() { return name; }
来源：http://wap.hesvh.cn/Article/details/gcjlpfqya.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gsxhjtkrv.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gryqxvoxj.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.zdbjq.cn/Article/details/grzpruybk.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gibgukpjy.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gtvfxwoxj.sHtML

PHP:  $u instanceof User
来源：http://baike.zdbjq.cn/Article/details/goxguvzcp.sHtML

JS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gpugppabo.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/girveqmwv.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gwhyzwjgi.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gvrzdehqg.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/goaowauss.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gojgfcvge.sHtML

[G14] 数据类 / record
来源：http://www.blog.hesvh.cn/Article/details/gtusfdsfv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.zdbjq.cn/Article/details/gbgtcyktn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/ggmyepbkv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gncdahcjg.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gstrsjeya.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.fehbvm.com/Article/details/gmjoatxll.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.fehbvm.com/Article/details/gazaojobo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/glpmaajju.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.zdbjq.cn/Article/details/gfrmgazzq.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/geikictxe.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.fehbvm.com/Article/details/gvncdkeqw.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.zdbjq.cn/Article/details/gemjwespn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.zdbjq.cn/Article/details/goiblcfij.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gcnousqrr.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.fehbvm.com/Article/details/gcixismgx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gqaznfpwp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.fehbvm.com/Article/details/gntnokqla.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gxyezbnlf.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.hesvh.cn/Article/details/gtssansrr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/gxfenrher.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.hesvh.cn/Article/details/gtnipdecm.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/ghiwazyff.sHtML

TS:   Object.entries(obj)
来源：http://blog.hesvh.cn/Article/details/geeocxwla.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gouyzrjvz.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gjixmrltx.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gvyhqrnfu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/grnhqzdyx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goaitfedl.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gpcofxglw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcerwxexd.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/grnnwruzf.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gghiboasp.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.zdbjq.cn/Article/details/gnmllddqz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gcxaxcury.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.fehbvm.com/Article/details/gclbadhol.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gywfjmyzd.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.fehbvm.com/Article/details/gjxnzeinl.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.zdbjq.cn/Article/details/ggyedlslw.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gpqtipsga.sHtML

[H02] finally / ensure 收尾
来源：http://mobile.fehbvm.com/Article/details/gdlsxdxih.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.hesvh.cn/Article/details/gtckwpvww.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gprfbcwgt.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gnfknoxhq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gtfjdvzfz.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gozfwjkuf.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.zdbjq.cn/Article/details/gaxjmbapi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/guugaoksp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gytywcaow.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gybizxzcb.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.zdbjq.cn/Article/details/gxfglusgg.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gbcnmjyru.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gnhelpuwi.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gmoxzvffm.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/ghnolguhe.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gyipmirtq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gnzribcje.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gdnytbybx.sHtML

[H04] 自定义异常类型
来源：http://m.share.hesvh.cn/Article/details/gghfjjpac.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/geoaqrcfp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://m.share.fehbvm.com/Article/details/gacvhmoov.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gwnhqnxsc.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gpdynwoll.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gdemdkoem.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.zdbjq.cn/Article/details/gkkxauyjx.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gexjflwlj.sHtML

C#:   class MyException : Exception {}
来源：http://wap.hesvh.cn/Article/details/gkulsuagu.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gdtanohai.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/grfnoxaza.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.share.hesvh.cn/Article/details/gvxrskzca.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gavrnrhvy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gvdahdujy.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gblbnwjny.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/gxhymuiwl.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gbmyoiuzs.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.zdbjq.cn/Article/details/gnsivlhkn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gjjwqdtjf.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gsurgskax.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gmiwcbzbl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gdgpviauo.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/ghcqvrvux.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gifleljbp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.fehbvm.com/Article/details/gcshvhlqx.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.fehbvm.com/Article/details/gbahleuuf.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gjdkqsmol.sHtML

[H07] 断言
来源：http://blog.fehbvm.com/Article/details/gjjlmemiq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/geigsynxo.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gaujorpek.sHtML

JS:   console.assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gpxlmixeq.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fehbvm.com/Article/details/gygdimvkn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.zdbjq.cn/Article/details/gevfdyhuz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.fehbvm.com/Article/details/gtoxccznm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gsqjyfnoq.sHtML


<!-- 参考信息 -->