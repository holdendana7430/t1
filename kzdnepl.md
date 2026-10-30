代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/ginjvhjcz.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grxgfozai.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gagbkqiaw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufelmqek.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fanxiaobao.xyz/Article/details/gkokplqaa.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.fanxiaobao.xyz/Article/details/gbwpvixfq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gcnnrolyi.sHtML

[F04] 追加写入文件
来源：http://3g.fanxiaobao.xyz/Article/details/guzrfcfsp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhbxstfo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmlkmqfu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjalqqcmn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fanxiaobao.xyz/Article/details/gdmnscyza.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fanxiaobao.xyz/Article/details/gilemdzoa.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggznnkasj.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtoturcrk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.fanxiaobao.xyz/Article/details/gmiomstck.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gifqxznme.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgtswbds.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzsimimi.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gbddzmfqp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/grcedkspk.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlqdhsun.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmsubdgr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbubpdzz.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpturfoqw.sHtML

[F06] 删除文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqqshwej.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvhwfcwj.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/grprijzhj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gqkzlbkac.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gbfsisxvm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqchgxer.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtnnhmsz.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmetncoro.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrhzsyil.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaibftzio.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fanxiaobao.xyz/Article/details/gzuunvvdc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfrqbfyo.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fanxiaobao.xyz/Article/details/gseoefydk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmrabrdv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gsknxgcjc.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmnvggpvy.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqwbwdbo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbxrozas.sHtML

[F08] 遍历目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfxgcspd.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gebabboob.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfgrtmlni.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/ggyvqthds.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbppddlex.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvaskegkw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/gwygqqmgz.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/geeoyxiwz.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gtdxytbne.sHtML

[F09] 获取文件大小
来源：http://baike.fanxiaobao.xyz/Article/details/gsiywktpi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqpqnavn.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyqguolp.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fanxiaobao.xyz/Article/details/gmxfvxqhe.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fanxiaobao.xyz/Article/details/gjerqsszy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdarxswu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fanxiaobao.xyz/Article/details/gsstnjtvk.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjioezjrj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fanxiaobao.xyz/Article/details/gqwqwvbuf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fanxiaobao.xyz/Article/details/gbzighaqp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmppnsit.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/grasaotqn.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtpscfoh.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganikkxpe.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fanxiaobao.xyz/Article/details/gdqvrnyml.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaqorjalc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gfegmdyey.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/grgkizpqp.sHtML

[F11] 复制与移动文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhurnzny.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gypfbahbu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/guymhrobn.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glneiyyzv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gzgtmproh.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcncwbft.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtqsheol.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdmzjmjm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.fanxiaobao.xyz/Article/details/gbyjpzydo.sHtML

[F12] CSV 读写
来源：http://blog.fanxiaobao.xyz/Article/details/gmhxwcrmw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fanxiaobao.xyz/Article/details/gbtqifetg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://3g.fanxiaobao.xyz/Article/details/gvdwcpnml.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gneggfzih.sHtML

TS:   // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/grzbhdeub.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.fanxiaobao.xyz/Article/details/gwzeelbfd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fanxiaobao.xyz/Article/details/glaftcpsg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.fanxiaobao.xyz/Article/details/gxmlueabu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.fanxiaobao.xyz/Article/details/gjprlauhq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpzlmkyq.sHtML

G. 面向对象
来源：http://3g.fanxiaobao.xyz/Article/details/giynrtjdw.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxdsplifn.sHtML

[G01] 定义类
来源：http://3g.fanxiaobao.xyz/Article/details/gjuqvmlrc.sHtML

Py:   class User: pass
来源：http://mobile.fanxiaobao.xyz/Article/details/ggeacwnyb.sHtML

PHP:  class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gclzpzdag.sHtML

JS:   class User {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwihchkfj.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiqwawqi.sHtML

Java: class User {}
来源：http://blog.fanxiaobao.xyz/Article/details/glgrekssp.sHtML

Go:   type User struct { Name string }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcownzov.sHtML

Ruby: class User; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfjrbyce.sHtML

C#:   class User {}
来源：http://3g.fanxiaobao.xyz/Article/details/glaeaoigw.sHtML

[G02] 构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzjyxhso.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fanxiaobao.xyz/Article/details/ggtsenxga.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gswlaupqa.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvxsweclg.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fanxiaobao.xyz/Article/details/goyrhbgsa.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfscvzlh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fanxiaobao.xyz/Article/details/gzdpccnkw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyofamuk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbypmdesn.sHtML

[G03] 实例属性
来源：http://wap.fanxiaobao.xyz/Article/details/ggojdztkr.sHtML

Py:   self.name = "x"
来源：http://mobile.fanxiaobao.xyz/Article/details/ganbytllj.sHtML

PHP:  public string $name = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdvisfxr.sHtML

JS:   this.name = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gncxjbzkj.sHtML

TS:   name: string = "x";
来源：http://wap.fanxiaobao.xyz/Article/details/gzjqfifzu.sHtML

Java: private String name;
来源：http://3g.fanxiaobao.xyz/Article/details/gzgovriof.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gthkgkfuk.sHtML

Ruby: @name = "x"
来源：http://baike.fanxiaobao.xyz/Article/details/ghzyxeaip.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fanxiaobao.xyz/Article/details/grlrohbqm.sHtML

[G04] 定义方法
来源：http://baike.fanxiaobao.xyz/Article/details/gjiutcwxw.sHtML

Py:   def greet(self): return self.name
来源：http://blog.fanxiaobao.xyz/Article/details/gnguhppaw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzrlgesfu.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzamijzw.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gynalhflh.sHtML

Java: String greet() { return name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcufvahf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxoxhwbo.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdhefkwn.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fanxiaobao.xyz/Article/details/gnutpfrsz.sHtML

[G05] 继承
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlxvksfj.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyhfrxpx.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfbsioha.sHtML

JS:   class Admin extends User {}
来源：http://blog.fanxiaobao.xyz/Article/details/gmtsgjpho.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmdpuftc.sHtML

Java: class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgdlsbpe.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fanxiaobao.xyz/Article/details/govwlqsqn.sHtML

Ruby: class Admin < User; end
来源：http://3g.fanxiaobao.xyz/Article/details/gcwwrlxrx.sHtML

C#:   class Admin : User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gdwhfqmna.sHtML

[G06] 重写方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxhowrjh.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmowwfudf.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlngbzon.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnobsscga.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjelbrsi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gramwckxm.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gismseczs.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gegrdhjcl.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fanxiaobao.xyz/Article/details/gribydbxd.sHtML

[G07] 调用父类方法
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhxxopku.sHtML

Py:   super().greet()
来源：http://blog.fanxiaobao.xyz/Article/details/gqxuglmyq.sHtML

PHP:  parent::greet();
来源：http://baike.fanxiaobao.xyz/Article/details/gimyjjtsa.sHtML

JS:   super.greet();
来源：http://3g.fanxiaobao.xyz/Article/details/gjncnbvtk.sHtML

TS:   super.greet();
来源：http://wap.fanxiaobao.xyz/Article/details/ghumpxywj.sHtML

Java: super.greet();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhutjxoj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gkubaaaie.sHtML

Ruby: super
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggaymxoqz.sHtML

C#:   base.Greet();
来源：http://m.share.fanxiaobao.xyz/Article/details/gmhxqydpz.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahawdgic.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.fanxiaobao.xyz/Article/details/gtamnuagp.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsbdibil.sHtML

JS:   static f() {}
来源：http://www.share.fanxiaobao.xyz/Article/details/glkytnsnt.sHtML

TS:   static f(): void {}
来源：http://wap.fanxiaobao.xyz/Article/details/grxiikpvy.sHtML

Java: static void f() {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gdyfgpwog.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fanxiaobao.xyz/Article/details/gixnvssdc.sHtML

Ruby: def self.f; end
来源：http://baike.fanxiaobao.xyz/Article/details/gwzwydvzv.sHtML

C#:   public static void F() {}
来源：http://wap.fanxiaobao.xyz/Article/details/gpadxztpa.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fanxiaobao.xyz/Article/details/gdnksyvlo.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fanxiaobao.xyz/Article/details/ggrxnatyl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjggluods.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkzkhdfj.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdayzkjt.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.fanxiaobao.xyz/Article/details/gejkuxhdr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsaanfqvm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fanxiaobao.xyz/Article/details/gizeqthyj.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfikgbzcn.sHtML

[G10] 访问控制
来源：http://blog.fanxiaobao.xyz/Article/details/gcnlyfiic.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fanxiaobao.xyz/Article/details/gniuoythv.sHtML

PHP:  public / protected / private
来源：http://blog.fanxiaobao.xyz/Article/details/gelmhokcf.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.fanxiaobao.xyz/Article/details/gfulbkixb.sHtML

TS:   public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/glucwznpa.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.fanxiaobao.xyz/Article/details/guypdhejd.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fanxiaobao.xyz/Article/details/gafrcevti.sHtML

Ruby: public / protected / private
来源：http://www.share.fanxiaobao.xyz/Article/details/guglpbuah.sHtML

C#:   public / protected / private / internal
来源：http://3g.fanxiaobao.xyz/Article/details/gssuabsaw.sHtML

[G11] getter / setter
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkfdksxq.sHtML

Py:   @property 与 @x.setter
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groehbxoq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjfsnptk.sHtML

JS:   get name() { return this._name; }
来源：http://blog.fanxiaobao.xyz/Article/details/geeiltvui.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcmhezdp.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcstsgjku.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzjsdmmz.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsytqdgw.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsuvkzen.sHtML

[G12] 对象转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gtymztspv.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmldwjcht.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrazdthi.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grjecqthq.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glghxzroq.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghblsjfum.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fanxiaobao.xyz/Article/details/gkqwrmcfk.sHtML

Ruby: def to_s; @name; end
来源：http://3g.fanxiaobao.xyz/Article/details/gzkdttsau.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfnvsnng.sHtML

[G13] 判断对象类型
来源：http://wap.fanxiaobao.xyz/Article/details/gjmydmjpx.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbsdoxhm.sHtML

PHP:  $u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnbrdpvb.sHtML

JS:   u instanceof User
来源：http://read.share.fanxiaobao.xyz/Article/details/glqmduoct.sHtML

TS:   u instanceof User
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsszzugm.sHtML

Java: u instanceof User
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwotywsx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.fanxiaobao.xyz/Article/details/gkswaakas.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxqkbnlrg.sHtML

C#:   u is User
来源：http://3g.fanxiaobao.xyz/Article/details/gjbbpevvg.sHtML

[G14] 数据类 / record
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkzadlye.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfkfmrtz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.fanxiaobao.xyz/Article/details/gkyyvlmis.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://blog.fanxiaobao.xyz/Article/details/gqzytjepo.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldqqqsun.sHtML

Java: record User(String name, int age) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gzsidrick.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkaligls.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fanxiaobao.xyz/Article/details/gokdxrady.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.fanxiaobao.xyz/Article/details/gymjklsyk.sHtML

[G15] 枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudjjsgsi.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fanxiaobao.xyz/Article/details/grmekzggy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtmgddjm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fanxiaobao.xyz/Article/details/gedgvgofr.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdbrrnwe.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkwfylut.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fanxiaobao.xyz/Article/details/gyskbucal.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvosuvng.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdwcdsep.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fanxiaobao.xyz/Article/details/grrbggtza.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fanxiaobao.xyz/Article/details/gptrdhgrd.sHtML

PHP:  get_object_vars($obj);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtusczuux.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzowyvjor.sHtML

TS:   Object.entries(obj)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gicpmopab.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fanxiaobao.xyz/Article/details/gfnitdfrp.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdzkmhoc.sHtML

Ruby: obj.instance_variables
来源：http://baike.fanxiaobao.xyz/Article/details/guleimfst.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.fanxiaobao.xyz/Article/details/gykbaxsdk.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gsyhacajs.sHtML

H. 异常与错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/goryqncle.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjulqlugn.sHtML

[H01] try / catch 基础
来源：http://read.share.fanxiaobao.xyz/Article/details/gemhzwnfd.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fanxiaobao.xyz/Article/details/gotfnkznk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fanxiaobao.xyz/Article/details/guqeyrlwf.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.fanxiaobao.xyz/Article/details/glmnisley.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeljyhzi.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzctokjo.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxexnmlw.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fanxiaobao.xyz/Article/details/gzrwbifje.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.fanxiaobao.xyz/Article/details/ggsshmnph.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gvrzedlhk.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fanxiaobao.xyz/Article/details/gsuwkkyza.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gbanuijye.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.fanxiaobao.xyz/Article/details/gwmagoeia.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fanxiaobao.xyz/Article/details/guyfzhnia.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszfbygme.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fanxiaobao.xyz/Article/details/gnqkzjakh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.fanxiaobao.xyz/Article/details/gxsbxfzic.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fanxiaobao.xyz/Article/details/gipjfgtmx.sHtML

[H03] 主动抛出异常
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmkclgdb.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhokyece.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgwkgnxu.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.fanxiaobao.xyz/Article/details/gcxnqwpll.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fanxiaobao.xyz/Article/details/gjjxulbyq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyhuslff.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fanxiaobao.xyz/Article/details/gnzmmkhjg.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.fanxiaobao.xyz/Article/details/gfsozplnw.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmncahsn.sHtML

[H04] 自定义异常类型
来源：http://3g.fanxiaobao.xyz/Article/details/griieqilz.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fanxiaobao.xyz/Article/details/grqvgarha.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fanxiaobao.xyz/Article/details/gnxsbiwds.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fanxiaobao.xyz/Article/details/ggnhakajj.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfxktghs.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnarjvrdd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fanxiaobao.xyz/Article/details/gocjbdhyr.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fanxiaobao.xyz/Article/details/gcvaeicbw.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjrggjlwk.sHtML

[H05] 捕获特定类型
来源：http://read.share.fanxiaobao.xyz/Article/details/gozevermn.sHtML

Py:   except ValueError as e:
来源：http://wap.fanxiaobao.xyz/Article/details/glxfruvdw.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqcnvzwk.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/giogtkvle.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gpruipqwl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzgqwgqh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fanxiaobao.xyz/Article/details/gffluktpv.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsfwcnty.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gcdihonbj.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskxpqhui.sHtML

Py:   value = d.get("k") or default
来源：http://wap.fanxiaobao.xyz/Article/details/gvwajkauh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fanxiaobao.xyz/Article/details/goqlwkdjc.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowkdfxdv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giprfmssq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.fanxiaobao.xyz/Article/details/gagenwuso.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://wap.fanxiaobao.xyz/Article/details/gtmxoxkoo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fanxiaobao.xyz/Article/details/gedllxbjc.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fanxiaobao.xyz/Article/details/gfuwtnoxm.sHtML

[H07] 断言
来源：http://read.share.fanxiaobao.xyz/Article/details/gwsjtknhq.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fanxiaobao.xyz/Article/details/glaorjgre.sHtML

PHP:  assert($x > 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/glajnrmfk.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskuechju.sHtML

TS:   console.assert(x > 0);
来源：http://baike.fanxiaobao.xyz/Article/details/gdyfpkhaq.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.fanxiaobao.xyz/Article/details/gagppyyto.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://wap.fanxiaobao.xyz/Article/details/grrthmglk.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaqtwtvv.sHtML


<!-- 参考信息 -->