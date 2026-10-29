代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.zdbjq.cn/Article/details/gnocxzwjp.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gwtsqnooi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gbcwxbzya.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gvqgvhidf.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gcepbuqcx.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fehbvm.com/Article/details/gsdeeebni.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/gehmncgbz.sHtML

[F04] 追加写入文件
来源：http://www.share.hesvh.cn/Article/details/gxbwldokl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gubpzyalt.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.fehbvm.com/Article/details/govxtfbsc.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gbrtmopxm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.hesvh.cn/Article/details/gxbltzjbj.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gnpqkmied.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.hesvh.cn/Article/details/gzffsflvh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gtubcgnvw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.hesvh.cn/Article/details/gpauzpcpk.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gvvvvbwfp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.fehbvm.com/Article/details/ggqsewgyz.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.zdbjq.cn/Article/details/glonmucbx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gaxztzfhh.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gbujdkmlr.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gqpywnuqt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gqhvuexmg.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/glautrmvv.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvulxgntm.sHtML

[F06] 删除文件
来源：http://m.share.zdbjq.cn/Article/details/gnqjmghih.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxmdwlisq.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gohzkudrz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/guglhkwcp.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gmgwezpsx.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gprfnjcih.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gqllizjzt.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gkwnljbqb.sHtML

C#:   File.Delete("a.txt");
来源：http://blog.fehbvm.com/Article/details/gozrjaaur.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.hesvh.cn/Article/details/geyxyvrzz.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.fehbvm.com/Article/details/ggjtjmxnr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gkajyqvpi.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gmjoblham.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://wap.fehbvm.com/Article/details/goqhwxtxh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/gzynznubd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gwwpgcjuc.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gzgurlzyw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.share.zdbjq.cn/Article/details/gfafybufl.sHtML

[F08] 遍历目录
来源：http://read.share.zdbjq.cn/Article/details/gsbmpcudx.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.hesvh.cn/Article/details/ggkpmstis.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.hesvh.cn/Article/details/gnupwgvdl.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/grsoxiaqt.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/glxyzevya.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/ggqvafauz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gzdxiapny.sHtML

Ruby: Dir.children("dir")
来源：http://3g.hesvh.cn/Article/details/gshqfvawk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gimvmbjak.sHtML

[F09] 获取文件大小
来源：http://baike.zdbjq.cn/Article/details/gwimogmbs.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gbsraokfy.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gwkipjzgq.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.blog.zdbjq.cn/Article/details/gtbxtoaai.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gsuoajwky.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gfjmuhszm.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/grchwvnud.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmglpoeql.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gulkdgkyg.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gmdtqxrhq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gblxliqiz.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/grggatjny.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcihzksgd.sHtML

TS:   path.extname("a.txt")
来源：http://3g.fehbvm.com/Article/details/gfxqhmmbj.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gdisgvsuv.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gktiijjpn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gjobebqhd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gjpvhidhj.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gnodgdfrv.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gprbeqizc.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.zdbjq.cn/Article/details/grqstbaad.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/goepueuhw.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gzjsoplmg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gqdxezzer.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gbzkbzjva.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gnuhemywn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gkzrxlsmh.sHtML

[F12] CSV 读写
来源：http://www.share.zdbjq.cn/Article/details/gguupuwqd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gusillmxg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.zdbjq.cn/Article/details/gyrkaikvx.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.hesvh.cn/Article/details/ggmqeyqod.sHtML

TS:   // 同上
来源：http://www.m.share.hesvh.cn/Article/details/grxktucct.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.zdbjq.cn/Article/details/ghchwaalo.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.hesvh.cn/Article/details/gdnsvedrg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.hesvh.cn/Article/details/gfrblwian.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.fehbvm.com/Article/details/gsbfxtxda.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gudtpubvm.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gprddfikp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfxnvzdin.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/ggbruskcw.sHtML

Py:   class User: pass
来源：http://m.share.zdbjq.cn/Article/details/gtclfrfxg.sHtML

PHP:  class User {}
来源：http://read.share.fehbvm.com/Article/details/gpvwmcpgx.sHtML

JS:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gpisxsols.sHtML

TS:   class User { name: string = ""; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggkohaoto.sHtML

Java: class User {}
来源：http://www.m.share.hesvh.cn/Article/details/geluhadij.sHtML

Go:   type User struct { Name string }
来源：http://baike.hesvh.cn/Article/details/gyvzibwlu.sHtML

Ruby: class User; end
来源：http://www.share.fehbvm.com/Article/details/giafhivsw.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gpbjpzlij.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gayzkogms.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://mobile.hesvh.cn/Article/details/gccrpwetf.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.zdbjq.cn/Article/details/gdqhqxsvj.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/guxhzzyfh.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.hesvh.cn/Article/details/gnxjnsnts.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gpojytgxl.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gucgtjhtq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gxgyaxtsp.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/gjvfadtxm.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gykkolxwj.sHtML

Py:   self.name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gvvvyqlgs.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gkbfwnllh.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gkxtpfvpv.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gdmzqzmvy.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/ggwwyojkj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.share.hesvh.cn/Article/details/gnkvwhmss.sHtML

Ruby: @name = "x"
来源：http://m.share.hesvh.cn/Article/details/gdnlfvwan.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gfyglvege.sHtML

[G04] 定义方法
来源：http://blog.fehbvm.com/Article/details/glxhlxpae.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gstirdnsh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gyrpbxuxy.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gvonqsxmp.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gjqqozwpn.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gdimxqvsv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/guhvbdrwt.sHtML

Ruby: def greet; @name; end
来源：http://baike.hesvh.cn/Article/details/gkkjmgkqc.sHtML

C#:   public string Greet() => Name;
来源：http://baike.fehbvm.com/Article/details/gctobwcfj.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gnxrpiypz.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gfhvdegqu.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/glqgojmtj.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gshffgqfx.sHtML

TS:   class Admin extends User {}
来源：http://blog.hesvh.cn/Article/details/gxfmzyumb.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gjdicbxpg.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.zdbjq.cn/Article/details/gozikqckt.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gdubhupaj.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/gyplguofe.sHtML

[G06] 重写方法
来源：http://blog.fehbvm.com/Article/details/gejkozjwn.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/guawvqvit.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gotzbvtcu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/ghvveekaw.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjluomnqg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gpaknurtb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/genuwsqgf.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gsxhiksuo.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gvxqcerph.sHtML

[G07] 调用父类方法
来源：http://wap.hesvh.cn/Article/details/gfkxiwhhx.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gbrqxtgng.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/gyidyezpt.sHtML

JS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/grwrabqyh.sHtML

TS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gozvwgqwt.sHtML

Java: super.greet();
来源：http://wap.hesvh.cn/Article/details/gvtzapfxt.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.fehbvm.com/Article/details/gvvreilch.sHtML

Ruby: super
来源：http://read.share.fehbvm.com/Article/details/gwxovzikw.sHtML

C#:   base.Greet();
来源：http://baike.hesvh.cn/Article/details/gjipfrswu.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gszgcqflb.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.fehbvm.com/Article/details/gdcjovgii.sHtML

PHP:  public static function f() {}
来源：http://baike.hesvh.cn/Article/details/gmbwwssra.sHtML

JS:   static f() {}
来源：http://www.m.share.fehbvm.com/Article/details/grdvcvutx.sHtML

TS:   static f(): void {}
来源：http://blog.fehbvm.com/Article/details/guaouleqs.sHtML

Java: static void f() {}
来源：http://baike.zdbjq.cn/Article/details/gurglmjpu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gdofltssv.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gryyzqysb.sHtML

C#:   public static void F() {}
来源：http://read.share.zdbjq.cn/Article/details/gsepfzbap.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.zdbjq.cn/Article/details/gcgedfnev.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/glcntbsid.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/grklebtuf.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://read.share.hesvh.cn/Article/details/ghblsnwex.sHtML

TS:   interface Shape { area(): number; }
来源：http://read.share.hesvh.cn/Article/details/gmqmnsfle.sHtML

Java: interface Shape { double area(); }
来源：http://blog.fehbvm.com/Article/details/gkpibjzyu.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gbusrkmvm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.share.zdbjq.cn/Article/details/gbiglzlqn.sHtML

C#:   interface IShape { double Area(); }
来源：http://baike.fehbvm.com/Article/details/gdchvhgeg.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gnpsazgmc.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.fehbvm.com/Article/details/gjghbksdh.sHtML

PHP:  public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gvbzhjsln.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gfutwlgnc.sHtML

TS:   public / protected / private
来源：http://mobile.fehbvm.com/Article/details/goskbqald.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gvijmeodg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gzmjpmecw.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/gncwaaxhm.sHtML

C#:   public / protected / private / internal
来源：http://m.share.fehbvm.com/Article/details/gvqueqzvi.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/goejxtyvv.sHtML

Py:   @property 与 @x.setter
来源：http://3g.fehbvm.com/Article/details/gstafyaid.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gtmqdumdz.sHtML

JS:   get name() { return this._name; }
来源：http://3g.fehbvm.com/Article/details/ggipinkao.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.hesvh.cn/Article/details/gbdhgicbs.sHtML

Java: public String getName() { return name; }
来源：http://mobile.hesvh.cn/Article/details/gydrarouo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gujipyzmp.sHtML

Ruby: attr_accessor :name
来源：http://blog.fehbvm.com/Article/details/gbyftdwlm.sHtML

C#:   public string Name { get; set; }
来源：http://blog.fehbvm.com/Article/details/gnzuhslht.sHtML

[G12] 对象转字符串
来源：http://m.share.fehbvm.com/Article/details/gqcmapbmn.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/ggmuqdqlq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gnmjaytwt.sHtML

JS:   toString() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gkhzdfedm.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gthlhqlay.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/gnrhzhwfz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gbddhixgq.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.hesvh.cn/Article/details/gilohqotb.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.fehbvm.com/Article/details/ghlicrgfv.sHtML

[G13] 判断对象类型
来源：http://m.share.fehbvm.com/Article/details/geytfxiso.sHtML

Py:   isinstance(u, User)
来源：http://baike.fehbvm.com/Article/details/gyjxxjtph.sHtML

PHP:  $u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/giafbdjlk.sHtML

JS:   u instanceof User
来源：http://wap.hesvh.cn/Article/details/gromqvcrt.sHtML

TS:   u instanceof User
来源：http://baike.hesvh.cn/Article/details/gelvykqse.sHtML

Java: u instanceof User
来源：http://read.share.hesvh.cn/Article/details/gbrszlqas.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.hesvh.cn/Article/details/godbikgbf.sHtML

Ruby: u.is_a?(User)
来源：http://wap.fehbvm.com/Article/details/gxauloqtu.sHtML

C#:   u is User
来源：http://3g.fehbvm.com/Article/details/gekfwavdo.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gigfagkcs.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gsurpnvnc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://3g.hesvh.cn/Article/details/gzkyiartj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gykfqhdgq.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.zdbjq.cn/Article/details/gnhvovimr.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.fehbvm.com/Article/details/gepfnmiis.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gtmgtreuv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gsjmrpriq.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/givbmdylj.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gvoiipshl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://mobile.zdbjq.cn/Article/details/gpheksohu.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.hesvh.cn/Article/details/gdhjlckhw.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.hesvh.cn/Article/details/gzxmcdzae.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/gbnusbaqs.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.fehbvm.com/Article/details/ggtutfzlw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.fehbvm.com/Article/details/gslgqpwyq.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/gahxcdtln.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.zdbjq.cn/Article/details/ghaqajhqj.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.hesvh.cn/Article/details/gzsbmzivf.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.blog.hesvh.cn/Article/details/gunhtznki.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gesrxahms.sHtML

JS:   Object.entries(obj)
来源：http://3g.fehbvm.com/Article/details/gazwmshub.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gnoussmip.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.zdbjq.cn/Article/details/gdaseprul.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.share.zdbjq.cn/Article/details/garvxtlet.sHtML

Ruby: obj.instance_variables
来源：http://mobile.hesvh.cn/Article/details/gnwilbsux.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.hesvh.cn/Article/details/guemhweub.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmnemudwm.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gsdkymrgp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmcbmdatm.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/gvywtmrkq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://3g.fehbvm.com/Article/details/gsdrebwqm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/glzivownr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gkuisvexe.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/grectaoim.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://mobile.hesvh.cn/Article/details/gzovgszqe.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gozwivfzj.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.zdbjq.cn/Article/details/gyiopsgjl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.zdbjq.cn/Article/details/gnzkmjmpj.sHtML

[H02] finally / ensure 收尾
来源：http://blog.zdbjq.cn/Article/details/guqgxgefj.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.fehbvm.com/Article/details/gkdvudxfl.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gpckaccis.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gcmkmwzzd.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gkigsxcwv.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/giepxznds.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/gneumlrvg.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gsotlempc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gseywrpkm.sHtML

[H03] 主动抛出异常
来源：http://wap.zdbjq.cn/Article/details/gnshqfqgs.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/guwplhbdj.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gdfdosjte.sHtML

JS:   throw new Error("错误信息");
来源：http://baike.fehbvm.com/Article/details/geavnrzld.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gqskivwub.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.hesvh.cn/Article/details/giigyzcic.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gcxhjhuhf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gesnvadkb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/grxsozfny.sHtML

[H04] 自定义异常类型
来源：http://www.share.zdbjq.cn/Article/details/gswzayxva.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.zdbjq.cn/Article/details/gtopjwfao.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.fehbvm.com/Article/details/gmhxmjkjr.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gpdutvqyj.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.hesvh.cn/Article/details/gllkeexxp.sHtML

Java: class MyException extends RuntimeException {}
来源：http://mobile.zdbjq.cn/Article/details/guzfinkvp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gqmqjuhru.sHtML

Ruby: class MyError < StandardError; end
来源：http://baike.fehbvm.com/Article/details/gkfdlhyyl.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.hesvh.cn/Article/details/ghvujuefk.sHtML

[H05] 捕获特定类型
来源：http://read.share.hesvh.cn/Article/details/gtsixtoof.sHtML

Py:   except ValueError as e:
来源：http://wap.fehbvm.com/Article/details/gehdssivg.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gcolnewwp.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gklrzegsw.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.zdbjq.cn/Article/details/gkwesdjxa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.hesvh.cn/Article/details/goovghrzi.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.share.hesvh.cn/Article/details/gjdpgxdza.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gpkjirlzh.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.zdbjq.cn/Article/details/gbodhwwlt.sHtML

[H06] 可选值 / 空值安全访问
来源：http://3g.zdbjq.cn/Article/details/gjajogifx.sHtML

Py:   value = d.get("k") or default
来源：http://blog.hesvh.cn/Article/details/gtmhpfawk.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.fehbvm.com/Article/details/goyupffkb.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/gqhojiaxw.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/ghizpxjjr.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.zdbjq.cn/Article/details/ghgbxxiid.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://3g.fehbvm.com/Article/details/geqteweaa.sHtML

Ruby: d&.dig(:a, :b)
来源：http://3g.hesvh.cn/Article/details/gzqxxbbzt.sHtML

C#:   obj?.A?.B ?? default
来源：http://m.share.fehbvm.com/Article/details/gbflnyorr.sHtML

[H07] 断言
来源：http://read.share.hesvh.cn/Article/details/ghraxjrpo.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gdqdfwssa.sHtML

PHP:  assert($x > 0);
来源：http://www.m.share.hesvh.cn/Article/details/grpxqnvpr.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gqprisvfl.sHtML

TS:   console.assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gfzzdxsxd.sHtML

Java: assert x > 0 : "必须为正";
来源：http://m.share.fehbvm.com/Article/details/gkdwdilco.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gesrgdcnl.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://read.share.fehbvm.com/Article/details/gxroqzzku.sHtML


<!-- 参考信息 -->