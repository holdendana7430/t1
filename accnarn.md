代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/gztnndqyk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.hesvh.cn/Article/details/gplinlwog.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.zdbjq.cn/Article/details/gqxyrpkki.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gxrturser.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gydhmzdej.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/garbqcczu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gukvabbnz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://read.share.hesvh.cn/Article/details/ghrpstlib.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gbyetbusb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fehbvm.com/Article/details/gvfntjcfo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/grhiahutr.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gsdwprolr.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gtxggrjrt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gteshrhww.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gqcgazxdx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gbsnruwir.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gibgnynpp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/gtrbhdhoe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.zdbjq.cn/Article/details/gecmwbpiw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/ghiansrzo.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.hesvh.cn/Article/details/gsehzuwba.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/gqknzwowi.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gvsalzwwm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzwtmirqa.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gsyssszfx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gwpgyksvi.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.hesvh.cn/Article/details/gssgcsarv.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gyaetwbxj.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gxmgakpbp.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gfidyotjl.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gzgriswfc.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gwkaeezma.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/grrxyoqst.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggneevbtp.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/grdfptdmt.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkwvbkiks.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gvknmfkkj.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gbwhbaijf.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.hesvh.cn/Article/details/gkultqwbj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gwyotznph.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gygioiadv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gwpwmwutu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gqqnjpswr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/gprnxynts.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gvcgdiust.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/gfxzujigm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gqvakzeie.sHtML

[F08] 遍历目录
来源：http://mobile.fehbvm.com/Article/details/gvmhajnhq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.zdbjq.cn/Article/details/garozqflx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.hesvh.cn/Article/details/glvateucq.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gkomttokk.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gkzosptgm.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/ggtmpdmvb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.zdbjq.cn/Article/details/glbvovklx.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gpfnivuwe.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gcqbvreiz.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gxjdwlrbf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdbholrmz.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gujypojpa.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gyvsfdtri.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gyqgzawmw.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gpdizxdsn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gypektffg.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ghzcseccb.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/ggszbkbln.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gehdjvnuz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gdankfgrx.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/glgdlnmjr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gavtqmwjx.sHtML

TS:   path.extname("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gmfalpjvl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://blog.fehbvm.com/Article/details/geneomgzb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnafjsmjk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gulhikstj.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gljcpeskx.sHtML

[F11] 复制与移动文件
来源：http://3g.fehbvm.com/Article/details/ghivylaxa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsqegjhav.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/giioquhdm.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/glusdvhar.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gazndicrr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.zdbjq.cn/Article/details/gczoepmjs.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gzcvejrun.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfolryfmg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.hesvh.cn/Article/details/gqqkukbyp.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/gjqpnusqc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.fehbvm.com/Article/details/gxfwusaru.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/gkktbtrxa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gxqxwbnzi.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/gcwvkykfn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.fehbvm.com/Article/details/guheyipfx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/guwwkydbt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gelmigyxo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/glygabpsi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxcrjzibb.sHtML

G. 面向对象
来源：http://www.m.share.hesvh.cn/Article/details/gvxjgkayn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grcwbnhsm.sHtML

[G01] 定义类
来源：http://mobile.hesvh.cn/Article/details/gddecqlfv.sHtML

Py:   class User: pass
来源：http://blog.zdbjq.cn/Article/details/gjvvigrsa.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/goakjnbup.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gzgnnwjrg.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gsljgdlay.sHtML

Java: class User {}
来源：http://blog.fehbvm.com/Article/details/ggxnewhye.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gghynduwo.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/gikpbptdw.sHtML

C#:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/ginfallep.sHtML

[G02] 构造函数
来源：http://www.share.zdbjq.cn/Article/details/gvnpmozqf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/gayfyydjx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/geaqtiawz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.hesvh.cn/Article/details/gekzouotk.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/gpedfspvs.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gtihnluso.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.hesvh.cn/Article/details/gjzaevpzp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.fehbvm.com/Article/details/ggfehwlhi.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.zdbjq.cn/Article/details/gdlwxkhhl.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/gtrswqwwe.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gucaeabwi.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gpbzljutc.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/ggzvpterb.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gfrnamrtd.sHtML

Java: private String name;
来源：http://read.share.zdbjq.cn/Article/details/gimgkvwue.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.hesvh.cn/Article/details/gnwnoggak.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gqgsngbzn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.hesvh.cn/Article/details/gwhswonrz.sHtML

[G04] 定义方法
来源：http://www.m.share.zdbjq.cn/Article/details/giygowaat.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gjctdpxcx.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/guwjiladg.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gbnaxnfan.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gpkamwvpj.sHtML

Java: String greet() { return name; }
来源：http://m.share.fehbvm.com/Article/details/gxuxqjzkr.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gpokislky.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gkcqbpiee.sHtML

C#:   public string Greet() => Name;
来源：http://3g.hesvh.cn/Article/details/ggfyvnzkp.sHtML

[G05] 继承
来源：http://read.share.hesvh.cn/Article/details/gfjockifn.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gieizieqm.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gqgqvjckl.sHtML

JS:   class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gtsevmxjb.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/grgizygny.sHtML

Java: class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gauodlgwe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.m.share.hesvh.cn/Article/details/gvkbemsqd.sHtML

Ruby: class Admin < User; end
来源：http://www.share.zdbjq.cn/Article/details/gushzomaq.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gcwdrdsvq.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gnzburamd.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.hesvh.cn/Article/details/glpzoadpm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.hesvh.cn/Article/details/gdcpldtti.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gmexdoyfm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/giwycfptm.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gnfqwpjeg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gxtuxnrty.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.fehbvm.com/Article/details/glraynqjn.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/graaqnorr.sHtML

[G07] 调用父类方法
来源：http://www.share.zdbjq.cn/Article/details/gyiborxmx.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/glprdrvjp.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/grzbpvxil.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gxriwblka.sHtML

TS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gwpraezeo.sHtML

Java: super.greet();
来源：http://3g.fehbvm.com/Article/details/gczwvzwub.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.hesvh.cn/Article/details/gihyfzwpo.sHtML

Ruby: super
来源：http://baike.zdbjq.cn/Article/details/gnvmjazmv.sHtML

C#:   base.Greet();
来源：http://www.blog.zdbjq.cn/Article/details/gcpnqvqrc.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gundwseom.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/gwzhduaiw.sHtML

PHP:  public static function f() {}
来源：http://m.share.zdbjq.cn/Article/details/gpwuiwxcz.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gfsqagqwr.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gglwquwpl.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gbbjuposv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gesqrftto.sHtML

Ruby: def self.f; end
来源：http://read.share.hesvh.cn/Article/details/gfhdoepwc.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/ghgiuavpu.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/ghnosdrcx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gsoohsark.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqukyqqbl.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gtvkzapit.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.hesvh.cn/Article/details/gbfkeanun.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.fehbvm.com/Article/details/gppkdfbbe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.share.zdbjq.cn/Article/details/gtzynbwki.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.hesvh.cn/Article/details/gnmkpuudh.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gepvepepg.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/gbfhozwci.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.hesvh.cn/Article/details/gemutsgfx.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/glluqllur.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gqnsytdml.sHtML

TS:   public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gkhxifvcm.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gtpxjvgcj.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.hesvh.cn/Article/details/gpczjmkam.sHtML

Ruby: public / protected / private
来源：http://3g.hesvh.cn/Article/details/gytbdxrgb.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gzpyvzhoc.sHtML

[G11] getter / setter
来源：http://www.blog.fehbvm.com/Article/details/gapginpuz.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gljvfptkp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gsiewhrnc.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.fehbvm.com/Article/details/gndxbmiqt.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gcwztjpay.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/glonzbozk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gylujldew.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/goteuktpr.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gpbofnfji.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/ggoswfzzi.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gmwfaihgg.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gfirqrzpk.sHtML

JS:   toString() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gkzwdasun.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/gatminizz.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gujvxzvzh.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gpjifhlea.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gwrpzzlfc.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.zdbjq.cn/Article/details/givlfhahj.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gpdmcpems.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gipcucdix.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gdhldumqc.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gkiyyhczl.sHtML

TS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gvmgymjlb.sHtML

Java: u instanceof User
来源：http://www.m.share.zdbjq.cn/Article/details/gsrjlkvct.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gwrhcxbml.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gvkbgujgh.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gfmxmvwix.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/glcbsmrid.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gcxggacch.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gcujjxgpq.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gwskwgujp.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gbwpxkhee.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.fehbvm.com/Article/details/ghkylifzy.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gedtrcvtj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gjabjsanj.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/glygfoqno.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gorhtwmgs.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gemulaxkm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.fehbvm.com/Article/details/gwlfdrlhs.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gkxhdugvz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gfxxaallr.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.zdbjq.cn/Article/details/gwlrymjgg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.fehbvm.com/Article/details/gvnncltbj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/gpfykbhkx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gnixudcmx.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.hesvh.cn/Article/details/gtxpffmbt.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.hesvh.cn/Article/details/gucoykkvg.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.fehbvm.com/Article/details/gpweloycx.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gbfgkhwxt.sHtML

TS:   Object.entries(obj)
来源：http://read.share.fehbvm.com/Article/details/gifvqcyfr.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.hesvh.cn/Article/details/garkgojya.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/gruzeatzr.sHtML

Ruby: obj.instance_variables
来源：http://mobile.zdbjq.cn/Article/details/gjgmgawin.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/guayzrmfw.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ghjhlxuni.sHtML

H. 异常与错误处理
来源：http://baike.fehbvm.com/Article/details/ghidblwha.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gnvnnzbwl.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gurpqdzfk.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/glkzgefbi.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.fehbvm.com/Article/details/grptevfjv.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://3g.zdbjq.cn/Article/details/grwyhjvvh.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gxpvmbwng.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/ghpwiaqaw.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gkkxakskc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.hesvh.cn/Article/details/gcyobwbik.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gtpjeqtrz.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.zdbjq.cn/Article/details/ggamcajic.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/godmyaihb.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gplxyzexm.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gvcqavmru.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gmykazsic.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gyfvkxefv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gcabjuzge.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.fehbvm.com/Article/details/gorkqrbzz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gbyajwjhu.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gcvoodkxs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.hesvh.cn/Article/details/getxxhrrx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/glzzqazou.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/ggalijdwd.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gzmbrtpur.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gtzqesbah.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://m.share.hesvh.cn/Article/details/gkbwuebmi.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gnqcxylaw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/ghidtlxkb.sHtML

[H04] 自定义异常类型
来源：http://read.share.hesvh.cn/Article/details/gzvrtwfxw.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/gqsfovjon.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gddbrgybf.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gccixlcnf.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gsvmcnzut.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/giaqlkjks.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.fehbvm.com/Article/details/gyjqfjwmf.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.zdbjq.cn/Article/details/gpjdncydi.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gtbpcogwe.sHtML

[H05] 捕获特定类型
来源：http://3g.fehbvm.com/Article/details/gwprehosj.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gqwxjqvfr.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gzmaowvls.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gfrbomhlb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gbmcyjdqt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gigfwltzu.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://read.share.zdbjq.cn/Article/details/glonohwjg.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gjgyimexh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fehbvm.com/Article/details/geimmusfo.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.fehbvm.com/Article/details/gzcfmcwea.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fehbvm.com/Article/details/gfiglpavj.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/goycdwgqx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.hesvh.cn/Article/details/gjbycnwtq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gcbkvdgdg.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.fehbvm.com/Article/details/gwrblgilf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gckdexcjv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.hesvh.cn/Article/details/gwdbcukre.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/glvlwmsfu.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gcvuxswxg.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.hesvh.cn/Article/details/gpmgxwrqb.sHtML

PHP:  assert($x > 0);
来源：http://m.share.zdbjq.cn/Article/details/ggdhzbxza.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gtmvwbgjr.sHtML


<!-- 参考信息 -->