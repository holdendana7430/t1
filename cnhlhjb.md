代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.share.zdbjq.cn/Article/details/gfhrphnkn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/glfyyftdv.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.zdbjq.cn/Article/details/grkktptfw.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gastqfdmc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gonfwgwlq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/ghdkpdsoc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gyehdehuj.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gjnfqrmwv.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.zdbjq.cn/Article/details/gqatfixay.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gtybkaiqe.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gykwrgvrr.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gwkswwuqo.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/gputhvlgq.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gilfngrzh.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gmawrcwcg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/giniiqiat.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gyenaitmg.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gyucgvxnm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gcfovapap.sHtML

Ruby: File.exist?("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcxjkpbje.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grnykrrry.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/ggwepzxne.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gvgnpeyig.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gxzfhijyy.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gxfdtcyat.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsyqpwgtb.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gvqmzcfsd.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gewzkhnrn.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/glegwcxmi.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gqahpylyf.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gsccahfbi.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gjaucixsv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.zdbjq.cn/Article/details/gurfhxsna.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gokuciiwm.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.fehbvm.com/Article/details/gqgzrelmj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gguvempmb.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.fehbvm.com/Article/details/gwomiyvgk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gddcijdku.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.zdbjq.cn/Article/details/gwkdbhsnp.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gqjyblheq.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gavvjsyac.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gjdxitfpq.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/ggmvvwnsm.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gspatwnjq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gxsqvfcgt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://blog.fehbvm.com/Article/details/gypsoxkjh.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gvrcxmanu.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.zdbjq.cn/Article/details/gljooqjbc.sHtML

[F09] 获取文件大小
来源：http://www.m.share.zdbjq.cn/Article/details/gozuhlwvq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gggmbmxoz.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/ggculygrs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gtbvumzdx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/gvxjjipuj.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/giqvapfgh.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.hesvh.cn/Article/details/gupxjbwqu.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/granjxkcu.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.zdbjq.cn/Article/details/gfdyoywuh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gherkxdku.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjmtahqrt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gphsehdip.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gjajvnamx.sHtML

TS:   path.extname("a.txt")
来源：http://blog.fehbvm.com/Article/details/gcoxfyewv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.fehbvm.com/Article/details/gqkiembkh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gcptxarlk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfgfsbqzn.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gakigwhtu.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/gcdbndhea.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gauogchtm.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gtbelypho.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gigqxoqgh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gnxyryjml.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.fehbvm.com/Article/details/glxkwnvxq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gkzejhrug.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gvivtbjas.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.fehbvm.com/Article/details/gmbreehsa.sHtML

[F12] CSV 读写
来源：http://wap.fehbvm.com/Article/details/gopkbpihv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://wap.zdbjq.cn/Article/details/gncyyjuwg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gcsxuqfqq.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.fehbvm.com/Article/details/gikpylmda.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gesthblkl.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fehbvm.com/Article/details/ggtivntfp.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/ghzojafco.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.hesvh.cn/Article/details/grotualdx.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.hesvh.cn/Article/details/gqekrypuj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/glkigrbtt.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/grpywrffn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzgvtfcqp.sHtML

[G01] 定义类
来源：http://blog.fehbvm.com/Article/details/gobloowcn.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gnzryxpxl.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gmvkluzad.sHtML

JS:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gyfsbeblk.sHtML

TS:   class User { name: string = ""; }
来源：http://www.share.fehbvm.com/Article/details/grxxgyjef.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/ggpqckhxx.sHtML

Go:   type User struct { Name string }
来源：http://baike.zdbjq.cn/Article/details/glglvhmkg.sHtML

Ruby: class User; end
来源：http://3g.fehbvm.com/Article/details/glmyzcwno.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gfohxpmqo.sHtML

[G02] 构造函数
来源：http://3g.fehbvm.com/Article/details/glndtcsnf.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.blog.fehbvm.com/Article/details/gokqhbufn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.hesvh.cn/Article/details/gkyhaatdk.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gthqkqsrl.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gnpuvinut.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/glbanflhw.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.zdbjq.cn/Article/details/gxsvavfdz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.hesvh.cn/Article/details/gwgqbspfb.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/glnvlewzl.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gobakyiix.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gcnpmuaya.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gzvbsiqaq.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gunepaqzo.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gmgbtiihz.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/gsqzxdxho.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gfoiqenkg.sHtML

Ruby: @name = "x"
来源：http://wap.hesvh.cn/Article/details/ggkrdluql.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/grlaxadpi.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gkwvzwfsq.sHtML

Py:   def greet(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/gorlfuiui.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gpfdewbof.sHtML

JS:   greet() { return this.name; }
来源：http://3g.fehbvm.com/Article/details/giwmhwmdn.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gshvrcwbr.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gqhualmio.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gzhogihky.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gjodafdon.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.zdbjq.cn/Article/details/gbecvjjwn.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gzspezvpl.sHtML

Py:   class Admin(User): pass
来源：http://m.share.fehbvm.com/Article/details/ggbqoihjj.sHtML

PHP:  class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gxxixajie.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gnuxcqrfq.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gvmhebosl.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gzctpwjtp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.hesvh.cn/Article/details/gttdrvedo.sHtML

Ruby: class Admin < User; end
来源：http://m.share.zdbjq.cn/Article/details/gaywclpsx.sHtML

C#:   class Admin : User {}
来源：http://www.m.share.hesvh.cn/Article/details/gkezuetqe.sHtML

[G06] 重写方法
来源：http://baike.hesvh.cn/Article/details/gxrheuioi.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.hesvh.cn/Article/details/gtfijmqzu.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gqziiwsrh.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gmuychjqj.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gzzlsdqxc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gvlrsuszw.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.blog.hesvh.cn/Article/details/gpxjqlzlx.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gpyibugty.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.hesvh.cn/Article/details/gtxsfdwqv.sHtML

[G07] 调用父类方法
来源：http://3g.hesvh.cn/Article/details/ghqctfghq.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/ggfckcqjf.sHtML

PHP:  parent::greet();
来源：http://wap.hesvh.cn/Article/details/gcbxvbqxg.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/goqprlepi.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gkleelskg.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gyhkfuhmy.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.blog.fehbvm.com/Article/details/gqscbhgpm.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gwldyifai.sHtML

C#:   base.Greet();
来源：http://www.share.zdbjq.cn/Article/details/gkbdcqgud.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/geqbutmeu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.hesvh.cn/Article/details/gyuwnejrw.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gjgpnzpbz.sHtML

JS:   static f() {}
来源：http://mobile.zdbjq.cn/Article/details/gyekgcjlk.sHtML

TS:   static f(): void {}
来源：http://mobile.hesvh.cn/Article/details/gxilvgbdi.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gmnglqkyk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/gbrkrxdaq.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gadjzfmxf.sHtML

C#:   public static void F() {}
来源：http://www.blog.fehbvm.com/Article/details/goctpgjms.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gaebxsbjj.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.zdbjq.cn/Article/details/gjikmyqui.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.fehbvm.com/Article/details/gclqwvvbs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gqogosfka.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbkuninad.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gpczakbbz.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gpfzacsjp.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.zdbjq.cn/Article/details/gjsknxsws.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.fehbvm.com/Article/details/gkinjhktm.sHtML

[G10] 访问控制
来源：http://mobile.fehbvm.com/Article/details/gispzhtgg.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://blog.zdbjq.cn/Article/details/gerdjcmed.sHtML

PHP:  public / protected / private
来源：http://baike.zdbjq.cn/Article/details/ghzvsgkfw.sHtML

JS:   #private 字段；其余公开
来源：http://3g.fehbvm.com/Article/details/gpdicbifu.sHtML

TS:   public / protected / private
来源：http://mobile.hesvh.cn/Article/details/gmknbrhiv.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.hesvh.cn/Article/details/gqqppjtvv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.hesvh.cn/Article/details/ghbbfcgjm.sHtML

Ruby: public / protected / private
来源：http://baike.hesvh.cn/Article/details/gctctelpl.sHtML

C#:   public / protected / private / internal
来源：http://www.share.zdbjq.cn/Article/details/ggvrboggy.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gxyzlgwfd.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gvhuowixq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.zdbjq.cn/Article/details/gkdurksgf.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/ggkowqkrb.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.hesvh.cn/Article/details/gixxgofvr.sHtML

Java: public String getName() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gbpjlnsdw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gefwdggug.sHtML

Ruby: attr_accessor :name
来源：http://baike.hesvh.cn/Article/details/ghsyhwnrv.sHtML

C#:   public string Name { get; set; }
来源：http://baike.zdbjq.cn/Article/details/gjopfyska.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gijbezeab.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gxnwgwoym.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gujaxiwce.sHtML

JS:   toString() { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gcxdsuiak.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gtpvxzilv.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gruqyrchc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/guurbitvo.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gycuitmrj.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.zdbjq.cn/Article/details/gcitrlfze.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gkuxhyvgk.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gkwhzulmt.sHtML

PHP:  $u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gpxqpijtb.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gtjtmkqou.sHtML

TS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gbzvtrsjy.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/govzzhluu.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/giaponaah.sHtML

Ruby: u.is_a?(User)
来源：http://blog.fehbvm.com/Article/details/gwtqoexrk.sHtML

C#:   u is User
来源：http://m.share.hesvh.cn/Article/details/ghadzunvs.sHtML

[G14] 数据类 / record
来源：http://m.share.zdbjq.cn/Article/details/gwkmgwvia.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.hesvh.cn/Article/details/gzffyyfyq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gyntunqya.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gcoofvqqe.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/golxlxmta.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gdpkagemt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.fehbvm.com/Article/details/ghfvtubtd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.zdbjq.cn/Article/details/gztptzvlm.sHtML

C#:   record User(string Name, int Age);
来源：http://www.blog.hesvh.cn/Article/details/geuullybk.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gxkyoguzx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://read.share.zdbjq.cn/Article/details/grkkgubyi.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gbtvrrzof.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gfvunplux.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbhmozjzq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gxvoxufvt.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://blog.fehbvm.com/Article/details/gszpazrwj.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gneluaavq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/garzbjfyh.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.zdbjq.cn/Article/details/gyogakeiq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://read.share.zdbjq.cn/Article/details/gnyzcsvdu.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.zdbjq.cn/Article/details/gsjvdvhah.sHtML

JS:   Object.entries(obj)
来源：http://blog.zdbjq.cn/Article/details/gnizpndqk.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gixrkodzn.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.zdbjq.cn/Article/details/ggzjzxtxt.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.hesvh.cn/Article/details/gsrshsaff.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.fehbvm.com/Article/details/gfhcbsdne.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gmtheqqnb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcewydkhw.sHtML

H. 异常与错误处理
来源：http://read.share.zdbjq.cn/Article/details/gzatiewsb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggzxposcl.sHtML

[H01] try / catch 基础
来源：http://blog.fehbvm.com/Article/details/gzrgxyyrx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/geagtlzmx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gnkqklcym.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gzboipafc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gdpyxtkbr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://baike.fehbvm.com/Article/details/gcuqruoyk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gzqdkxehu.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gfgfhpqdf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.hesvh.cn/Article/details/gprkorhcg.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.hesvh.cn/Article/details/gzvqkvomi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gfbjvdaoi.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.zdbjq.cn/Article/details/gxxtddnvs.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.hesvh.cn/Article/details/ghwymindw.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gmxrxyxkt.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/geprnqgxs.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gzsqgeuxk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gobdarfpl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gneczivwt.sHtML

[H03] 主动抛出异常
来源：http://3g.hesvh.cn/Article/details/gafsqgzno.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.blog.zdbjq.cn/Article/details/gobkyssbt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/glpejdlgm.sHtML

JS:   throw new Error("错误信息");
来源：http://www.m.share.hesvh.cn/Article/details/ggpjopwqi.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gsuekgtzy.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/gsjebmbrr.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/govazpplc.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://wap.zdbjq.cn/Article/details/gsuxjxetf.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gxwkkufmf.sHtML

[H04] 自定义异常类型
来源：http://wap.hesvh.cn/Article/details/gzquddwgy.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.hesvh.cn/Article/details/gibnhxqzy.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gmhwakeie.sHtML

JS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gzcefiypv.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.fehbvm.com/Article/details/gijflrcrn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://3g.zdbjq.cn/Article/details/gpedrrogk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://wap.hesvh.cn/Article/details/gjgxzukvn.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/giiosrmgy.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/garikjbix.sHtML

[H05] 捕获特定类型
来源：http://www.share.zdbjq.cn/Article/details/ghxfzyvmo.sHtML

Py:   except ValueError as e:
来源：http://www.blog.zdbjq.cn/Article/details/gefnhjvzm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.fehbvm.com/Article/details/gkagkynkv.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/ghzhvryrx.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.fehbvm.com/Article/details/gqotqwvzv.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/gfixpoqac.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://wap.hesvh.cn/Article/details/gomezebea.sHtML

Ruby: rescue ArgumentError => e
来源：http://blog.hesvh.cn/Article/details/gnhauwbyv.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.hesvh.cn/Article/details/gwbzgnwzh.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.hesvh.cn/Article/details/gpgpfcgfj.sHtML

Py:   value = d.get("k") or default
来源：http://mobile.hesvh.cn/Article/details/gjpmwsxxy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/gjpvuuehz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gsnrvuuxk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/gfhiemsco.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.blog.hesvh.cn/Article/details/gwalyadxf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.zdbjq.cn/Article/details/gjjmzkvpc.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gcxhjtjtd.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.zdbjq.cn/Article/details/gupnjrbir.sHtML

[H07] 断言
来源：http://www.share.zdbjq.cn/Article/details/gviclvtxt.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/gjwdbxqht.sHtML

PHP:  assert($x > 0);
来源：http://baike.zdbjq.cn/Article/details/gecnrwpgm.sHtML

JS:   console.assert(x > 0);
来源：http://baike.zdbjq.cn/Article/details/grthdlcqd.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gkzdxkwoc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.hesvh.cn/Article/details/gqxddflrb.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://3g.hesvh.cn/Article/details/ghijbscdf.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.hesvh.cn/Article/details/gzzohqmpm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://read.share.zdbjq.cn/Article/details/gdilgzpob.sHtML

[H08] 获取错误信息与堆栈
来源：http://read.share.hesvh.cn/Article/details/gzzrcutys.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://www.blog.zdbjq.cn/Article/details/gxdyezbxo.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gzuaqynre.sHtML


<!-- 参考信息 -->