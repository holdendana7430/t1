代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fehbvm.com/Article/details/ghesqkrld.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://wap.fehbvm.com/Article/details/gvhqqzbji.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gzinnclna.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/grsldyfba.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.hesvh.cn/Article/details/gurvdhsab.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gvdyvvguw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gfsxkuuby.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gomfcdefo.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.fehbvm.com/Article/details/gpbqzcwhv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gvlqosjhi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gtjfocivq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/gbzaeesij.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/gwjhacdzf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.fehbvm.com/Article/details/gvahrpfyf.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gbbyclnog.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdgyjkeqm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gojdbwods.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gkutxmeni.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.fehbvm.com/Article/details/gukdtejla.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/ghqwsyelp.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/guhleqfqj.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gbzsohvzq.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gulygsfgg.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gufhlyjij.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghvawgckh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gqobznfdf.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gwmgkyzvc.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkxonyont.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghzxmxnff.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gtzevjpen.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gqzzqopnd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gccualjaz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.hesvh.cn/Article/details/gofozvnch.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gxizdunng.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gttisobnc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fehbvm.com/Article/details/gxiosoaih.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gxqnllopi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.hesvh.cn/Article/details/gqmlhwxfr.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gjrbbraoi.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gddywlgnb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.zdbjq.cn/Article/details/gqmtejpmi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.zdbjq.cn/Article/details/grdrqgewu.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gzgdgdxkb.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/ggpptaagz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gvlnzvbpm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gnjbvbvhx.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/guazatfvl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gxqlclibs.sHtML

[F09] 获取文件大小
来源：http://blog.fehbvm.com/Article/details/gkdmoarmk.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gzwnnxahl.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gnebhhumv.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/gompyduzu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/grrpzxmfr.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gghjycbwu.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.zdbjq.cn/Article/details/gfvekjucd.sHtML

Ruby: File.size("a.txt")
来源：http://baike.hesvh.cn/Article/details/glaxqfavx.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.hesvh.cn/Article/details/gbnhasexc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.fehbvm.com/Article/details/gmylryatv.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gdrwoowed.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gesjzbmyo.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gplefvvaz.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwucrirlf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gjbevncao.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gfwjledgr.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/geymwbxjg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.hesvh.cn/Article/details/gbysncxuz.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gtwivhngv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gckbgsoio.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.fehbvm.com/Article/details/gjgidksda.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gqtlbwgeb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gjbxtsikl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/glqzqyamm.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gspwnktwk.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gyxalqmpp.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gsrsrnpwd.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gttxwprgf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gvwyiczhk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/glcftnsww.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gnkanwcqc.sHtML

TS:   // 同上
来源：http://mobile.zdbjq.cn/Article/details/granazozz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gwariplij.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.hesvh.cn/Article/details/ghsikqznd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.m.share.hesvh.cn/Article/details/glkfoijzh.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gfuquwyml.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggfceofil.sHtML

G. 面向对象
来源：http://m.share.fehbvm.com/Article/details/gdivywiax.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghjrurpze.sHtML

[G01] 定义类
来源：http://blog.hesvh.cn/Article/details/gbqbowdin.sHtML

Py:   class User: pass
来源：http://wap.fehbvm.com/Article/details/gdalnitaf.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gwaehdnwi.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/grycifxzr.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.fehbvm.com/Article/details/gjikbenew.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/gmhzqouxo.sHtML

Go:   type User struct { Name string }
来源：http://read.share.fehbvm.com/Article/details/gpivyueyl.sHtML

Ruby: class User; end
来源：http://read.share.fehbvm.com/Article/details/gchjrmpfh.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gnawcqtdr.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gtfhpehwy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.hesvh.cn/Article/details/gnouodngz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/gwlzmtyog.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwmrfjcmd.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.fehbvm.com/Article/details/gvvthiwsv.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggnfdnhmo.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gvplgpnue.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.fehbvm.com/Article/details/gactqgpwn.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvmingxjx.sHtML

[G03] 实例属性
来源：http://baike.hesvh.cn/Article/details/gtdoqhjlj.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gmueypqyw.sHtML

PHP:  public string $name = "x";
来源：http://www.share.hesvh.cn/Article/details/gjpplsggs.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/grmyepwre.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gdzfvtqro.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gyifpvrdr.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gebksrohg.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gcktnmhyr.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/ghehztxgs.sHtML

[G04] 定义方法
来源：http://wap.zdbjq.cn/Article/details/gxxfknweq.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gwftkladi.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gguesrdru.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/glqftgsdg.sHtML

TS:   greet(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/geplyvclj.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/gveqhtwui.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.hesvh.cn/Article/details/gpijpbtzg.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/gzhzxxkdl.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/grryypmrp.sHtML

[G05] 继承
来源：http://www.blog.fehbvm.com/Article/details/grbxuftkm.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/grfryefez.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/giybtfurm.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gabhwqqiy.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gopvxhvla.sHtML

Java: class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gtijwiwhd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gsimglhtf.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/gpeecwohh.sHtML

C#:   class Admin : User {}
来源：http://3g.hesvh.cn/Article/details/gffigonop.sHtML

[G06] 重写方法
来源：http://www.m.share.fehbvm.com/Article/details/gsypryxbb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.zdbjq.cn/Article/details/gpyjpyysi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gbsezioal.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.fehbvm.com/Article/details/gpjtabnge.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gdvergdjj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gfrplrqna.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.fehbvm.com/Article/details/gyscbgyix.sHtML

Ruby: def greet; "admin"; end
来源：http://wap.fehbvm.com/Article/details/gpaxxwmjy.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.fehbvm.com/Article/details/gknrmnawj.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gqrsvdssl.sHtML

Py:   super().greet()
来源：http://www.share.hesvh.cn/Article/details/gxdjbeeet.sHtML

PHP:  parent::greet();
来源：http://3g.fehbvm.com/Article/details/gsyghrtsn.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gtvttqpeh.sHtML

TS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gfgafkxyv.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gpivlbukb.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/gwudkjgwk.sHtML

Ruby: super
来源：http://mobile.hesvh.cn/Article/details/grsaoxkyf.sHtML

C#:   base.Greet();
来源：http://blog.hesvh.cn/Article/details/gdzohoicr.sHtML

[G08] 静态方法与属性
来源：http://m.share.zdbjq.cn/Article/details/gortbacfy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gelavvwsg.sHtML

PHP:  public static function f() {}
来源：http://baike.zdbjq.cn/Article/details/gntzdalyd.sHtML

JS:   static f() {}
来源：http://3g.hesvh.cn/Article/details/gkcgggxky.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gkshyniik.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/guyaqwbzw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gjtvcjjqz.sHtML

Ruby: def self.f; end
来源：http://www.m.share.hesvh.cn/Article/details/grkvraeld.sHtML

C#:   public static void F() {}
来源：http://read.share.fehbvm.com/Article/details/gzqtlniyt.sHtML

[G09] 接口 / 抽象类
来源：http://3g.hesvh.cn/Article/details/gfilieayw.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gdiepzpdi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.zdbjq.cn/Article/details/gdxvgyafd.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://3g.zdbjq.cn/Article/details/gwqowihdz.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.hesvh.cn/Article/details/gnaxlgcku.sHtML

Java: interface Shape { double area(); }
来源：http://blog.hesvh.cn/Article/details/gqbhfqhem.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.hesvh.cn/Article/details/gwscvxgei.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/gdfucdbey.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.hesvh.cn/Article/details/glxzaalvk.sHtML

[G10] 访问控制
来源：http://www.share.fehbvm.com/Article/details/gtmjcktwv.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gnwobpmlv.sHtML

PHP:  public / protected / private
来源：http://blog.hesvh.cn/Article/details/gvrdwsxju.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.fehbvm.com/Article/details/grhxldhlx.sHtML

TS:   public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gdrzjyvvh.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gwsuvuiaq.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.hesvh.cn/Article/details/gzyrumhur.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gdwkgufuq.sHtML

C#:   public / protected / private / internal
来源：http://mobile.hesvh.cn/Article/details/gxjilrknv.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/guycoaygv.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.zdbjq.cn/Article/details/glveiqytr.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gssogbldo.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.fehbvm.com/Article/details/glttxtrcl.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwdrkktdt.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gdnvabkuc.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gajxidcjx.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gmxyatoer.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gexxydyzr.sHtML

[G12] 对象转字符串
来源：http://blog.zdbjq.cn/Article/details/gomlryvrl.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gfyhrcyim.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkaqzwwja.sHtML

JS:   toString() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/grmcuwukd.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.zdbjq.cn/Article/details/ggpubparn.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gfetdktby.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/groctyikw.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gimlnbtuy.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gysboqffw.sHtML

[G13] 判断对象类型
来源：http://baike.hesvh.cn/Article/details/gsycxswgh.sHtML

Py:   isinstance(u, User)
来源：http://m.share.zdbjq.cn/Article/details/glwuaqssf.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gtdnvqxyh.sHtML

JS:   u instanceof User
来源：http://blog.zdbjq.cn/Article/details/glawarmrl.sHtML

TS:   u instanceof User
来源：http://mobile.fehbvm.com/Article/details/giwhhufqo.sHtML

Java: u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gtmjkjyze.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gurmkhglh.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gugdtmcyy.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gybhgvpiw.sHtML

[G14] 数据类 / record
来源：http://mobile.zdbjq.cn/Article/details/guzonxjpx.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/ghxvhfhcw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gwohdlcid.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.zdbjq.cn/Article/details/gbzbuqytj.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gisnvaywd.sHtML

Java: record User(String name, int age) {}
来源：http://baike.zdbjq.cn/Article/details/gkgroeczz.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gbegszxwv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/getsahokm.sHtML

C#:   record User(string Name, int Age);
来源：http://wap.hesvh.cn/Article/details/gukpjagnm.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gkomnizop.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/ggcukpcsu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.fehbvm.com/Article/details/guerplqjp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://m.share.hesvh.cn/Article/details/gfttvqqog.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.zdbjq.cn/Article/details/grcbqmuag.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gcybptbtf.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/ggyntacsm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gklotokgh.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/gseabbnix.sHtML

[G16] 对象转数组 / 字典
来源：http://mobile.hesvh.cn/Article/details/gddtasjxi.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gijvxqjui.sHtML

PHP:  get_object_vars($obj);
来源：http://blog.zdbjq.cn/Article/details/gurylquza.sHtML

JS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gfxnuruco.sHtML

TS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gmrhhuszx.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gailuiccy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gqurzmlyb.sHtML

Ruby: obj.instance_variables
来源：http://3g.zdbjq.cn/Article/details/goyawczmf.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gwdtkgigi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gywysnzcu.sHtML

H. 异常与错误处理
来源：http://www.blog.zdbjq.cn/Article/details/gjdnvjedg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdsdrxbri.sHtML

[H01] try / catch 基础
来源：http://3g.hesvh.cn/Article/details/gvvaofmfr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.hesvh.cn/Article/details/grwilzwud.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gktefyrlk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.zdbjq.cn/Article/details/gbygzqrcf.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gbcesdddd.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gdtlnvqou.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.hesvh.cn/Article/details/geerfuvlt.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.hesvh.cn/Article/details/gaxakcutx.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsqskjozy.sHtML

[H02] finally / ensure 收尾
来源：http://baike.hesvh.cn/Article/details/gvrizidst.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gwdohtjkc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/gmmqfjwfg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gvevlolmg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gpiljixel.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gsmnhpqax.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.fehbvm.com/Article/details/gcudghpai.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gculmdhoc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gbarmjdtj.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/gctyomatw.sHtML

Py:   raise ValueError("错误信息")
来源：http://mobile.zdbjq.cn/Article/details/guxrxbdlx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gzvpdwhlx.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/ggkdfkqfy.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gfndxfayd.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/grfxisehs.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gdbgzqqxn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/gjlhbhbzh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/greqkpbaz.sHtML

[H04] 自定义异常类型
来源：http://mobile.fehbvm.com/Article/details/gbvodhewx.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.zdbjq.cn/Article/details/gaobfhobp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.fehbvm.com/Article/details/gvylpfmxu.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gbukclkri.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gukonhfku.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.hesvh.cn/Article/details/gfcfidssq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/goikfszht.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.hesvh.cn/Article/details/gmuobcfoz.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gypahdeff.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gizidqeby.sHtML

Py:   except ValueError as e:
来源：http://m.share.hesvh.cn/Article/details/ggtmvavhn.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gayjpmmlv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gikkuoxwh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/gwfywtkct.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/gaetwwirq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.hesvh.cn/Article/details/ggipvzedh.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.blog.zdbjq.cn/Article/details/gxmuucvcz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.m.share.hesvh.cn/Article/details/guaaefrxs.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.fehbvm.com/Article/details/gcsjjrrdp.sHtML

Py:   value = d.get("k") or default
来源：http://wap.zdbjq.cn/Article/details/goailnqyo.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gygrpkwgp.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gcsyqrxno.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gfsoubray.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://m.share.zdbjq.cn/Article/details/gjrneiopu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gjcfwsunr.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.hesvh.cn/Article/details/gkdgekjpe.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gkbrqnspm.sHtML

[H07] 断言
来源：http://m.share.zdbjq.cn/Article/details/gnmmayacs.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gbruwenbs.sHtML

PHP:  assert($x > 0);
来源：http://3g.fehbvm.com/Article/details/gybhlnlce.sHtML

JS:   console.assert(x > 0);
来源：http://blog.hesvh.cn/Article/details/gwurmlmtu.sHtML

TS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gtawmxqvl.sHtML

Java: assert x > 0 : "必须为正";
来源：http://3g.hesvh.cn/Article/details/gfpfkvjha.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.share.fehbvm.com/Article/details/gvtsolkdd.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/ggoozhvjo.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gwugdesst.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.fehbvm.com/Article/details/gduasiojs.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.share.hesvh.cn/Article/details/gbvdehiiv.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.fehbvm.com/Article/details/gacwweimy.sHtML


<!-- 参考信息 -->