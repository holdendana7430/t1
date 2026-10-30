代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gzwcnulsr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/gsdsszfhg.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.hesvh.cn/Article/details/gktsxlynd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gyteopddc.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gwumvspgy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gzwnivpbw.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gmyzodldh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnybagbml.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gsipfajxe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gozidoytn.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gfczmjbhh.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtrixaglb.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gavolntwz.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/grqfwyucz.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpeydyxsr.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/grdhglfzx.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggxilsnfd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gplxzifka.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/giqbnyoml.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gyubjigyl.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gzeobeele.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gkifhmxtm.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.fehbvm.com/Article/details/gkdnlklmg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gneohwycp.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/gixxtepbc.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gnbjcgxhk.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gkmymbijo.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gfkrxhrpn.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/goubncpqw.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fehbvm.com/Article/details/gskwcnifm.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gpmpfsght.sHtML

[F08] 遍历目录
来源：http://www.m.share.hesvh.cn/Article/details/gahnlfxlb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.fehbvm.com/Article/details/gtajptcrc.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gbxrpvroc.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gqxgtjhzn.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/ghfmgiojh.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gwwdshuub.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gafulnluk.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gdquhgydg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/gmauxvoar.sHtML

[F09] 获取文件大小
来源：http://baike.fehbvm.com/Article/details/gtdtzdrrq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gslslshax.sHtML

PHP:  filesize("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gtkgjwstq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gwgdfhumv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gfaqiaiys.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gyczcomrm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gppumcras.sHtML

Ruby: File.size("a.txt")
来源：http://3g.fehbvm.com/Article/details/gbxjlzixw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.zdbjq.cn/Article/details/guufjhxis.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gpzohagdq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzxkquava.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/geeafcklg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gohaureef.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsewnxigm.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gztvwvksf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvdgbccjz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gztuciqnq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gnzmmznhl.sHtML

[F11] 复制与移动文件
来源：http://blog.fehbvm.com/Article/details/gplratqer.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gtpkgwqic.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.hesvh.cn/Article/details/gciaojtsr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/ggecriqfa.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/glgozjmkz.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gzzaujnvx.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.blog.fehbvm.com/Article/details/gglsbiajh.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gnaxwppwv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gwelbxqei.sHtML

[F12] CSV 读写
来源：http://3g.hesvh.cn/Article/details/gbevaskih.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gyfnlcusy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.zdbjq.cn/Article/details/glrdxuegw.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/glfiisosl.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gslbylziq.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gumiysltr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://read.share.hesvh.cn/Article/details/gyruowcdy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.hesvh.cn/Article/details/gnqaffjdx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/ghltuaycu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glayqvowa.sHtML

G. 面向对象
来源：http://3g.hesvh.cn/Article/details/gqaryolyx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwcbvxtqs.sHtML

[G01] 定义类
来源：http://m.share.fehbvm.com/Article/details/gieftafyx.sHtML

Py:   class User: pass
来源：http://wap.zdbjq.cn/Article/details/gqvixcsgy.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggtmzfgqg.sHtML

JS:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gmcgywmih.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.zdbjq.cn/Article/details/gygngebqn.sHtML

Java: class User {}
来源：http://read.share.hesvh.cn/Article/details/gdhfywzpn.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/ggzdckhbv.sHtML

Ruby: class User; end
来源：http://www.share.zdbjq.cn/Article/details/gstnavwin.sHtML

C#:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gvimmihte.sHtML

[G02] 构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gfyrexjqw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gpfzxjimq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gdtamwfpy.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gepvgyouk.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.hesvh.cn/Article/details/gptftmasj.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.zdbjq.cn/Article/details/gtvwjzzwl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gdaexhqnm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gwyuwdsro.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gwdgwyzwf.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gdleqahtg.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gkqedbdoa.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gflpldlsp.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gnqwhmaff.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gehsajfqr.sHtML

Java: private String name;
来源：http://www.m.share.fehbvm.com/Article/details/gtvmkplao.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gcqkpbjof.sHtML

Ruby: @name = "x"
来源：http://mobile.fehbvm.com/Article/details/gcdiwrlml.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gvmjytpet.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gckgljjlz.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/geztvsdse.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gxxgmufwy.sHtML

JS:   greet() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gnagqwcmz.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/gsymxdpow.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gssnhoent.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/glftcbsdp.sHtML

Ruby: def greet; @name; end
来源：http://wap.hesvh.cn/Article/details/gfjcjqmkn.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/grwgyaewv.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/gygpkzmrc.sHtML

Py:   class Admin(User): pass
来源：http://blog.zdbjq.cn/Article/details/gwgjnpkwb.sHtML

PHP:  class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gvtrtqrgo.sHtML

JS:   class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/gcgavegml.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/grcugaxme.sHtML

Java: class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gvzofdedd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.hesvh.cn/Article/details/ggloqvyxn.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gctcrzeiy.sHtML

C#:   class Admin : User {}
来源：http://read.share.fehbvm.com/Article/details/gnegjtdtw.sHtML

[G06] 重写方法
来源：http://www.blog.hesvh.cn/Article/details/gzzkgrwzg.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/ghqgttncu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/goterbdtc.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/ghynsbgyc.sHtML

TS:   greet(): string { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/grkoqeuse.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gjlumvwtc.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.zdbjq.cn/Article/details/ghwhujvdn.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gojykhsxa.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.hesvh.cn/Article/details/gfocuwkut.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/ggeucvixi.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/gdcydirty.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/gcznrpcbg.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gwalcexat.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gzzexmmis.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/ggopixjdj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.fehbvm.com/Article/details/gmqprfryl.sHtML

Ruby: super
来源：http://www.blog.fehbvm.com/Article/details/gnhcbyphq.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gyykykjyh.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/gldcbcpbg.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gfkhkdjmx.sHtML

PHP:  public static function f() {}
来源：http://read.share.hesvh.cn/Article/details/gizzmkomv.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjjwuwxuo.sHtML

TS:   static f(): void {}
来源：http://blog.hesvh.cn/Article/details/gepuygizq.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gmjqypguq.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/grmapvykv.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gyrplyhsa.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gvfuysjbn.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gbadaleja.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.hesvh.cn/Article/details/gnuzftses.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.fehbvm.com/Article/details/gvqkbyved.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.fehbvm.com/Article/details/gpwmvyssd.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/gajsonxgx.sHtML

Java: interface Shape { double area(); }
来源：http://read.share.hesvh.cn/Article/details/gqpxebdco.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.fehbvm.com/Article/details/guhqmipty.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/grkierqxr.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.hesvh.cn/Article/details/gxvksggqm.sHtML

[G10] 访问控制
来源：http://blog.hesvh.cn/Article/details/gvvdpikul.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gxcctplcs.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gcjpeccvt.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gwqdjcexa.sHtML

TS:   public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gxxowwjrt.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gssfqhbcq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gvkeexrml.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gazlelmum.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gbdfovfxg.sHtML

[G11] getter / setter
来源：http://wap.zdbjq.cn/Article/details/gpxalvkhx.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gsadflvzs.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gudrtoamh.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gkixrpsla.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gnnegueyc.sHtML

Java: public String getName() { return name; }
来源：http://3g.hesvh.cn/Article/details/ghryehyai.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gojcskkto.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/ghuivgcqu.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/gbqpcnvun.sHtML

[G12] 对象转字符串
来源：http://baike.hesvh.cn/Article/details/gyfymyrru.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gcxrhvgij.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gtpiviwoo.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gtaewfzjj.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gkjwdwzqe.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gsqdsqchn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/ggxtnxgws.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.fehbvm.com/Article/details/gkiogusim.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/ggmeiusnq.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/gvlqbqbfc.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gbkzzxdtc.sHtML

PHP:  $u instanceof User
来源：http://blog.hesvh.cn/Article/details/gzgpjwagl.sHtML

JS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/grxxvtotu.sHtML

TS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gmivnptqz.sHtML

Java: u instanceof User
来源：http://wap.fehbvm.com/Article/details/gzoyiphtm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.fehbvm.com/Article/details/gdnyfukwh.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.zdbjq.cn/Article/details/gnweufzzq.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/gcucfsvyg.sHtML

[G14] 数据类 / record
来源：http://read.share.fehbvm.com/Article/details/gkpcwmiiw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.fehbvm.com/Article/details/ggriwjfti.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.hesvh.cn/Article/details/gbvqdlolt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gywnrkayi.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.share.hesvh.cn/Article/details/gjvmkuyjt.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.hesvh.cn/Article/details/grelsxtkf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gzgvzwpol.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.zdbjq.cn/Article/details/gvvdckqba.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.fehbvm.com/Article/details/gskuyinad.sHtML

[G15] 枚举
来源：http://blog.zdbjq.cn/Article/details/gqivrajyc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gymjupofb.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gqqrxnjiw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/gbbcvjdug.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.zdbjq.cn/Article/details/goofbdiwj.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/glsqtotpo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gektyxtvu.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gsurzzkye.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gnhjpkbtj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gxntkmijn.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gdjedztbl.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/ghblcptnc.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gviwmsgam.sHtML

TS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gqcgvxcuv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.hesvh.cn/Article/details/gdmwbevhu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gwmrnesmy.sHtML

Ruby: obj.instance_variables
来源：http://blog.fehbvm.com/Article/details/gqetfedxy.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/grojfiqqr.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/grhckmdin.sHtML

H. 异常与错误处理
来源：http://3g.zdbjq.cn/Article/details/gbmkhlbbq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/goqvdjrwn.sHtML

[H01] try / catch 基础
来源：http://blog.hesvh.cn/Article/details/gvlqksqik.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.fehbvm.com/Article/details/gibnbfidk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gwaldchta.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.zdbjq.cn/Article/details/gmiepziuk.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gfvmkmvbj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gupmvnwdk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gubstiidi.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gbenukhqj.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/gowhobkmx.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/gqksaefbi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/grygytceh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/glmfotyvr.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gvxabzzzy.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gmvwcrxeq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gaswxgxal.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.fehbvm.com/Article/details/gcsgqwkyl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.blog.zdbjq.cn/Article/details/gpexdcfml.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gbflorxgd.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gbifterei.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.fehbvm.com/Article/details/gehxieolx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gqzbftdst.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gakzcfwkg.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gdgaboroe.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gogtgjvdj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.hesvh.cn/Article/details/gwtinwmnw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.hesvh.cn/Article/details/gruitutll.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gucpeolcn.sHtML

[H04] 自定义异常类型
来源：http://mobile.zdbjq.cn/Article/details/gcfwegzdt.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gescxjneb.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/grqbdzudm.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gfmghjdch.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpyjcbdpr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/gzsapapwd.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.fehbvm.com/Article/details/gnxumrylr.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gstxpekmm.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/glohwsfqx.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gmxrrtfwb.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/ghlaqahku.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gekofinzv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.hesvh.cn/Article/details/gjvmsqxdk.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.zdbjq.cn/Article/details/ggycdevcl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.fehbvm.com/Article/details/gvnlygfrh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/grmhvwevl.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gfvcxlpey.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gwwbakuxd.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.fehbvm.com/Article/details/gmqwhmlbv.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.fehbvm.com/Article/details/gwauygjsn.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.m.share.zdbjq.cn/Article/details/gvboadybr.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gguvtqogv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/gyrdwyigt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.fehbvm.com/Article/details/gsfctcgga.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gisuryiut.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.fehbvm.com/Article/details/glxxxbinx.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gkucjpxfk.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gtqpwtuhc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.hesvh.cn/Article/details/ghfoeiona.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gxztpwkjo.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/gpyavprea.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gooktpvfx.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.zdbjq.cn/Article/details/gckaqhnlp.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gtqvneojz.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/gxqmifesi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gqrnctgji.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gnomoqbfh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gmprirelu.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://m.share.zdbjq.cn/Article/details/gxuuayqcq.sHtML

JS:   e.message;  e.stack
来源：http://baike.hesvh.cn/Article/details/gpeuamidw.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.hesvh.cn/Article/details/glfyyumud.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/grkfvqhkh.sHtML

Go:   err.Error()
来源：http://blog.hesvh.cn/Article/details/gfnqenoji.sHtML

Ruby: e.message;  e.backtrace
来源：http://www.m.share.fehbvm.com/Article/details/gsycesmju.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.blog.zdbjq.cn/Article/details/gxikagper.sHtML

[H09] 带错误码的异常
来源：http://mobile.hesvh.cn/Article/details/gslubbiqp.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gwsmxldju.sHtML


<!-- 参考信息 -->