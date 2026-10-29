代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gzfblggld.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.hesvh.cn/Article/details/gcntqcbvc.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/gjqaqgljo.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gqgrapvqc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gfzvpqaot.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gpsbbozra.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gbhhkgmfn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gwyedrivb.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gfrtzrmpx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/glbhapmcp.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gulkjsvtf.sHtML

[F04] 追加写入文件
来源：http://m.share.fehbvm.com/Article/details/gtaysnrzf.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fehbvm.com/Article/details/gevrsuehg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gpvadrnda.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/gzcylozqr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gqoecglwm.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.blog.fehbvm.com/Article/details/gowtqnxxh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.zdbjq.cn/Article/details/gprgxwthu.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/guykqcung.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.fehbvm.com/Article/details/gddkvxool.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gsstqmxwn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/gbtwfmdhq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gmwfgdmyd.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gqghobtuk.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtnlreglp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gygvgzoax.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gdfcsfirk.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.hesvh.cn/Article/details/gortwnbfa.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ggpkdkkyo.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gxwzsbiio.sHtML

Py:   os.remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/giomyjvae.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/guceasabf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grdxpzrwn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdqaroroj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gzyewfspv.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcggtisoy.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gsfzbijqq.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gsjxxfdyq.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gcmgwllhq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/gmbfoxcph.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gjexsrkaj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/grryqjjsp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.hesvh.cn/Article/details/gpbrkjdxq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gkexydrly.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gieeekchm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/geksghuqw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gcfsnczby.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/gjrvwkwon.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.zdbjq.cn/Article/details/grfoefxtl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.hesvh.cn/Article/details/gheownfmq.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.hesvh.cn/Article/details/gkpigeulk.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/guiyywjwb.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.fehbvm.com/Article/details/grfeatvtg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gesgogyus.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gecgubpdv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gknyuzhuc.sHtML

[F09] 获取文件大小
来源：http://wap.fehbvm.com/Article/details/gevmgehsy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gafehtelt.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ghpupxctm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gtgqwaall.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/ghjwdfvhd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gjshgrspl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gnxbsngkr.sHtML

Ruby: File.size("a.txt")
来源：http://baike.fehbvm.com/Article/details/gwnmjazms.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gonfjdgto.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gtvyjmcvk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gdrwxwsil.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gwmaiyxqe.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/guocetvgn.sHtML

TS:   path.extname("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmpokimxd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.hesvh.cn/Article/details/guwtivwvc.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gjonyqpzh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gtiwlchjg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gpnauuclb.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/ghbrzgbnp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gwsjcjmtj.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gfnksbwxd.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghzinyxfv.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gahbxmnxj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/ghacntefd.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gksguhjcg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxuzudjyi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.zdbjq.cn/Article/details/gybwlvjdq.sHtML

[F12] CSV 读写
来源：http://blog.hesvh.cn/Article/details/glgfeddib.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.hesvh.cn/Article/details/gvlslonez.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gdiazoblq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.hesvh.cn/Article/details/ggagwuvaq.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/glhlojipw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gwaqldmrl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gdwtoeqxe.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/gjzopsrck.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/gkcyuhvjj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkhettymz.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gpwuxtblb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/glttwbxkw.sHtML

[G01] 定义类
来源：http://www.m.share.zdbjq.cn/Article/details/gypjczmvz.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/gfixwmanw.sHtML

PHP:  class User {}
来源：http://mobile.hesvh.cn/Article/details/gwtqultgk.sHtML

JS:   class User {}
来源：http://wap.hesvh.cn/Article/details/gffdnzzjz.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/groqxpltt.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gfqcbwrma.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gxekdqqsw.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/gtveikpdz.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gjskutqil.sHtML

[G02] 构造函数
来源：http://m.share.zdbjq.cn/Article/details/ghqfnafts.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gnurpcfng.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.m.share.zdbjq.cn/Article/details/glnkojbmz.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gqubbapqp.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gajbiazzw.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gfpbtgfkl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gezeinlup.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.fehbvm.com/Article/details/gbiswhniy.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.zdbjq.cn/Article/details/gaflcjxop.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gxrwhktot.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gapcchacp.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gjsivrwha.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gdirgsvnu.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/gngetdtfb.sHtML

Java: private String name;
来源：http://wap.fehbvm.com/Article/details/gsxidirrx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gsramgmii.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gacprbsfe.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gwrqkqkac.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gcdobbnav.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gbxbrgrsh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwtrcuroo.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gfqqeduaa.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gfrtbxorf.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/glqovwglj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.zdbjq.cn/Article/details/giechjcno.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gbchogssc.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gbrehlcsq.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gxtqodtby.sHtML

Py:   class Admin(User): pass
来源：http://blog.fehbvm.com/Article/details/giopsqxts.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gdtjgqklp.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/grbfnzfcz.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/glipuvawg.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/glwuxcihv.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gvoiamxwy.sHtML

Ruby: class Admin < User; end
来源：http://www.share.hesvh.cn/Article/details/gqtrrnrqg.sHtML

C#:   class Admin : User {}
来源：http://baike.hesvh.cn/Article/details/gpmlzydbi.sHtML

[G06] 重写方法
来源：http://m.share.zdbjq.cn/Article/details/gloxnwtnq.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.zdbjq.cn/Article/details/gdyvxstqb.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gayucxvph.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.zdbjq.cn/Article/details/gtzhvqcuz.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gvgbhxeov.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gfnfoeozr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.zdbjq.cn/Article/details/gehxbxrpg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.hesvh.cn/Article/details/gjrddedie.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/glbevsery.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gcfoipnui.sHtML

Py:   super().greet()
来源：http://m.share.fehbvm.com/Article/details/gjfxvccmu.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/gfriikrhn.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gmdzzbfpp.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gjnnzifab.sHtML

Java: super.greet();
来源：http://www.share.fehbvm.com/Article/details/gehmimbbe.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/gajgdqizs.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gaytqsdwb.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gfyijnfzr.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gvitekyij.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gpoeykeej.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gpoinpeoc.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/godfimefe.sHtML

TS:   static f(): void {}
来源：http://baike.fehbvm.com/Article/details/gxbvxcycm.sHtML

Java: static void f() {}
来源：http://www.m.share.hesvh.cn/Article/details/ghkekuslu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gmfrolsni.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/ggzqfkknj.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gvqyewfvj.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.hesvh.cn/Article/details/ghsiurwim.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.zdbjq.cn/Article/details/gajpqrmdr.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gepxntvnc.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gdyzjfjhu.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/grxyeucvy.sHtML

Java: interface Shape { double area(); }
来源：http://baike.zdbjq.cn/Article/details/gezolhsnh.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gewwioofc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.fehbvm.com/Article/details/gaubzekce.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gsnsxysqp.sHtML

[G10] 访问控制
来源：http://www.m.share.hesvh.cn/Article/details/gsmkbaxul.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/grjvruqxo.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gwprsijfr.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gdkkamqof.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gsiigpesi.sHtML

Java: public / protected / private / 默认包级
来源：http://www.blog.hesvh.cn/Article/details/gojukydla.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.fehbvm.com/Article/details/gdhdkebdw.sHtML

Ruby: public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gpmrnmpfo.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gmrqqodlw.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gsexvfpad.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gbdazonch.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gynilptws.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gkjtnpcew.sHtML

TS:   get name(): string { return this._name; }
来源：http://3g.zdbjq.cn/Article/details/gtbbkfdkp.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gfkpacjpl.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gsetpddfh.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gcjlgzaqw.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/glbztxrvi.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/gftcrbtoc.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/gvotplvdc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gqnjzcnfc.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gmztwaqqw.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.zdbjq.cn/Article/details/grgcvvyxj.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqlzzlcos.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/goubklolo.sHtML

Ruby: def to_s; @name; end
来源：http://blog.zdbjq.cn/Article/details/gqscldnpl.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.hesvh.cn/Article/details/gbtxwjrbs.sHtML

[G13] 判断对象类型
来源：http://m.share.hesvh.cn/Article/details/gtqsmmwvr.sHtML

Py:   isinstance(u, User)
来源：http://m.share.fehbvm.com/Article/details/gvtajjril.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/guyjdilhs.sHtML

JS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/govbwzcqm.sHtML

TS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gcqnuknhq.sHtML

Java: u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/ggxtmhzby.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.hesvh.cn/Article/details/gfdcbquqq.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gumscscnw.sHtML

C#:   u is User
来源：http://www.m.share.zdbjq.cn/Article/details/gzmfypdfr.sHtML

[G14] 数据类 / record
来源：http://read.share.zdbjq.cn/Article/details/gnztfwcgr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.hesvh.cn/Article/details/glvnnqyhn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/gxxtxkqeo.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gwommazdq.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.zdbjq.cn/Article/details/gmyrrnilu.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/ghjersnwj.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gbyjffzxk.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.blog.fehbvm.com/Article/details/gvtfxthzq.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.zdbjq.cn/Article/details/gsydorzep.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gwkbiwdvg.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/gawmzeqoe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.hesvh.cn/Article/details/gvjxngqxe.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.hesvh.cn/Article/details/glulzbigw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/girthksoz.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gphepuxtj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.hesvh.cn/Article/details/gcihzulao.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gtzsjetyx.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gznnuzxee.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gfgjpklfk.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gonquvwph.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gxlmleasr.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gpvkrgisk.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gldjeqvgi.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://baike.zdbjq.cn/Article/details/gvebhivms.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.fehbvm.com/Article/details/gpkuedzmp.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gqohbejcl.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gnqgxmqqt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gmuvhxawa.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/ggtokqwsh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjcrclzkw.sHtML

[H01] try / catch 基础
来源：http://m.share.fehbvm.com/Article/details/gnletmzef.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://baike.zdbjq.cn/Article/details/grprxqbox.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://baike.zdbjq.cn/Article/details/gmtkifvtd.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/glanpsxyv.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.fehbvm.com/Article/details/gpxjabpra.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gajxutmdb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/guuytzzuc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.zdbjq.cn/Article/details/givuejdrl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.blog.zdbjq.cn/Article/details/grhffuzjo.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gbvyugslj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.hesvh.cn/Article/details/gnmshdbzd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/giitiypbw.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gfwbjmdvu.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gcinjqbku.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gowydqmhh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gsjjspvqt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/glewqnjky.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.zdbjq.cn/Article/details/gnfdsuiqw.sHtML

[H03] 主动抛出异常
来源：http://www.share.zdbjq.cn/Article/details/gekdkimse.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gndtpwdzk.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gjnkmknzr.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/gkmtsyrwf.sHtML

TS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gtgjgprej.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gmmvprtsp.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/goqonulaw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.zdbjq.cn/Article/details/goiwzuotc.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gsuuzhkzi.sHtML

[H04] 自定义异常类型
来源：http://m.share.fehbvm.com/Article/details/gcqbcmxby.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gtjequjhe.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/glwqhbkux.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/glfacnrwj.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.fehbvm.com/Article/details/glotmiixn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gfkgqeowc.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/ggyhxfxnv.sHtML

Ruby: class MyError < StandardError; end
来源：http://blog.zdbjq.cn/Article/details/gjyosdiuy.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.zdbjq.cn/Article/details/gdztjsayr.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gbwckonak.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/gzhgkmrae.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/grbxzgwzz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gzkgfxhjd.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gcgezwbdg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/gbcwfhaiv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/gbgfnowql.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/gbhwnkenk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://3g.hesvh.cn/Article/details/ggflfmuru.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gnarbwjrf.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/guilrsdma.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/guhdbilpy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.zdbjq.cn/Article/details/ggevxjqrj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gmrxtgifq.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gaunvlkzq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.zdbjq.cn/Article/details/grlulctwn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gcnvhsipw.sHtML

C#:   obj?.A?.B ?? default
来源：http://read.share.zdbjq.cn/Article/details/gdshdomtp.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gjumaevbu.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gtyaxpzvw.sHtML

PHP:  assert($x > 0);
来源：http://read.share.hesvh.cn/Article/details/gqjuurqss.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gkgzosuqv.sHtML


<!-- 参考信息 -->