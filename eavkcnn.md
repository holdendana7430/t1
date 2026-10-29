代发 wailian999

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gsaulfknc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gqizmcyfd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/gececprwb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gaisffwsx.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gkxhbfvae.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gnowlkkiu.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gwwjrsiuv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gtdvptowm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gtjxmryvj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/grilgsbli.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gibejytvr.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gmqiipaeu.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grfqwamkw.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gnqagsqol.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkrwurhea.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gavomueka.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gfwwnfqgo.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gknqgpocr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gdqfzrcpm.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gnxixqtvf.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gysxnzohu.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/geqqzhasr.sHtML

[F07] 创建目录（含多级）
来源：http://baike.hesvh.cn/Article/details/gjpsudfgw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gilqoxhfc.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.fehbvm.com/Article/details/gnmioihgn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gcrbwhxql.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gjtftseyd.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.zdbjq.cn/Article/details/gaxfuosts.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gbgmsvset.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gvifsvdrf.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gaobxvuka.sHtML

[F08] 遍历目录
来源：http://www.blog.zdbjq.cn/Article/details/gffhmwodg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/gilidjwxx.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gbigutxcp.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gedigbbvk.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gzadopglp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/gxrqpjhfa.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gokomtrqb.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gqzpwxofh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.fehbvm.com/Article/details/gnlfifzkz.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gmaytifnq.sHtML

Py:   os.path.getsize("a.txt")
来源：http://wap.fehbvm.com/Article/details/gvdhcvkvx.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gmhcrwmkf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gtrlluphh.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gwqyfpbju.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/glkhsowho.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://read.share.zdbjq.cn/Article/details/gefcwpytm.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gbkfrubau.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gsjxmiake.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gxjhqfeqh.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gleppscsw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://3g.hesvh.cn/Article/details/gahezvrnl.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gcuexwoai.sHtML

TS:   path.extname("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gvpprvmyi.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.hesvh.cn/Article/details/ggepaervb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gcwqfcmrt.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvdplepby.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gnsqtvrkm.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/grkkvbkff.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpzbcvmmg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.hesvh.cn/Article/details/gqtxoobic.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gyomnjyrz.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gdzusnetv.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gezskjrmt.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gwvyygujc.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gaugalqfz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gysaqbrca.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gaodqnxoe.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/goxqjqewi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.hesvh.cn/Article/details/gkcowyrzy.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gnllfpjzh.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gazushbee.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.zdbjq.cn/Article/details/ghwpnawbf.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gcgvdznsd.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://wap.fehbvm.com/Article/details/gdunwfgeo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.hesvh.cn/Article/details/grkgnabkv.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwqdzixtp.sHtML

G. 面向对象
来源：http://blog.zdbjq.cn/Article/details/gwkgdufzk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ggdmdxwgp.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gyhpohxnv.sHtML

Py:   class User: pass
来源：http://www.share.hesvh.cn/Article/details/gxkzruokl.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxrsypdfo.sHtML

JS:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gelsraacx.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gqlizneja.sHtML

Java: class User {}
来源：http://m.share.hesvh.cn/Article/details/goblwyuzb.sHtML

Go:   type User struct { Name string }
来源：http://3g.hesvh.cn/Article/details/gvloeetlo.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gftuowwkb.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/gfyhdldpx.sHtML

[G02] 构造函数
来源：http://www.m.share.hesvh.cn/Article/details/guwsnsgwz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gvgorrqkp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gkrkazslq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gdnpxedwe.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/gggvaxcej.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/guqnvyhdr.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gpugnkdxp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gbmggyjmd.sHtML

C#:   public User(string name) { Name = name; }
来源：http://baike.fehbvm.com/Article/details/gsswscexx.sHtML

[G03] 实例属性
来源：http://wap.fehbvm.com/Article/details/gyiwpmanq.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/gzxfonixg.sHtML

PHP:  public string $name = "x";
来源：http://www.m.share.fehbvm.com/Article/details/ghohyupcc.sHtML

JS:   this.name = "x";
来源：http://read.share.hesvh.cn/Article/details/ghwfrhcfq.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/grtxluygd.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/goyeukvej.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://blog.hesvh.cn/Article/details/gtpedvpdm.sHtML

Ruby: @name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gfswqzcpc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gwmxmavzn.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/gubjmupth.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.fehbvm.com/Article/details/gzwwdvxxt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gtfvckmtb.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/ghtjxgzex.sHtML

TS:   greet(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gxybxnspm.sHtML

Java: String greet() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gjrpnauoj.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://m.share.hesvh.cn/Article/details/grcxgelky.sHtML

Ruby: def greet; @name; end
来源：http://m.share.fehbvm.com/Article/details/gnvcyvdqr.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/gwxsfcuwc.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gknmnbvhi.sHtML

Py:   class Admin(User): pass
来源：http://m.share.hesvh.cn/Article/details/gqerbqppb.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gcsgmfyod.sHtML

JS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gnuwdkmxi.sHtML

TS:   class Admin extends User {}
来源：http://mobile.fehbvm.com/Article/details/glqahuxoa.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/godmmhhyq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gvwjcbpng.sHtML

Ruby: class Admin < User; end
来源：http://mobile.hesvh.cn/Article/details/gdbulepui.sHtML

C#:   class Admin : User {}
来源：http://mobile.zdbjq.cn/Article/details/gjlapphtz.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gvgmuafjk.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gcqdjkxje.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gdbbnsezp.sHtML

JS:   greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gqpuceafd.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gukgtzbnh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gmvnuxope.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gmjtbwzaz.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.hesvh.cn/Article/details/gktrcnobt.sHtML

C#:   public override string Greet() => "admin";
来源：http://3g.zdbjq.cn/Article/details/gbditpdtb.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gsqldzcst.sHtML

Py:   super().greet()
来源：http://www.blog.fehbvm.com/Article/details/gqsfpnrcr.sHtML

PHP:  parent::greet();
来源：http://blog.hesvh.cn/Article/details/gddxzitnf.sHtML

JS:   super.greet();
来源：http://read.share.fehbvm.com/Article/details/glzkwabci.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/glmwducnh.sHtML

Java: super.greet();
来源：http://baike.hesvh.cn/Article/details/gxhtzljae.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.hesvh.cn/Article/details/gqezqhzvi.sHtML

Ruby: super
来源：http://3g.zdbjq.cn/Article/details/guerzymxq.sHtML

C#:   base.Greet();
来源：http://wap.zdbjq.cn/Article/details/gsdhfnfzv.sHtML

[G08] 静态方法与属性
来源：http://m.share.fehbvm.com/Article/details/gztajoeyu.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.zdbjq.cn/Article/details/gxkixbbri.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/gjwhehrnl.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gulvnwhii.sHtML

TS:   static f(): void {}
来源：http://www.m.share.hesvh.cn/Article/details/gpogvbcfq.sHtML

Java: static void f() {}
来源：http://m.share.hesvh.cn/Article/details/gesfwknkk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gavqnnmwh.sHtML

Ruby: def self.f; end
来源：http://www.blog.hesvh.cn/Article/details/gcbmjrfcb.sHtML

C#:   public static void F() {}
来源：http://mobile.hesvh.cn/Article/details/gfapwfcrs.sHtML

[G09] 接口 / 抽象类
来源：http://wap.zdbjq.cn/Article/details/gksosdfol.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.blog.fehbvm.com/Article/details/grjqtypjy.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.blog.fehbvm.com/Article/details/gzateteiz.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gtvfowqow.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gkigzgwls.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.hesvh.cn/Article/details/gllzkgxhj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gqjlasphd.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://3g.fehbvm.com/Article/details/gjbtgtuut.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gkzmyneqy.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gyygbcoqq.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.zdbjq.cn/Article/details/gmiawvjsr.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gstmocwmw.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/gvivyaiiy.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gklxztvlq.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gjcpuxjcx.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.fehbvm.com/Article/details/gyblhhvts.sHtML

Ruby: public / protected / private
来源：http://wap.zdbjq.cn/Article/details/gmnbhbwsy.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/gfhhcqykw.sHtML

[G11] getter / setter
来源：http://mobile.zdbjq.cn/Article/details/gwagnkfxd.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/grwcmljkj.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gvbxktnly.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.zdbjq.cn/Article/details/grltcntxb.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gnoqjikis.sHtML

Java: public String getName() { return name; }
来源：http://3g.fehbvm.com/Article/details/gydlocpuj.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gjmgvofvh.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/granocpnq.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gsckmrjyy.sHtML

[G12] 对象转字符串
来源：http://www.blog.hesvh.cn/Article/details/gutzitdsu.sHtML

Py:   def __str__(self): return self.name
来源：http://3g.hesvh.cn/Article/details/ghwnbgzrm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gvtywbauq.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcpwwwvav.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gdukypumg.sHtML

Java: @Override public String toString() { return name; }
来源：http://m.share.zdbjq.cn/Article/details/glsqoglko.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/goirrbowe.sHtML

Ruby: def to_s; @name; end
来源：http://www.share.fehbvm.com/Article/details/gmwtxmhtu.sHtML

C#:   public override string ToString() => Name;
来源：http://3g.fehbvm.com/Article/details/gndqkbjdi.sHtML

[G13] 判断对象类型
来源：http://read.share.fehbvm.com/Article/details/geisrthsw.sHtML

Py:   isinstance(u, User)
来源：http://mobile.fehbvm.com/Article/details/gimhdlvmx.sHtML

PHP:  $u instanceof User
来源：http://www.share.fehbvm.com/Article/details/glqfugazr.sHtML

JS:   u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gxfkxllse.sHtML

TS:   u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gglvitqtt.sHtML

Java: u instanceof User
来源：http://mobile.zdbjq.cn/Article/details/gmyajgdzm.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.zdbjq.cn/Article/details/ghzxetwfx.sHtML

Ruby: u.is_a?(User)
来源：http://mobile.hesvh.cn/Article/details/gtaknrbty.sHtML

C#:   u is User
来源：http://www.m.share.fehbvm.com/Article/details/gbhchjsqj.sHtML

[G14] 数据类 / record
来源：http://www.share.zdbjq.cn/Article/details/gnlloxbex.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://wap.fehbvm.com/Article/details/gevyvwykc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.fehbvm.com/Article/details/gyobypndt.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.fehbvm.com/Article/details/gpougrvqj.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.zdbjq.cn/Article/details/ggfjiguba.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/ghpmayksf.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.fehbvm.com/Article/details/gdxapscnv.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gaauezwyx.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.hesvh.cn/Article/details/gunlrqvbg.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/golaezltk.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.zdbjq.cn/Article/details/guduzozxe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/giybqudmv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gasedcjnl.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.hesvh.cn/Article/details/gscnuaufq.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.hesvh.cn/Article/details/gxbepuhyq.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://wap.fehbvm.com/Article/details/gjyzhlypt.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.hesvh.cn/Article/details/gljzdnlvb.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.fehbvm.com/Article/details/gyfrkrbow.sHtML

[G16] 对象转数组 / 字典
来源：http://www.blog.zdbjq.cn/Article/details/gginwgdhb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gxtjgcphm.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.zdbjq.cn/Article/details/gfadascfp.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gdnizbkub.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gkfyxkxvz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.zdbjq.cn/Article/details/goeidgdor.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.hesvh.cn/Article/details/gbkdvwjgl.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gkzvflsqh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gcaobqfjw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqhkjtjfw.sHtML

H. 异常与错误处理
来源：http://read.share.fehbvm.com/Article/details/gftcjkuiy.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gelftidqf.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gzsproabm.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://m.share.fehbvm.com/Article/details/gtcuekcew.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.fehbvm.com/Article/details/goluuilpr.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://blog.hesvh.cn/Article/details/gjraihuyd.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://mobile.zdbjq.cn/Article/details/gduveuguj.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gobqjwelf.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.fehbvm.com/Article/details/gcsqjuecd.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/gwjlsoorf.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/grhnldiug.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gqarqzoic.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/ghvlfojcc.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.hesvh.cn/Article/details/gorcifoft.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/ghpwhdufc.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.zdbjq.cn/Article/details/gmvqglorm.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwurqinfh.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gtcfpperi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gfflvdzyv.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://wap.hesvh.cn/Article/details/giqiymnrd.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gxdylvcen.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.fehbvm.com/Article/details/gpciakfla.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gaowgpeuz.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.hesvh.cn/Article/details/ghlqmeird.sHtML

TS:   throw new Error("错误信息");
来源：http://baike.hesvh.cn/Article/details/gldigmmtx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gjogsaczn.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.zdbjq.cn/Article/details/grirqmynu.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gwtiadyhr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/guuvzfvbg.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gltwmiuaa.sHtML

Py:   class MyError(Exception): pass
来源：http://read.share.hesvh.cn/Article/details/gkbuzrcie.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gtiimbvtx.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gsldbiaqj.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.hesvh.cn/Article/details/gypumicyn.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gwrnqhfvh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.fehbvm.com/Article/details/gwewumkvp.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.zdbjq.cn/Article/details/gdafukqar.sHtML

C#:   class MyException : Exception {}
来源：http://blog.zdbjq.cn/Article/details/gzpkvnlxw.sHtML

[H05] 捕获特定类型
来源：http://3g.hesvh.cn/Article/details/gttjxtxcq.sHtML

Py:   except ValueError as e:
来源：http://www.blog.hesvh.cn/Article/details/gizkfbzqf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gbbkxfzai.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/ggmuizhmn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://m.share.hesvh.cn/Article/details/gshlupzfa.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/gsiwojldk.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gqfrtufrd.sHtML

Ruby: rescue ArgumentError => e
来源：http://m.share.fehbvm.com/Article/details/gntoandcz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.hesvh.cn/Article/details/girkjsekx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://blog.fehbvm.com/Article/details/gzgzlzuho.sHtML

Py:   value = d.get("k") or default
来源：http://3g.zdbjq.cn/Article/details/gfaojbcbs.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://baike.fehbvm.com/Article/details/gobaunhnw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gumbszikc.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gcmiifezt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.hesvh.cn/Article/details/gmbmhldyi.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/gbupdljgi.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/giqdixgqn.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.fehbvm.com/Article/details/gubasntst.sHtML

[H07] 断言
来源：http://wap.zdbjq.cn/Article/details/gpzpppktn.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.m.share.fehbvm.com/Article/details/gibecrhzp.sHtML

PHP:  assert($x > 0);
来源：http://www.share.fehbvm.com/Article/details/giddrabsw.sHtML

JS:   console.assert(x > 0);
来源：http://blog.zdbjq.cn/Article/details/gdtyasmpf.sHtML

TS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/grqqxsazh.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.fehbvm.com/Article/details/gxawypniv.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://read.share.zdbjq.cn/Article/details/gpcsoiled.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.hesvh.cn/Article/details/ggunjhfmt.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/gvbirtxnj.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.zdbjq.cn/Article/details/gruyxxjgb.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://baike.hesvh.cn/Article/details/gvomdartf.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/ggcrmlyxp.sHtML

JS:   e.message;  e.stack
来源：http://baike.zdbjq.cn/Article/details/gpcfdfdko.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.hesvh.cn/Article/details/gtuvrnuic.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.m.share.fehbvm.com/Article/details/gctqvswap.sHtML

Go:   err.Error()
来源：http://www.share.zdbjq.cn/Article/details/gnspxqegl.sHtML

Ruby: e.message;  e.backtrace
来源：http://mobile.fehbvm.com/Article/details/gssccxhje.sHtML

C#:   e.Message;  e.StackTrace
来源：http://baike.fehbvm.com/Article/details/gnmduvpah.sHtML

[H09] 带错误码的异常
来源：http://blog.zdbjq.cn/Article/details/gjaduoifj.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://read.share.zdbjq.cn/Article/details/gnkppcwnv.sHtML


<!-- 参考信息 -->