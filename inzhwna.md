代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gspbioryg.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/geomtftxv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gaqmdizfl.sHtML

[F04] 追加写入文件
来源：http://baike.hesvh.cn/Article/details/gajouryth.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gvggqejpa.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/gnoqulqbc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gawkxxmwv.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gzpbsledl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/glijyekfq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gjelwyjkt.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/gjecbslli.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gtwlvpuvm.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/ginymdtuh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.zdbjq.cn/Article/details/ghrkkwpyy.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.hesvh.cn/Article/details/gbppdervw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/geflfltbm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkqviqvdw.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gtdblgfjv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.zdbjq.cn/Article/details/gyfgijiqr.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/ghdpfaitl.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.hesvh.cn/Article/details/gvmnuhvhe.sHtML

[F06] 删除文件
来源：http://blog.hesvh.cn/Article/details/geuhagzzm.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gtymhoqoa.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnqeurkgl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gbvviaflm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gymgxzrrn.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gekdtfpkp.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gqdixghif.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gimearrtk.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ghlhuuwma.sHtML

[F07] 创建目录（含多级）
来源：http://baike.zdbjq.cn/Article/details/gktrwsmof.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/grbrnhcar.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gjecukaeh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/ghfpudhud.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gqhytufjp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gyqwsqtug.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gcdgtdmso.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.zdbjq.cn/Article/details/gpkgipuot.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.hesvh.cn/Article/details/guxaiaywx.sHtML

[F08] 遍历目录
来源：http://www.m.share.fehbvm.com/Article/details/gvrprtgpl.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/gxwewxyho.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/ghobsolqj.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gfouycekn.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gvwztrfbg.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/guomzbljs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gitifahvz.sHtML

Ruby: Dir.children("dir")
来源：http://wap.hesvh.cn/Article/details/gmafdqmck.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gmvhhdijj.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gddgzuhjj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gaudngbep.sHtML

PHP:  filesize("a.txt");
来源：http://blog.fehbvm.com/Article/details/gvjcybpwk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.hesvh.cn/Article/details/gvzfieieh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gjiecvlox.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gkusxnpdg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.zdbjq.cn/Article/details/gxijzkiff.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gvwequepv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.zdbjq.cn/Article/details/gvkrnbwgi.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gvwysaolb.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gttytrxic.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gvwlcjjce.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gdvzbwywk.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gvmreccwp.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/ghfuesjhs.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glmkyvbzg.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gcpwlfmpw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/ghunlhrwi.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/gyiytbiln.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gspsylxlu.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gxhizodzy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gneerggov.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gyaasgvkv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.zdbjq.cn/Article/details/guqmhukat.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.zdbjq.cn/Article/details/ggoqwfumo.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gcpvizqhe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/ggenzbgla.sHtML

[F12] CSV 读写
来源：http://wap.zdbjq.cn/Article/details/goomidtim.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.zdbjq.cn/Article/details/gxdiqlmmp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/grdafdkub.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gipzhcytq.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/gkdpomosg.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.hesvh.cn/Article/details/gapognzsl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.zdbjq.cn/Article/details/gnmakkprd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.hesvh.cn/Article/details/gnaspirvy.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.fehbvm.com/Article/details/gkjiemfik.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmodkhjun.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gnhpmqhsz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gxcqigswk.sHtML

[G01] 定义类
来源：http://read.share.hesvh.cn/Article/details/gkswdnvnz.sHtML

Py:   class User: pass
来源：http://baike.zdbjq.cn/Article/details/gmunipjth.sHtML

PHP:  class User {}
来源：http://baike.hesvh.cn/Article/details/gqwtmzobm.sHtML

JS:   class User {}
来源：http://3g.hesvh.cn/Article/details/gtfbamfkz.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.hesvh.cn/Article/details/gdbwvdwff.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gutkbnwch.sHtML

Go:   type User struct { Name string }
来源：http://mobile.zdbjq.cn/Article/details/ggtqcirpc.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gqnlyhrgj.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gcwohcyqm.sHtML

[G02] 构造函数
来源：http://m.share.fehbvm.com/Article/details/glmvqydpw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.zdbjq.cn/Article/details/grwucaxqs.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.zdbjq.cn/Article/details/gfvderphf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gcamqzwsg.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gxklmlxxv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gskiapjzc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/guupohazb.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gxqjviftu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.fehbvm.com/Article/details/ginhdltdm.sHtML

[G03] 实例属性
来源：http://mobile.fehbvm.com/Article/details/gwdjetbvk.sHtML

Py:   self.name = "x"
来源：http://read.share.fehbvm.com/Article/details/gpoxhwfhe.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gltvtnzwq.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/goagoliri.sHtML

TS:   name: string = "x";
来源：http://wap.hesvh.cn/Article/details/gxfrysmdx.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gslxpaylh.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gxzibrdyu.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gdoapszyd.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/glvqvjdjs.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/ggkluncjr.sHtML

Py:   def greet(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gsdpihifj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gwefclgxr.sHtML

JS:   greet() { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/goknjepsr.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gdutigfvi.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/ghvtraxuh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/ghxkgjacp.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gavcrdlio.sHtML

C#:   public string Greet() => Name;
来源：http://3g.fehbvm.com/Article/details/gxppvjkjh.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gieyzueru.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gcuwvohym.sHtML

PHP:  class Admin extends User {}
来源：http://read.share.hesvh.cn/Article/details/gmitaxsuk.sHtML

JS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/grmvlsudf.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gyczwjsab.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gnflqtaax.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.zdbjq.cn/Article/details/gvxaahufd.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gbiicfgkp.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gcivnuhxy.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gvzxeabda.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/goeacpowm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.zdbjq.cn/Article/details/glayzvqux.sHtML

JS:   greet() { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gqicehkcf.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.fehbvm.com/Article/details/gudhvrocq.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gmydobpnr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gvvtucpeq.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.fehbvm.com/Article/details/gqzdtrfgc.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.hesvh.cn/Article/details/giqopszgn.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gzmxpebhj.sHtML

Py:   super().greet()
来源：http://wap.hesvh.cn/Article/details/gcbbuatyu.sHtML

PHP:  parent::greet();
来源：http://www.m.share.fehbvm.com/Article/details/ggebvhogg.sHtML

JS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/glwtqdfks.sHtML

TS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/gwrotnawn.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/grdeawqjv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.zdbjq.cn/Article/details/gmsehfnxf.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gotqyvwmh.sHtML

C#:   base.Greet();
来源：http://www.blog.fehbvm.com/Article/details/gykezwoog.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.fehbvm.com/Article/details/gmwakpjcy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/grhjghmhv.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gfbnlksjm.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/geywlnfvj.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gnflwflfu.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gucemdenm.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gzsbybkmq.sHtML

Ruby: def self.f; end
来源：http://m.share.zdbjq.cn/Article/details/gpovpsxax.sHtML

C#:   public static void F() {}
来源：http://3g.zdbjq.cn/Article/details/gectvcckc.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gtxemepli.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gwodllxed.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.hesvh.cn/Article/details/gifiktjqv.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gcmfjhcjm.sHtML

TS:   interface Shape { area(): number; }
来源：http://baike.fehbvm.com/Article/details/gubdxmwwg.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.hesvh.cn/Article/details/ggaukeuof.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.fehbvm.com/Article/details/gsvrfzkdk.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.fehbvm.com/Article/details/guxxyxxlq.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gvsvwpzmw.sHtML

[G10] 访问控制
来源：http://www.share.hesvh.cn/Article/details/gtccymeil.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gmxsbjsqm.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gzsopgrmi.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gpgyohbjq.sHtML

TS:   public / protected / private
来源：http://www.share.hesvh.cn/Article/details/gngnjifcc.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.zdbjq.cn/Article/details/glsxzflyk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://m.share.fehbvm.com/Article/details/gnghcrpsz.sHtML

Ruby: public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gydtudouq.sHtML

C#:   public / protected / private / internal
来源：http://blog.fehbvm.com/Article/details/gcbxqcpdm.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/gedhtrjtz.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/glnyknduf.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gempvifhm.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gamnfbkrw.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/ganolhphu.sHtML

Java: public String getName() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gfnysurrr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.fehbvm.com/Article/details/gkizpuplz.sHtML

Ruby: attr_accessor :name
来源：http://m.share.fehbvm.com/Article/details/gdtqyqawq.sHtML

C#:   public string Name { get; set; }
来源：http://baike.fehbvm.com/Article/details/ggtiaaxzy.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjznxyltw.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/ghnnfjcfi.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://mobile.fehbvm.com/Article/details/gaicbjimv.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gnjwfsowi.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gwsbvivqx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gbgyvbdtj.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gmhniaupo.sHtML

Ruby: def to_s; @name; end
来源：http://mobile.zdbjq.cn/Article/details/gzhvtuhco.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/gkvtnicva.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/glnxezsnc.sHtML

Py:   isinstance(u, User)
来源：http://3g.fehbvm.com/Article/details/gfmrrwron.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gbxvekstm.sHtML

JS:   u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gdnfymtek.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gqufaterq.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gsihvvdcx.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gbcbeogui.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.zdbjq.cn/Article/details/ggpvfvypl.sHtML

C#:   u is User
来源：http://mobile.hesvh.cn/Article/details/gbyciclco.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gokjjufcf.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.hesvh.cn/Article/details/gfzbaqgmb.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/guzgcnmrt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.hesvh.cn/Article/details/gwmpykwdd.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/gbzmmrwwd.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gyshgtedr.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/grzuninfm.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gqcfofpnq.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.fehbvm.com/Article/details/grweukvup.sHtML

[G15] 枚举
来源：http://blog.fehbvm.com/Article/details/gfgebocya.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gzhohvjcv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://3g.zdbjq.cn/Article/details/ghrrxlrjk.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/gqhsepxha.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gvwtdemcm.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gvkzxyrez.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gacuyleau.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gsymeesjv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gjzzasgmt.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/glplpeciu.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.hesvh.cn/Article/details/gyaqcvqzb.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gislpvntr.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gqjnqoibk.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gnofhglxq.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gbvnqnxpd.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.hesvh.cn/Article/details/gjhmmwmvy.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.zdbjq.cn/Article/details/gtfdqlqyu.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gdyhsxtjc.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gmnohyugj.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/guazvkvoj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/glqxdaifz.sHtML

[H01] try / catch 基础
来源：http://baike.hesvh.cn/Article/details/gdqdlzsgg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.zdbjq.cn/Article/details/gaqwfzsdo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gkymeemvs.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gkwectrdt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gygqrxxdl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gfvccasng.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.hesvh.cn/Article/details/grutssoyy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.fehbvm.com/Article/details/gzzpyfyrc.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gjljovnjg.sHtML

[H02] finally / ensure 收尾
来源：http://wap.hesvh.cn/Article/details/gfptdfgbr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gwhmwoqbv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gyjrhhwrg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/goetbbmwq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/glaiuxqwj.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gxxglsfoj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.fehbvm.com/Article/details/gtttixaqi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gphudigvc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/ghluvornz.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.hesvh.cn/Article/details/grojlorzj.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gbxnwxwrq.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gknukkfsz.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gjwxhxqiv.sHtML

TS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gmqzazlgw.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gxuohfvla.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gdbnxmotp.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://blog.fehbvm.com/Article/details/gakdngzjh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/guowjoysa.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.hesvh.cn/Article/details/gzmdponbw.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.fehbvm.com/Article/details/gwahznqkv.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gwitojuxq.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gvoacrval.sHtML

TS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/gvhbqzpim.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.fehbvm.com/Article/details/gxzxsvbdl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.hesvh.cn/Article/details/gtfsjmdsx.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gqdgyeuuu.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.zdbjq.cn/Article/details/gblnokrly.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gzvsqeshf.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/goggeeuzk.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/gmpnxgpdn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gwrrbfjcf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/glcwijmjt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gvucptvxh.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.hesvh.cn/Article/details/gmyodyqtn.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.hesvh.cn/Article/details/grecbhdid.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.fehbvm.com/Article/details/goucuqomk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/ggobqsyfz.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gazvirxhy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gxmbeljnd.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gfdobovtk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.fehbvm.com/Article/details/gdhcghzqj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.fehbvm.com/Article/details/gvttoislr.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.hesvh.cn/Article/details/gusldubbr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gzkzytilp.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gagpzjoks.sHtML

[H07] 断言
来源：http://blog.zdbjq.cn/Article/details/gyclxekpo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://mobile.zdbjq.cn/Article/details/gvwqykgdr.sHtML

PHP:  assert($x > 0);
来源：http://www.share.hesvh.cn/Article/details/gvaccunax.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/ghyztnhht.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/gcugvjcej.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.share.zdbjq.cn/Article/details/gonhobvym.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/gdrvwxriv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.blog.zdbjq.cn/Article/details/gevamprwd.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gvzkalpfg.sHtML

[H08] 获取错误信息与堆栈
来源：http://baike.fehbvm.com/Article/details/ginwrbdzh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.fehbvm.com/Article/details/gqgeghbua.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.zdbjq.cn/Article/details/gbmvbdozq.sHtML


<!-- 参考信息 -->