代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/gkrgvmfdv.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gdprxerxx.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gzipytdzf.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gvlxdegab.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/ggeveuylz.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/gvcgxeudu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gqcpzyqcn.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.hesvh.cn/Article/details/gurxucpvr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.fehbvm.com/Article/details/glgwhkowu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.hesvh.cn/Article/details/geaabdyjp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/ghdlrwjdx.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/gezeitdeh.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fehbvm.com/Article/details/gfgjeqwac.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fehbvm.com/Article/details/gfzumzqps.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gvewhtclw.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gifdpledg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfyafnwec.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gtdxdzzzm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.fehbvm.com/Article/details/gbfnatbzx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/geivxrdwx.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grmgzapxh.sHtML

[F06] 删除文件
来源：http://m.share.hesvh.cn/Article/details/glxnypfdq.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gyukemilh.sHtML

PHP:  unlink("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gycykbxse.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/geiecukvq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glvubjibl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gnfushgjw.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gekswflyd.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxgmgoucr.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gvnupognb.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gihpgfhfn.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/ggqjqdpgx.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gnshderun.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fehbvm.com/Article/details/ghzjuspeq.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gnrhmpcwk.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.hesvh.cn/Article/details/gencqjevh.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fehbvm.com/Article/details/gmrdwbrgu.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/gpwzxxlsu.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gmmhuavhl.sHtML

[F08] 遍历目录
来源：http://3g.hesvh.cn/Article/details/gbohquifw.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gecurciph.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gikulfibk.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gbcqhjhjn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gytzdfyqc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/grbhyqlqf.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gmcseiudh.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gsrihfbby.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.hesvh.cn/Article/details/gylualojw.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gxwuhgcww.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzwbulddk.sHtML

PHP:  filesize("a.txt");
来源：http://3g.fehbvm.com/Article/details/gybwjnihn.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/ggnglagll.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gtawssvhh.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/ghrlofjxc.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gqfgtbtek.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbmzbkpil.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/gvbexphuj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gutcvycjz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gflyavotb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gitmqnspi.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/goifuddid.sHtML

TS:   path.extname("a.txt")
来源：http://wap.fehbvm.com/Article/details/gemyvfbli.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gvuhimjgm.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gqfolxinb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gapjqklqa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnzqxwlnu.sHtML

[F11] 复制与移动文件
来源：http://www.share.fehbvm.com/Article/details/ghyqheood.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/grtwabbtd.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/gimxicszq.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/ggnnvkdof.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gpxedbsiw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gxtsxpuqk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.hesvh.cn/Article/details/gfurowxtf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gefsccpvv.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.hesvh.cn/Article/details/gujeqikhz.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/guwokbnhe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gapuireae.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gktycynow.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/gmwiayirz.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gotvunkno.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.hesvh.cn/Article/details/gsuyupadd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gtdmspmov.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gslxfkjue.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gowrqiwsz.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gknccktke.sHtML

G. 面向对象
来源：http://blog.fehbvm.com/Article/details/grauyvloo.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghnuhtylf.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gacvvkotf.sHtML

Py:   class User: pass
来源：http://www.m.share.fehbvm.com/Article/details/gshsiqdmp.sHtML

PHP:  class User {}
来源：http://3g.zdbjq.cn/Article/details/gjucpmxdo.sHtML

JS:   class User {}
来源：http://m.share.hesvh.cn/Article/details/ghsunnzgq.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.zdbjq.cn/Article/details/gsyiypxur.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gdppxvzul.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gyetnsdrz.sHtML

Ruby: class User; end
来源：http://read.share.hesvh.cn/Article/details/grrgezifm.sHtML

C#:   class User {}
来源：http://www.share.hesvh.cn/Article/details/gnxhljpwr.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/gvfonijma.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gsfyktwkm.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.hesvh.cn/Article/details/guxicwjez.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.hesvh.cn/Article/details/gznmegvsd.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.hesvh.cn/Article/details/gktdiofgl.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gwoohitof.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/gvsjhkpjm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://wap.zdbjq.cn/Article/details/govyakice.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gsdnkgvnn.sHtML

[G03] 实例属性
来源：http://baike.zdbjq.cn/Article/details/glpbqvtky.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gbrozopnm.sHtML

PHP:  public string $name = "x";
来源：http://wap.hesvh.cn/Article/details/gcmpwxbie.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gkaeftcue.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gdtfgxwxj.sHtML

Java: private String name;
来源：http://blog.fehbvm.com/Article/details/gjtddicts.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gydlfoome.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/ghvqgeqfy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gorqyjlww.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gskeziics.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.fehbvm.com/Article/details/gmzyimhzw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gprgcjsty.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gsujhmdxz.sHtML

TS:   greet(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gotobvyvn.sHtML

Java: String greet() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gtitvohnx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gkpxbknkw.sHtML

Ruby: def greet; @name; end
来源：http://3g.zdbjq.cn/Article/details/grgelzndx.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.zdbjq.cn/Article/details/gswiueewz.sHtML

[G05] 继承
来源：http://www.share.fehbvm.com/Article/details/gjijrrlbq.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.hesvh.cn/Article/details/gmdllmgrj.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gmconcydq.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gzaoocvwu.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gwihlwwnr.sHtML

Java: class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gyyghjonw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.hesvh.cn/Article/details/gekrtzlsd.sHtML

Ruby: class Admin < User; end
来源：http://mobile.zdbjq.cn/Article/details/gdplyctdf.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxwpurhyz.sHtML

[G06] 重写方法
来源：http://mobile.hesvh.cn/Article/details/guvxvacuu.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/geizdxcvu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gesqffcay.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gdpmhxtjm.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gtbvgmvjo.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/ghcbkyrjx.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gfoxdxhze.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gadlaxmpu.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.zdbjq.cn/Article/details/gisdwjmaj.sHtML

[G07] 调用父类方法
来源：http://mobile.hesvh.cn/Article/details/gefwoqdmh.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gtptxqmft.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gcvalazpy.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/gjgydhpek.sHtML

TS:   super.greet();
来源：http://wap.hesvh.cn/Article/details/galztdypt.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gylpyidcy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/gtbjqdfha.sHtML

Ruby: super
来源：http://read.share.zdbjq.cn/Article/details/gyasgohem.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gbqyfodll.sHtML

[G08] 静态方法与属性
来源：http://mobile.zdbjq.cn/Article/details/gljhfqpyw.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gsrmzwjbw.sHtML

PHP:  public static function f() {}
来源：http://www.blog.hesvh.cn/Article/details/gbwbxfcon.sHtML

JS:   static f() {}
来源：http://3g.fehbvm.com/Article/details/grjopwwah.sHtML

TS:   static f(): void {}
来源：http://www.share.zdbjq.cn/Article/details/glwtnjdmj.sHtML

Java: static void f() {}
来源：http://read.share.zdbjq.cn/Article/details/ghmkhvtxz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://baike.fehbvm.com/Article/details/gtnavnfay.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/ggvaatgjw.sHtML

C#:   public static void F() {}
来源：http://mobile.zdbjq.cn/Article/details/gqeuxltqr.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gdvvfehtv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gelxwllre.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://baike.zdbjq.cn/Article/details/gadzleyum.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gpaonxsdi.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gymhmksqa.sHtML

Java: interface Shape { double area(); }
来源：http://3g.fehbvm.com/Article/details/gutaxqoks.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/ggymljdzm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.zdbjq.cn/Article/details/gkfpseudf.sHtML

C#:   interface IShape { double Area(); }
来源：http://read.share.zdbjq.cn/Article/details/ggsxlnrnx.sHtML

[G10] 访问控制
来源：http://www.share.zdbjq.cn/Article/details/gnkbcztgb.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.zdbjq.cn/Article/details/gkymksgwe.sHtML

PHP:  public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gtcumfibs.sHtML

JS:   #private 字段；其余公开
来源：http://baike.hesvh.cn/Article/details/gxulyufqv.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/gbuzvvaav.sHtML

Java: public / protected / private / 默认包级
来源：http://3g.fehbvm.com/Article/details/gzhivevwu.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gykdzqqeb.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gqulnvhgs.sHtML

C#:   public / protected / private / internal
来源：http://read.share.zdbjq.cn/Article/details/glfyoprjl.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gtsuslvxp.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gakwfzket.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/glyqdyets.sHtML

JS:   get name() { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gqkydhqcn.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/glxjggegn.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnlhtjwxh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.hesvh.cn/Article/details/gttdmcpjh.sHtML

Ruby: attr_accessor :name
来源：http://mobile.zdbjq.cn/Article/details/graicugqq.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.zdbjq.cn/Article/details/goqkijccj.sHtML

[G12] 对象转字符串
来源：http://www.share.zdbjq.cn/Article/details/grvijvrmo.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.zdbjq.cn/Article/details/glybncerb.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/grixzduyi.sHtML

JS:   toString() { return this.name; }
来源：http://m.share.fehbvm.com/Article/details/gmhyfwhpe.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/govcnfwgn.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvhswgfvw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/guwewcxcv.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gkafcivnn.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.fehbvm.com/Article/details/gefhfrylh.sHtML

[G13] 判断对象类型
来源：http://mobile.zdbjq.cn/Article/details/grauhjudf.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.hesvh.cn/Article/details/gnhnmjrgp.sHtML

PHP:  $u instanceof User
来源：http://3g.hesvh.cn/Article/details/ggbdmfatn.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gqcotznje.sHtML

TS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/gzjgohlgd.sHtML

Java: u instanceof User
来源：http://m.share.hesvh.cn/Article/details/ganquklht.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.hesvh.cn/Article/details/gigpphroi.sHtML

Ruby: u.is_a?(User)
来源：http://blog.hesvh.cn/Article/details/gtlvagnzy.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/golujtptl.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gspdxtniw.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.fehbvm.com/Article/details/gmglcdpkw.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.fehbvm.com/Article/details/gybkajgqz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.hesvh.cn/Article/details/gccabygdj.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.fehbvm.com/Article/details/galudhayc.sHtML

Java: record User(String name, int age) {}
来源：http://www.share.fehbvm.com/Article/details/gabokudfm.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/ghrgplxxo.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.fehbvm.com/Article/details/grfzgyqen.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.fehbvm.com/Article/details/gahoasyvd.sHtML

[G15] 枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gsekfadws.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.hesvh.cn/Article/details/gvvifutbl.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.fehbvm.com/Article/details/gzequzimz.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.share.hesvh.cn/Article/details/gxfsehsuu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gdojtenye.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.zdbjq.cn/Article/details/gecyuleha.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/gxpuusobc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gkgmxkavu.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.fehbvm.com/Article/details/gilbkewda.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.fehbvm.com/Article/details/gxxqpiwwg.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.zdbjq.cn/Article/details/glfsuhqru.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gejbuqiyr.sHtML

JS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/geqbgjxha.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gwxxgnwow.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gloiicync.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.fehbvm.com/Article/details/gnjdlxriw.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gjorecroj.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.fehbvm.com/Article/details/gneppdipp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpyzaltqn.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gdwcaeqbz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/geedpqszb.sHtML

[H01] try / catch 基础
来源：http://3g.fehbvm.com/Article/details/gojadfagr.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gbrzaymjs.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://read.share.fehbvm.com/Article/details/gqkrwolve.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gacywzgyt.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/grqcekvtp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.zdbjq.cn/Article/details/gtwhzieuk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gcoiubnma.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://mobile.fehbvm.com/Article/details/gptacleay.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gbhcussyu.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.fehbvm.com/Article/details/gsqdcrffo.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://mobile.zdbjq.cn/Article/details/gqyazelni.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/ghbwwmtgf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwvnytzbe.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/glhegceha.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/glsyntexn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.hesvh.cn/Article/details/golgbyxdm.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.m.share.fehbvm.com/Article/details/gzcfntvxj.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gwwxejbwk.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gykkntsku.sHtML

Py:   raise ValueError("错误信息")
来源：http://3g.hesvh.cn/Article/details/gubngxfkf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.fehbvm.com/Article/details/gurdwssja.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gpktbmkez.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/gecwklmko.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gviobmthq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.share.hesvh.cn/Article/details/gqraqlnaf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.fehbvm.com/Article/details/gsoyefwyh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/glxsoulic.sHtML

[H04] 自定义异常类型
来源：http://baike.zdbjq.cn/Article/details/gpavwbdiz.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gmtexcpua.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/geocfyseu.sHtML

JS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gnwpgfahb.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gsgauzsrn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://m.share.zdbjq.cn/Article/details/glrwinkbl.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gitxqezbx.sHtML

Ruby: class MyError < StandardError; end
来源：http://read.share.hesvh.cn/Article/details/gkbimcswt.sHtML

C#:   class MyException : Exception {}
来源：http://blog.hesvh.cn/Article/details/gkgqvdrpd.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/glbhoiekg.sHtML

Py:   except ValueError as e:
来源：http://3g.hesvh.cn/Article/details/gjswqghfc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/gaqsfeyhi.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/ggxzgqndj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.hesvh.cn/Article/details/ghjohaxbi.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/glcvcanlo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/glxcfhlcs.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.fehbvm.com/Article/details/gknrqqqym.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gpdldfyba.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gsdzgirzm.sHtML

Py:   value = d.get("k") or default
来源：http://www.blog.hesvh.cn/Article/details/gufywglgr.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/ggfjpzrbl.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.zdbjq.cn/Article/details/gowutwfsf.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/glbxfxxzk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gnngnzdlu.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://m.share.zdbjq.cn/Article/details/gfjkfphxo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gujbftdbg.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.fehbvm.com/Article/details/gtrxbnhbw.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/gvjaxfocy.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.zdbjq.cn/Article/details/gcfqbwjwy.sHtML

PHP:  assert($x > 0);
来源：http://m.share.fehbvm.com/Article/details/gzlbcqwrs.sHtML

JS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gnjmyaxod.sHtML

TS:   console.assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gimcjzxgp.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.hesvh.cn/Article/details/gbwnvohtk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.hesvh.cn/Article/details/grsktpcbr.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.hesvh.cn/Article/details/gllhsjwou.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gwqmhwivj.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.zdbjq.cn/Article/details/gclhtrjnv.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.m.share.fehbvm.com/Article/details/glewztouc.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://wap.fehbvm.com/Article/details/gnpdercxu.sHtML


<!-- 参考信息 -->