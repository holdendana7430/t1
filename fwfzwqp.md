代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gckpwzcfe.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/ggmrnbscy.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/giavexuio.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gezldoubh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.zdbjq.cn/Article/details/gvqwgcjww.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.fehbvm.com/Article/details/ggsyzezwb.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gassurbob.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.zdbjq.cn/Article/details/gakcemvwd.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.zdbjq.cn/Article/details/gfxxnwcxd.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/ghmdheqda.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gadoxdssb.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/ghtgwgjdc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/godkdlibx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gcdrqgrko.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/grookmavu.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gpgdxgfim.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gbsaunjze.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gorsvkltj.sHtML

Py:   os.remove("a.txt")
来源：http://baike.hesvh.cn/Article/details/gvtpnmptq.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gwhwcfofa.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/ghiuwbwcm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gyxqgtwia.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gdgyywbxg.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gtayyuwwe.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ghvmjsvbt.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnucprdph.sHtML

[F07] 创建目录（含多级）
来源：http://3g.hesvh.cn/Article/details/gukutbqso.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gytzfjxdr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gapbjkuvx.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gydqqiyuo.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gknxencxb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/glnzqtkud.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/ghzqluxzx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gxpusrtzg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.zdbjq.cn/Article/details/gjwbymffh.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/ggxhplrun.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gfslvbsgd.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/ghqvzodcj.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gkbjsqhpg.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gjwtilakp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxaafppi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gyrzyocrb.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gcrvorqmv.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gqqlckyef.sHtML

[F09] 获取文件大小
来源：http://www.share.zdbjq.cn/Article/details/gqpqxntjb.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gihxvjnuj.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fehbvm.com/Article/details/gvvitxjcj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.zdbjq.cn/Article/details/gqsifgxct.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/grorrlepb.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/grqklwebq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.hesvh.cn/Article/details/gyytdcdsy.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gczlnvwgy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/grjnxnacf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gjqrakcxf.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gqiwakwht.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.zdbjq.cn/Article/details/gbpgrdrxs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gdzajchtx.sHtML

TS:   path.extname("a.txt")
来源：http://baike.hesvh.cn/Article/details/gmiduhnoi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gzkqspvlx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjtjdsnzc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gkdddukrx.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkckcmlcr.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/ggfgiboei.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gfnobczor.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.zdbjq.cn/Article/details/gevhinlbf.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gjpmwqmmy.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gebpfgqbq.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/garjnaual.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.m.share.hesvh.cn/Article/details/gwusftkst.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/ggbfgnvgy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://3g.zdbjq.cn/Article/details/gxdquzydh.sHtML

[F12] CSV 读写
来源：http://mobile.hesvh.cn/Article/details/ghxnhsszy.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/gfhaizppy.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gbrxjcisa.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.zdbjq.cn/Article/details/ganbwsxzd.sHtML

TS:   // 同上
来源：http://www.blog.zdbjq.cn/Article/details/grjxwibae.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gssgjjqah.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gdztmgreb.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://3g.fehbvm.com/Article/details/gajkkfwhf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/ghnvhxhlu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtbygsyws.sHtML

G. 面向对象
来源：http://baike.zdbjq.cn/Article/details/ggcuajqqk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grbagdacd.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gfwyvsiza.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/givqcusmu.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/ghacjvwbg.sHtML

JS:   class User {}
来源：http://baike.zdbjq.cn/Article/details/gtypudymu.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.zdbjq.cn/Article/details/ginjfcsop.sHtML

Java: class User {}
来源：http://mobile.hesvh.cn/Article/details/gmebmjirr.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gwrtksznv.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/ggxkhcmnz.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gfndixqft.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gdybrhzhj.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/graygyfpd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.zdbjq.cn/Article/details/gcohrqrhi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/grmipbabc.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fehbvm.com/Article/details/gibzticee.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gjuswyqbu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.hesvh.cn/Article/details/gnwrkcxax.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/grnfaarag.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.hesvh.cn/Article/details/gbxdwggrb.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/ghuoppuwz.sHtML

Py:   self.name = "x"
来源：http://m.share.fehbvm.com/Article/details/gwjbjquqn.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gxwcgupwh.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/gqxwkioti.sHtML

TS:   name: string = "x";
来源：http://www.share.zdbjq.cn/Article/details/glsrhkvws.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/giewfetgy.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gycgaxnyo.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gdmwwvygd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gbpqeahlz.sHtML

[G04] 定义方法
来源：http://www.blog.zdbjq.cn/Article/details/gjjaoptdd.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.fehbvm.com/Article/details/gmadgohyd.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfynenpfb.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gyunhnvwo.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gfnhvgtzs.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gxuerabei.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/ghkzkuvfd.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gadrtspmo.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gfobcjpkx.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/glgvnuoqd.sHtML

Py:   class Admin(User): pass
来源：http://wap.fehbvm.com/Article/details/gqbsnpgni.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gevhvcfgb.sHtML

JS:   class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/guwnijrrc.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gldloedsv.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gjmcbjjpo.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.hesvh.cn/Article/details/gfisumxhq.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gfsujzjif.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gwuthzzcx.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gjtmufhuh.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gqcmqvfnr.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gshnszltr.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gfqpqmosy.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gqoaotxqi.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gdiclvaxx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.zdbjq.cn/Article/details/gfiatvzpr.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.zdbjq.cn/Article/details/gifaruipr.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.fehbvm.com/Article/details/gldgrpfxi.sHtML

[G07] 调用父类方法
来源：http://3g.zdbjq.cn/Article/details/gynsqkfvr.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gbhmhpjop.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gprbaipnj.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/guaxorywx.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gqurngcnv.sHtML

Java: super.greet();
来源：http://mobile.fehbvm.com/Article/details/gbbswzmyo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.hesvh.cn/Article/details/gqkvafckb.sHtML

Ruby: super
来源：http://baike.hesvh.cn/Article/details/gmspxlksx.sHtML

C#:   base.Greet();
来源：http://blog.fehbvm.com/Article/details/gmksmdzks.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gsiwjmxkk.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.zdbjq.cn/Article/details/glmdyyytp.sHtML

PHP:  public static function f() {}
来源：http://blog.hesvh.cn/Article/details/gijsnfcjy.sHtML

JS:   static f() {}
来源：http://baike.zdbjq.cn/Article/details/griikrrtf.sHtML

TS:   static f(): void {}
来源：http://www.blog.hesvh.cn/Article/details/gkdyucmoe.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/grvardbcf.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/gzpdqqdkc.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/gsoyjgota.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/grodvlmrc.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gjtwmrscw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/ghuqnzaub.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/gmpqxpqkz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.hesvh.cn/Article/details/govnlwult.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gqzjtyouc.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/gwvxosfdt.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.zdbjq.cn/Article/details/gkchbbmyx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.hesvh.cn/Article/details/giuaqbpru.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gmxpjpvyj.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gngmsvxwu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gnfbvixde.sHtML

PHP:  public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gfkczrlwc.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gkikdinez.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/ghumupawe.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gnmxnqhcr.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/grwpznhsr.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/ghmvnjykj.sHtML

C#:   public / protected / private / internal
来源：http://3g.fehbvm.com/Article/details/ggwggefpd.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gxhonukdc.sHtML

Py:   @property 与 @x.setter
来源：http://wap.zdbjq.cn/Article/details/goglbvsmt.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/glbtdgqgo.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gnfudklco.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/glctzklvq.sHtML

Java: public String getName() { return name; }
来源：http://baike.fehbvm.com/Article/details/gwgabawnc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/ghzbuvivi.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/guyzeawpu.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gnumzvqpk.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/glzjwgnpm.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gcagbuvzz.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/ggvhsbyir.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/glnysggcu.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gnmksckbl.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.fehbvm.com/Article/details/glpfwnoqp.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gohsyjnar.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gkaloywke.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gakehuguz.sHtML

[G13] 判断对象类型
来源：http://m.share.zdbjq.cn/Article/details/gabyulqkr.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gmrdhvwpp.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gaarepimp.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gjgrnelyu.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gpmisvcij.sHtML

Java: u instanceof User
来源：http://blog.hesvh.cn/Article/details/gybkyuzun.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gofgmpheh.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvonbkit.sHtML

C#:   u is User
来源：http://www.blog.fehbvm.com/Article/details/giwpldmxh.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gjpjwmlot.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gyoruxdrw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gjnkknone.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.hesvh.cn/Article/details/gjexokinu.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.hesvh.cn/Article/details/gpoycmkuy.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gbfsppjzc.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.fehbvm.com/Article/details/gsfflwyxj.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/ghyngiifm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.fehbvm.com/Article/details/ghfspsfpz.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gbltlrqhf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://m.share.zdbjq.cn/Article/details/grwgujcyd.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gvggidliz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gicvvnwpx.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gzaruksnn.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/gckfuejeo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gwzdtkysz.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.fehbvm.com/Article/details/ghdifvugh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/gjwthebbj.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gqqrokamr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.fehbvm.com/Article/details/gczauvnki.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/gzjbnpkzl.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gcsksthpy.sHtML

TS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gdaljtqyp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://wap.zdbjq.cn/Article/details/gfrleyaen.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gcmjyubdb.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gvyvwdtsa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gjaotbpmk.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gslsvslwx.sHtML

H. 异常与错误处理
来源：http://blog.fehbvm.com/Article/details/gfnwfmzzi.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gilsdltjr.sHtML

[H01] try / catch 基础
来源：http://mobile.fehbvm.com/Article/details/gecttnved.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gukxahaes.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.zdbjq.cn/Article/details/gwcoxjjig.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gunmnsxpz.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.hesvh.cn/Article/details/gpdwkpfuq.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/gohnvuwwb.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gholkwjgo.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gnxjbqxkx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gggoxvjjk.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/giaestlrb.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gesjmmpgq.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gwiejfezb.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gbixsqips.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gxfoqjiqf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/ggmhlcnuq.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.zdbjq.cn/Article/details/gzdhghqoh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/gdmicvmdw.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/grsgbdsbd.sHtML

[H03] 主动抛出异常
来源：http://3g.zdbjq.cn/Article/details/gwsawzvkv.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gvncmotjl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gwbuwsfjh.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gxosszhvq.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gucpbghfv.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/giczupujy.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.zdbjq.cn/Article/details/gjqxaqmmu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.hesvh.cn/Article/details/gbpgkgolz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gpnkbaexf.sHtML

[H04] 自定义异常类型
来源：http://3g.fehbvm.com/Article/details/gmiezadie.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/gekdeijno.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gdqnakeoz.sHtML

JS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gvfhdxorn.sHtML

TS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gmxrobxhf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gbgbrnohx.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gnabcdcfz.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.hesvh.cn/Article/details/gzxuashzr.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.zdbjq.cn/Article/details/gfkkqxmhz.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/grmcdzfgj.sHtML

Py:   except ValueError as e:
来源：http://3g.zdbjq.cn/Article/details/ggynjsmug.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gednedvmo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/gpcidmlff.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gfiyhjlmb.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.hesvh.cn/Article/details/gniexfnpn.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.hesvh.cn/Article/details/ghvgmsotw.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.fehbvm.com/Article/details/gxojonntk.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.fehbvm.com/Article/details/gclskevpn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.fehbvm.com/Article/details/gefhlqakh.sHtML

Py:   value = d.get("k") or default
来源：http://blog.zdbjq.cn/Article/details/gvrabfhul.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/ggmmxapta.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://mobile.fehbvm.com/Article/details/geyebyarv.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gtykapvjs.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/gmchmaclk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/gakzzdqbq.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gwnxooxmi.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gdfvcyckj.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/ggfpkcwng.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.zdbjq.cn/Article/details/gntjihwgo.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gdfnvlytd.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.hesvh.cn/Article/details/gfeigzzjq.sHtML

TS:   console.assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gtbabgvwm.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.zdbjq.cn/Article/details/gteuxtlwm.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/gwjfemgml.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gevffgeen.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/guxmejvib.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gspzocshv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.zdbjq.cn/Article/details/gyxblosrc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.hesvh.cn/Article/details/ggzkrxuks.sHtML

JS:   e.message;  e.stack
来源：http://www.blog.fehbvm.com/Article/details/gykxvnmrj.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/gdtvvxzej.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://m.share.hesvh.cn/Article/details/gyicpkxuk.sHtML

Go:   err.Error()
来源：http://3g.zdbjq.cn/Article/details/gbfbhpnvp.sHtML


<!-- 参考信息 -->