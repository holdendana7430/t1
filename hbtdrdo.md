代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://m.share.fehbvm.com/Article/details/gflgnlgrv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.hesvh.cn/Article/details/gdmgvelvf.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gnwupdosu.sHtML

[F04] 追加写入文件
来源：http://blog.hesvh.cn/Article/details/gmssbumdt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/galaeccai.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gnapjiwgh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gbuxopvor.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gvsmuuwsv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gdscillds.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.zdbjq.cn/Article/details/ghkepcqof.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gplzeinsz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gsdmijyur.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.hesvh.cn/Article/details/guzzxpbkz.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gpxdmjrbu.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gzgrkcxwn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gooyzmvxk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdmcavcyg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gqnhfkbmb.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/giutrunxr.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gakvrwgjc.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gamlkumab.sHtML

[F06] 删除文件
来源：http://blog.zdbjq.cn/Article/details/gmzayeoqq.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnprfbvzo.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gktyrtqsv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/ghrpfipql.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpemortnk.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gygtrrtug.sHtML

Go:   os.Remove("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfclxpmlz.sHtML

Ruby: File.delete("a.txt")
来源：http://wap.hesvh.cn/Article/details/gfrgmpvyi.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gszyhfkgh.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gaerqfjob.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gpstdiyyf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/guloolxrk.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gwmpsobcw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/ghohboytd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gcpmcpjah.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gmwdpfwoo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gigrthcee.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gczlduoag.sHtML

[F08] 遍历目录
来源：http://3g.fehbvm.com/Article/details/gmvzgqwjx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gzqyfiwko.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gmynepjhe.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/ghzuqqrlb.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gfjqgowmw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.zdbjq.cn/Article/details/ghecysqht.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.fehbvm.com/Article/details/gqhlfaqjl.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.zdbjq.cn/Article/details/gdyraajmi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gvojweqyo.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gnwlcxpcb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.hesvh.cn/Article/details/gxhuwewmb.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gutobaxhx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gmjxamgjw.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gcuqwbfmj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gljxqcthm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/grsoasvtv.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gnawyxyau.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.hesvh.cn/Article/details/gssuqjglb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.fehbvm.com/Article/details/gyhfqtbda.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gsrigaeuc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gbbdrlemz.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbganvpmo.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gowkzsoxp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gqqduhpvt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwfsfrifv.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmiceiebc.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gihiwvsfg.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gpqgyfoxg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/guksbaxke.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gilhwaujl.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fehbvm.com/Article/details/gpdkvicee.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gocifhfua.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gwimepeuj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gnbjkuoqt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gtqpyuujg.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gkxbtowhw.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/gslwsrugc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.hesvh.cn/Article/details/ghgpxiccu.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.hesvh.cn/Article/details/gkyicluva.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gamimlcpv.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gewsexsqv.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.zdbjq.cn/Article/details/gcajqosct.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/grvncllyq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.zdbjq.cn/Article/details/gyonazgpf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.zdbjq.cn/Article/details/gigaizakl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gewsyezkg.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/gptkuvxak.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtzqnttdf.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gfkhhywke.sHtML

Py:   class User: pass
来源：http://baike.fehbvm.com/Article/details/gxsbvqsgx.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gyjidinoe.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gqfmizinz.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.fehbvm.com/Article/details/gzswaunaa.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gggwinqtb.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gwvjenqvt.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gkdppypob.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/ggxwbhdmw.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/govzktcyx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/glglwusdx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gkmdrijhq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gkbugrqqm.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.fehbvm.com/Article/details/gtldlnqyc.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gmprbbuzg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.zdbjq.cn/Article/details/gasynzdsg.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.fehbvm.com/Article/details/gcaacndqa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.hesvh.cn/Article/details/gtztfxydo.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/gwjvylzcf.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gasflekls.sHtML

PHP:  public string $name = "x";
来源：http://baike.hesvh.cn/Article/details/gvkdraztv.sHtML

JS:   this.name = "x";
来源：http://read.share.fehbvm.com/Article/details/gudzgafpv.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/getzloaoe.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gblrvmgxp.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.hesvh.cn/Article/details/glxqagien.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/gyqquyqdv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.zdbjq.cn/Article/details/gpxlgfnyz.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gzrepwpsk.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/glzyozolf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gqepomytt.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gvbidlanm.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gczbdqtoa.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gvujimvmf.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gcyrmalcj.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gdmdvqjkl.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gnlknkanb.sHtML

[G05] 继承
来源：http://www.m.share.fehbvm.com/Article/details/gcyetzdhe.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.fehbvm.com/Article/details/ghwagaaem.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gaydbygyv.sHtML

JS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/grljhgufl.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gnijoldcs.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gzosidagn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.fehbvm.com/Article/details/glaveilhq.sHtML

Ruby: class Admin < User; end
来源：http://blog.zdbjq.cn/Article/details/ghrivpluc.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/giyhebzmy.sHtML

[G06] 重写方法
来源：http://wap.hesvh.cn/Article/details/gpxlwappm.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.hesvh.cn/Article/details/gypuyapqh.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gejojdxib.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/grradnkrz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.hesvh.cn/Article/details/geepqulgv.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gzxpqqlfe.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/graloyjpb.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gkaqmwcrr.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.zdbjq.cn/Article/details/guwjoeauj.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gkbngevcr.sHtML

Py:   super().greet()
来源：http://www.m.share.fehbvm.com/Article/details/gkbfrotig.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gyftrsfji.sHtML

JS:   super.greet();
来源：http://blog.fehbvm.com/Article/details/grohfomju.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gljcejfrv.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gbioftski.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gecwxwatv.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gsqizsayv.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gejbwebod.sHtML

[G08] 静态方法与属性
来源：http://wap.fehbvm.com/Article/details/giknjrvlm.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.zdbjq.cn/Article/details/gteccwdag.sHtML

PHP:  public static function f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gkikvsgdp.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/glhjvoeft.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/ghddhqtqh.sHtML

Java: static void f() {}
来源：http://read.share.fehbvm.com/Article/details/gtmrbdjtv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gjszkltad.sHtML

Ruby: def self.f; end
来源：http://www.blog.fehbvm.com/Article/details/gdnkjqkti.sHtML

C#:   public static void F() {}
来源：http://www.m.share.fehbvm.com/Article/details/gmuvsldib.sHtML

[G09] 接口 / 抽象类
来源：http://www.blog.zdbjq.cn/Article/details/gmkyabhgq.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/gjhklhujy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gtellspqv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gzsnxevma.sHtML

TS:   interface Shape { area(): number; }
来源：http://3g.fehbvm.com/Article/details/goeafumgt.sHtML

Java: interface Shape { double area(); }
来源：http://3g.hesvh.cn/Article/details/gnlijlrdr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.hesvh.cn/Article/details/gelhtpgce.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gzagoxofa.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gcoenzagp.sHtML

[G10] 访问控制
来源：http://blog.fehbvm.com/Article/details/ggorbjpcy.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gmvelajuq.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gkfnmevyb.sHtML

JS:   #private 字段；其余公开
来源：http://www.share.hesvh.cn/Article/details/gwzjyryqq.sHtML

TS:   public / protected / private
来源：http://www.m.share.fehbvm.com/Article/details/gcwrelilr.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gkqyozlvg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gvqczybco.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gnwkikole.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gwzdyowkd.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/gmnknajgd.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/gcfqplxvy.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gocoeyrmy.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/gcdakdauj.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gvlmahjfr.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzcjtbfwv.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.hesvh.cn/Article/details/gleogavqx.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/gchggaqrk.sHtML

C#:   public string Name { get; set; }
来源：http://3g.fehbvm.com/Article/details/groczytgr.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gvqrgdulc.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gzmulnkgh.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gapxlgxal.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/gxgcllfgi.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gpbirivhx.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gslnqvuup.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gquojpfpp.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gahfzldld.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gtbxteptp.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gqcuxqmmc.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/grktbcvpv.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gvznyzqbo.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gjcghhnyg.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/ggzdwhvco.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/grsuhwxkz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.fehbvm.com/Article/details/gjzpayvbb.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gjeoiqrpw.sHtML

C#:   u is User
来源：http://mobile.fehbvm.com/Article/details/gcshrjjlh.sHtML

[G14] 数据类 / record
来源：http://www.blog.fehbvm.com/Article/details/gnqanokxg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.blog.hesvh.cn/Article/details/geoznfxec.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.zdbjq.cn/Article/details/gsxdtjoht.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.hesvh.cn/Article/details/gerxvkikm.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/glxqnfgin.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gagsdglok.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.fehbvm.com/Article/details/gafmrbdbx.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.zdbjq.cn/Article/details/ggqcgnvyx.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.fehbvm.com/Article/details/ghjikzwmn.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gnwdgoxsv.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gisvitkgk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gwvalmvno.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.zdbjq.cn/Article/details/gzucjcpau.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gdnzpetea.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.m.share.hesvh.cn/Article/details/giknfough.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.hesvh.cn/Article/details/gcdtesocy.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/glstqhvuv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gckkpsean.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.zdbjq.cn/Article/details/gmkqikyas.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gxlloucge.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.zdbjq.cn/Article/details/gqfonezqd.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/glzjtljph.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gxfxksfmf.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.fehbvm.com/Article/details/gnanpjvfk.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/glnlzovdc.sHtML

Ruby: obj.instance_variables
来源：http://mobile.fehbvm.com/Article/details/gslwonsvm.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/glpsbhuph.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzziqzcio.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gvobceyhv.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gcmulpjbu.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/ghbewsylu.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://wap.zdbjq.cn/Article/details/gnnohcllw.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/gusxvlqdq.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gaougmdlp.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gmtjalixd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.m.share.hesvh.cn/Article/details/gkgnwssui.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/ghtdyssvu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gknwflqxf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gqgcbuovg.sHtML

[H02] finally / ensure 收尾
来源：http://baike.zdbjq.cn/Article/details/glwbjlcig.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.fehbvm.com/Article/details/gssyuzstr.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gsvwyfjcw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gnevzwmqo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/grzvjtvrv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gnminahdz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/ghaqcjvyo.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.fehbvm.com/Article/details/gbqmcfsrs.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gvblluwih.sHtML

[H03] 主动抛出异常
来源：http://mobile.fehbvm.com/Article/details/gilpqvlzo.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gukvizdkv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gzhcqrwvz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gotdpgdme.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gqzfffzlz.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gaemcizyw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gdlslvphv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.zdbjq.cn/Article/details/gxrjxvyns.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gidkygrny.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/ghdvumenk.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.fehbvm.com/Article/details/grmenuliq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gzghrcgbz.sHtML

JS:   class MyError extends Error {}
来源：http://baike.fehbvm.com/Article/details/gwcbdwsyu.sHtML

TS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/gndoildnr.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/ggeqjjtsa.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gvgxlfnog.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gqyuwnyve.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gdenhfran.sHtML

[H05] 捕获特定类型
来源：http://m.share.zdbjq.cn/Article/details/gigsflmsx.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gacwcnidb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gqkauwfqm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gberisnpq.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.m.share.fehbvm.com/Article/details/gutdxxwbh.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gvexyegjy.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.zdbjq.cn/Article/details/gsowucgiz.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/ggfmwpjkr.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gdgbxcmgn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.hesvh.cn/Article/details/grxwmeemm.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gcbafzbqu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gkprgetas.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gajhpfbmu.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gmanzvjlu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gplzsounx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/gipcjhpwk.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gwwdwlrho.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.zdbjq.cn/Article/details/grlmhhico.sHtML

[H07] 断言
来源：http://baike.fehbvm.com/Article/details/ggylgvhjk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.zdbjq.cn/Article/details/gotvfqsmo.sHtML

PHP:  assert($x > 0);
来源：http://blog.zdbjq.cn/Article/details/gbniuhkyn.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gsdxfhrhl.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gxjlesmjz.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.fehbvm.com/Article/details/gpxlzrofg.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.zdbjq.cn/Article/details/gmhutrxxb.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://m.share.hesvh.cn/Article/details/giwfjcsaj.sHtML

C#:   Debug.Assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gbyjbsiar.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/ggiupdbzs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.fehbvm.com/Article/details/gxyhxnpqy.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.fehbvm.com/Article/details/gclriuhlg.sHtML


<!-- 参考信息 -->