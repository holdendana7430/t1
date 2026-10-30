代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://wap.fehbvm.com/Article/details/gloktdgyf.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/gzdniyvxl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gnysqwssg.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gqitqmgdt.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.hesvh.cn/Article/details/gvdfrvmec.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://read.share.hesvh.cn/Article/details/gakgtmpkb.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gmagtakdr.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gwhjmkofr.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.fehbvm.com/Article/details/gxhgxqddu.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.fehbvm.com/Article/details/gkntgtaox.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gglxgecat.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gcglhmgdx.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.fehbvm.com/Article/details/gjncepspk.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/ggnzqolne.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gwcamewys.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grcnoshtj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqaglxaho.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gbxrwuhtm.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fehbvm.com/Article/details/grdxnjats.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grkndmkib.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdpjjpuxg.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gzlawyoql.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gqdwhvnsx.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/glmwqrslh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtzsbopvd.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyersjeha.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gxvrfutne.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gmlrpecjt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gpchqjtjp.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gtsyqzzey.sHtML

[F07] 创建目录（含多级）
来源：http://blog.hesvh.cn/Article/details/gkmvaomzl.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gjfzmpvbm.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.hesvh.cn/Article/details/gxejqkzcq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.zdbjq.cn/Article/details/gkysyyoqw.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.zdbjq.cn/Article/details/gkknbkduu.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.hesvh.cn/Article/details/gejoxyexp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/ggmjapkgo.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.zdbjq.cn/Article/details/gbrfjzzae.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.hesvh.cn/Article/details/gksypdvfg.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gvdfrubbn.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.zdbjq.cn/Article/details/gaqvlkvbl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gvlfdtuyx.sHtML

JS:   fs.readdirSync("dir")
来源：http://read.share.hesvh.cn/Article/details/gsqwysfgq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.fehbvm.com/Article/details/gytgyijld.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/grrofjrob.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.hesvh.cn/Article/details/ggwscpxbf.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gibwmskyc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gaiifishc.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gqhvircmy.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ghgxeqkvv.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gdjfyovgx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gilnycxng.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gtjwafjfi.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gnfnicqdn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gaunvvqdu.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/grzhijvhy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.hesvh.cn/Article/details/glxkgmbvg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.fehbvm.com/Article/details/gwvjwbluy.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gqdbrcyoo.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gkuobjnxs.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/givrzqglh.sHtML

TS:   path.extname("a.txt")
来源：http://wap.hesvh.cn/Article/details/gzxiuqzbq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gcgaolyrz.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmroegjkm.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gwysnosum.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gwooztbbp.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gbewijzls.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gtdyzmhbt.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.hesvh.cn/Article/details/gpylhlini.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gbtfufftb.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gsrkfkwkt.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvrxtuykk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gmydkgaki.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gjnrfwzla.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gauanuldm.sHtML

[F12] CSV 读写
来源：http://www.m.share.fehbvm.com/Article/details/gltohimkr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.fehbvm.com/Article/details/ggfhamivj.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gchlcfusg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.fehbvm.com/Article/details/gfrcxefft.sHtML

TS:   // 同上
来源：http://www.share.hesvh.cn/Article/details/gvxspwjax.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.hesvh.cn/Article/details/gmiamtplr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.fehbvm.com/Article/details/gptyoxcyp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.zdbjq.cn/Article/details/gzkhijzvw.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.blog.zdbjq.cn/Article/details/gaprvwash.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gjajwdotf.sHtML

G. 面向对象
来源：http://3g.fehbvm.com/Article/details/gxeaoczcu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggpdayttr.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gvjxmnqbs.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/ganampszy.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gadmfbmht.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gdyhbgbjy.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.hesvh.cn/Article/details/gicauirpq.sHtML

Java: class User {}
来源：http://www.share.fehbvm.com/Article/details/gbfwsvrkv.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.fehbvm.com/Article/details/gtumwlviw.sHtML

Ruby: class User; end
来源：http://www.m.share.zdbjq.cn/Article/details/grdimvfks.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gcymtidiy.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gkqupnezr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/ghwlctzzl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.hesvh.cn/Article/details/gxqrvxexq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gaoafpapa.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.fehbvm.com/Article/details/glukksmqc.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gzsyqlqsm.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/gdnotrymv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/grtyqykpx.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gklbjrsbo.sHtML

[G03] 实例属性
来源：http://www.m.share.fehbvm.com/Article/details/ghjpzpxuw.sHtML

Py:   self.name = "x"
来源：http://wap.hesvh.cn/Article/details/gvnkairjn.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gnqafafnw.sHtML

JS:   this.name = "x";
来源：http://www.m.share.hesvh.cn/Article/details/gabzctxvp.sHtML

TS:   name: string = "x";
来源：http://3g.hesvh.cn/Article/details/gxdtypxfy.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gusnvccqu.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.fehbvm.com/Article/details/gwmljqwab.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/gdiluiazu.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.hesvh.cn/Article/details/gsjlvwelb.sHtML

[G04] 定义方法
来源：http://read.share.fehbvm.com/Article/details/gtxuzybbd.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/guwziizpf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.fehbvm.com/Article/details/gjksrhnyi.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gdbubzbzd.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gjokthtpg.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/givuufakj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.zdbjq.cn/Article/details/gsahrmikt.sHtML

Ruby: def greet; @name; end
来源：http://www.share.hesvh.cn/Article/details/gijiggzwi.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gzgglnskk.sHtML

[G05] 继承
来源：http://baike.hesvh.cn/Article/details/gwwfniqpr.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gbshdhlwo.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/grdrmhcfm.sHtML

JS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/goweqbwfa.sHtML

TS:   class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gjwllyqdb.sHtML

Java: class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gifdgaitf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://baike.zdbjq.cn/Article/details/gyolaxmje.sHtML

Ruby: class Admin < User; end
来源：http://wap.fehbvm.com/Article/details/ghirideue.sHtML

C#:   class Admin : User {}
来源：http://baike.zdbjq.cn/Article/details/gubiznkmn.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gvffxqhvb.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/gaghqrhir.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ggirrtrkx.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gpthnlxvi.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gxkgwnagj.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdusegsky.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.hesvh.cn/Article/details/gctmotwpg.sHtML

Ruby: def greet; "admin"; end
来源：http://www.share.zdbjq.cn/Article/details/gmqxgohmb.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.m.share.zdbjq.cn/Article/details/gzdevwycf.sHtML

[G07] 调用父类方法
来源：http://baike.zdbjq.cn/Article/details/gpknrdqsw.sHtML

Py:   super().greet()
来源：http://3g.hesvh.cn/Article/details/gybpxizbz.sHtML

PHP:  parent::greet();
来源：http://read.share.hesvh.cn/Article/details/gpfnbwtdp.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gpfftsltx.sHtML

TS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gkxxgzath.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/gjfmjrvwh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gbgeoipxq.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gjsmoqdne.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gyytwlzkz.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/ggjawwbxt.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.share.hesvh.cn/Article/details/glzavnade.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gptscdrda.sHtML

JS:   static f() {}
来源：http://read.share.fehbvm.com/Article/details/gblyswxfj.sHtML

TS:   static f(): void {}
来源：http://m.share.fehbvm.com/Article/details/gfdaxhbek.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/grvqojvxo.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.hesvh.cn/Article/details/geiykulxl.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/gwmvzrpbd.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gejwiefzj.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.zdbjq.cn/Article/details/gzknldnan.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://wap.hesvh.cn/Article/details/gdfzamtwk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/groyfaenn.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gonknnedw.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gibhszzyb.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.zdbjq.cn/Article/details/glwbkahwe.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.hesvh.cn/Article/details/gjclgdcuv.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://wap.fehbvm.com/Article/details/ghvvtgnas.sHtML

C#:   interface IShape { double Area(); }
来源：http://mobile.fehbvm.com/Article/details/guijelkak.sHtML

[G10] 访问控制
来源：http://baike.hesvh.cn/Article/details/gygvfwjnp.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gmkskrciy.sHtML

PHP:  public / protected / private
来源：http://wap.hesvh.cn/Article/details/gfdedpxdk.sHtML

JS:   #private 字段；其余公开
来源：http://3g.hesvh.cn/Article/details/gdwyrmomh.sHtML

TS:   public / protected / private
来源：http://baike.fehbvm.com/Article/details/gffhafxpg.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.fehbvm.com/Article/details/gqkhsehyp.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.fehbvm.com/Article/details/ghfrpefbd.sHtML

Ruby: public / protected / private
来源：http://www.m.share.hesvh.cn/Article/details/gnzycnlwc.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.fehbvm.com/Article/details/gookiephe.sHtML

[G11] getter / setter
来源：http://www.m.share.fehbvm.com/Article/details/gogmphcxx.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.zdbjq.cn/Article/details/gtyogpyfp.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/grlskblmg.sHtML

JS:   get name() { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gwlnvcctw.sHtML

TS:   get name(): string { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/goamkosud.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gvebasiwe.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gddbqkqas.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/gmfzqbkbo.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/ggtxlylxd.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gqubitbrm.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/gjydqcoao.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gobvpfhwo.sHtML

JS:   toString() { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gchcpzhwh.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gikpknnqy.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gcvnaeprc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/gbjilecfa.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/gisatuvgj.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gayxslggh.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/gwszpsmnt.sHtML

Py:   isinstance(u, User)
来源：http://www.share.zdbjq.cn/Article/details/grjytqsyr.sHtML

PHP:  $u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gnvwzslcr.sHtML

JS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gadxysnvi.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/glsuqyejt.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gswkbhrim.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.blog.zdbjq.cn/Article/details/ghxakfjls.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/grrrpahmu.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gvcdwccdu.sHtML

[G14] 数据类 / record
来源：http://blog.zdbjq.cn/Article/details/gudqijdoe.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://mobile.fehbvm.com/Article/details/gyuccpqvl.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.blog.fehbvm.com/Article/details/goyhaxluz.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.hesvh.cn/Article/details/gkscxbbey.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.m.share.hesvh.cn/Article/details/gdlbvjbqq.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/gwmtggwcb.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/grmjkixjc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://wap.hesvh.cn/Article/details/ghvhlayly.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gmovyisdz.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gnhmxtwye.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.hesvh.cn/Article/details/gecalqzpo.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gjijigild.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.zdbjq.cn/Article/details/gwpezzptz.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gfhiekszs.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.fehbvm.com/Article/details/gcsignotj.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://mobile.zdbjq.cn/Article/details/gdznsdfnb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.fehbvm.com/Article/details/ghbwljywt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gxhtvniou.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gzrdinyrp.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.hesvh.cn/Article/details/gzxaxwasx.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.zdbjq.cn/Article/details/gqhhfwtbs.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gpxpaftxj.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gykalyuou.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/gurlwulcy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.fehbvm.com/Article/details/gamqikzpo.sHtML

Ruby: obj.instance_variables
来源：http://www.share.hesvh.cn/Article/details/gbbtizeds.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/grjcxerbj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/glrmcalhc.sHtML

H. 异常与错误处理
来源：http://wap.fehbvm.com/Article/details/ghbskuvvf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grrlqvgmd.sHtML

[H01] try / catch 基础
来源：http://m.share.hesvh.cn/Article/details/gctcnyhqs.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.share.zdbjq.cn/Article/details/gpxtpshqn.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/ghtluymnx.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/ghszcwfar.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdozceybp.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gvawykpli.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gfcnveamv.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/ggxcuouwr.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gsfgwgpwm.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gnzvncigi.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.fehbvm.com/Article/details/gusnevurg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gmimogipd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gyysuwqwm.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gduacyysv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.hesvh.cn/Article/details/gxznfoqho.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.hesvh.cn/Article/details/giiolpyvl.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.hesvh.cn/Article/details/gmtokzdcm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/gegfmxloz.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gpzfyfjdk.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.zdbjq.cn/Article/details/gxcteqocd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.fehbvm.com/Article/details/gwdsgczxk.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gawzpelxw.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.zdbjq.cn/Article/details/ggmtgmppx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gkeixfgrw.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.zdbjq.cn/Article/details/gidaamkqo.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.zdbjq.cn/Article/details/gfjwvkmnb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/griwlbzxc.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gnejksijh.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/gmmojsbtl.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://mobile.hesvh.cn/Article/details/gcedbpxwx.sHtML

JS:   class MyError extends Error {}
来源：http://wap.zdbjq.cn/Article/details/glhtigsdz.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gdzeailft.sHtML

Java: class MyException extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/gvptfkgti.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/ghadpezdu.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gesuwsoms.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gjtzaisai.sHtML

[H05] 捕获特定类型
来源：http://blog.zdbjq.cn/Article/details/gmqcneojc.sHtML

Py:   except ValueError as e:
来源：http://www.share.hesvh.cn/Article/details/gjulcupuh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.hesvh.cn/Article/details/ggbdvkwcp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gwhrjeaov.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gpiljrtaq.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://blog.zdbjq.cn/Article/details/gfwhxnzli.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.fehbvm.com/Article/details/gzmdmcyuz.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gzkilgwds.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/grwazlnok.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gylfcrhvv.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.hesvh.cn/Article/details/gbwdtmsur.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gamqinqsx.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gwzamsgoq.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/grhnjcznj.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/goxgvzdpf.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.hesvh.cn/Article/details/grokzwkoi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.fehbvm.com/Article/details/gaaebbxli.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gnkstczjx.sHtML

[H07] 断言
来源：http://blog.hesvh.cn/Article/details/genwjpycc.sHtML

Py:   assert x > 0, "必须为正"
来源：http://m.share.fehbvm.com/Article/details/glabalnfv.sHtML

PHP:  assert($x > 0);
来源：http://mobile.fehbvm.com/Article/details/gggupgorm.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/gjbeftzoo.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gvqwrkrnj.sHtML

Java: assert x > 0 : "必须为正";
来源：http://www.blog.fehbvm.com/Article/details/gywxyygun.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.hesvh.cn/Article/details/guclrvnds.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.zdbjq.cn/Article/details/gkgnsllnm.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.zdbjq.cn/Article/details/gpjjxhqde.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.zdbjq.cn/Article/details/gokjebooc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.fehbvm.com/Article/details/ghzbfczud.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.fehbvm.com/Article/details/gegrvcxuu.sHtML


<!-- 参考信息 -->