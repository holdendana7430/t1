代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://wap.fehbvm.com/Article/details/gyjstrctw.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/goxqwdots.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.fehbvm.com/Article/details/gzafqcktp.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gbgzfvgcs.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.fehbvm.com/Article/details/ghmqbxxpt.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/grthcxgym.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/giagdqskg.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.hesvh.cn/Article/details/gwjjfuvdy.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/ggeluankl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gmzctfdrt.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gunmbblwp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/grehwcjgv.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gcjvgwoxn.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gjpgpptyw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.hesvh.cn/Article/details/gdzdkkrao.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gvzuaqoae.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvgjcldji.sHtML

[F06] 删除文件
来源：http://www.share.hesvh.cn/Article/details/gwadeqhru.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnfteujoi.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gofwhzind.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gdlazmmly.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkazwldvc.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gzputibhf.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/gfvvgcqwj.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gltomjdio.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gfsxbkmgn.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gxbrmhzly.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/ghmgrcmwy.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.hesvh.cn/Article/details/grpslfmuy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gggacywfi.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gpdsrxwgr.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.fehbvm.com/Article/details/ggzrlpasg.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://3g.hesvh.cn/Article/details/gprduwtpe.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://wap.hesvh.cn/Article/details/gpgtnwvkj.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gnuyqgcfo.sHtML

[F08] 遍历目录
来源：http://baike.zdbjq.cn/Article/details/glxkgjvdy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.hesvh.cn/Article/details/ghtgjpdug.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/gnlkcugcw.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.hesvh.cn/Article/details/gycqnofem.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.zdbjq.cn/Article/details/gvrjdromp.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.fehbvm.com/Article/details/ggihowaiw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gcmeducvo.sHtML

Ruby: Dir.children("dir")
来源：http://mobile.hesvh.cn/Article/details/gfhucfsxn.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.fehbvm.com/Article/details/gagunhksn.sHtML

[F09] 获取文件大小
来源：http://www.m.share.fehbvm.com/Article/details/gbexwttfi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gbuwaucby.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gtykipezy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gacqhnpmz.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.fehbvm.com/Article/details/ghgftswet.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://wap.hesvh.cn/Article/details/gypzisveq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gvcdifkup.sHtML

Ruby: File.size("a.txt")
来源：http://blog.hesvh.cn/Article/details/ggijhpjno.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gtbbjwtdq.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://blog.hesvh.cn/Article/details/gmamkrljj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gsgxlkatu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/glmugkdot.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gkzyseopz.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gskzoxdaz.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.zdbjq.cn/Article/details/gwtumjfrx.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gssqujioz.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gzkaltpcy.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gqlpkljwf.sHtML

[F11] 复制与移动文件
来源：http://m.share.zdbjq.cn/Article/details/glzzkbjjr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/ggbqwpaoh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gbupmioli.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gfamvulpq.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gpnufolpe.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://wap.fehbvm.com/Article/details/gyrwyadeq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gvutddxss.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gewgmzeby.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.zdbjq.cn/Article/details/gddtnkxyp.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gjhlpnume.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.zdbjq.cn/Article/details/gixhlokvk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.hesvh.cn/Article/details/gvglruhwi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://mobile.hesvh.cn/Article/details/gitkfjgfy.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gcfuqmxlk.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.fehbvm.com/Article/details/gcwuuliky.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.zdbjq.cn/Article/details/ggqjenekv.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://mobile.fehbvm.com/Article/details/gbtgeslrk.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.zdbjq.cn/Article/details/gprlqjlyu.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gvuvmpnpp.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gmstdcfrd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpbwtesqv.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gbltthxjr.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/glyctyyoo.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/geyqvhrmw.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gcyeedfzz.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.hesvh.cn/Article/details/gjyktwwxg.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gskexmmye.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/geyanvubr.sHtML

Ruby: class User; end
来源：http://www.share.hesvh.cn/Article/details/grrisvbkm.sHtML

C#:   class User {}
来源：http://blog.fehbvm.com/Article/details/gzgqcxgil.sHtML

[G02] 构造函数
来源：http://read.share.hesvh.cn/Article/details/gnamkqfob.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gxapqecru.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.hesvh.cn/Article/details/gdkkwrppn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gongvacjc.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gkiugrfrt.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gmmvmanfn.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.fehbvm.com/Article/details/gpxsltfge.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.hesvh.cn/Article/details/gfmdxelym.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.hesvh.cn/Article/details/gpeopgpuh.sHtML

[G03] 实例属性
来源：http://www.share.hesvh.cn/Article/details/gcmedrzlu.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gsztuofrx.sHtML

PHP:  public string $name = "x";
来源：http://3g.hesvh.cn/Article/details/gnyjmysip.sHtML

JS:   this.name = "x";
来源：http://read.share.zdbjq.cn/Article/details/ghfxnehxo.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/glvtnkcjr.sHtML

Java: private String name;
来源：http://www.share.hesvh.cn/Article/details/gvjlekagq.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/gxoawjyob.sHtML

Ruby: @name = "x"
来源：http://blog.fehbvm.com/Article/details/grvdiyvnc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.hesvh.cn/Article/details/gpfbwcohl.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gkixaxvjb.sHtML

Py:   def greet(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gjdqahiwq.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmrwavikq.sHtML

JS:   greet() { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/glvxtpzyp.sHtML

TS:   greet(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/gpwpuazsi.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gltefypfd.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gcouqaaii.sHtML

Ruby: def greet; @name; end
来源：http://m.share.hesvh.cn/Article/details/gcgdoobso.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/grplfolky.sHtML

[G05] 继承
来源：http://blog.zdbjq.cn/Article/details/gszlybihy.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/gbxygabxy.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/gmprfzcee.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gjslvkpdn.sHtML

TS:   class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gzqxznuam.sHtML

Java: class Admin extends User {}
来源：http://m.share.hesvh.cn/Article/details/gkqtwgzml.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gxhzwxgvn.sHtML

Ruby: class Admin < User; end
来源：http://m.share.fehbvm.com/Article/details/gxvmivmdp.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/grfuhywzy.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gkhztahzm.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gzqoqrmmn.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gtrczzubu.sHtML

JS:   greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/glvbqfqnv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gwjybsxbe.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gylgpnfib.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gfttyxwyv.sHtML

Ruby: def greet; "admin"; end
来源：http://m.share.zdbjq.cn/Article/details/gsslawlrm.sHtML

C#:   public override string Greet() => "admin";
来源：http://blog.hesvh.cn/Article/details/gnmtucehc.sHtML

[G07] 调用父类方法
来源：http://3g.fehbvm.com/Article/details/gyoxzwpuq.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gdahsaxog.sHtML

PHP:  parent::greet();
来源：http://3g.zdbjq.cn/Article/details/gwlhkuikz.sHtML

JS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gdaaglbby.sHtML

TS:   super.greet();
来源：http://m.share.fehbvm.com/Article/details/gkhnztata.sHtML

Java: super.greet();
来源：http://3g.zdbjq.cn/Article/details/gznjmukpk.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://baike.fehbvm.com/Article/details/gmilnygtg.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gwfznyebi.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gyrmmtgdz.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gcgxnlbis.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gfbgfcyuu.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gikpvpwxr.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/gkkoqrpfd.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/goxfuzlbb.sHtML

Java: static void f() {}
来源：http://baike.hesvh.cn/Article/details/gzgpesedk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gmjkxhgiy.sHtML

Ruby: def self.f; end
来源：http://m.share.hesvh.cn/Article/details/ggmaeyywd.sHtML

C#:   public static void F() {}
来源：http://www.share.hesvh.cn/Article/details/gvcngfiwl.sHtML

[G09] 接口 / 抽象类
来源：http://wap.fehbvm.com/Article/details/gquolpstb.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://baike.hesvh.cn/Article/details/ghvrtrotp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://blog.hesvh.cn/Article/details/gnzvmzsfs.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.zdbjq.cn/Article/details/gfhsjmprv.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gfbcdctlp.sHtML

Java: interface Shape { double area(); }
来源：http://3g.zdbjq.cn/Article/details/gwbsqclio.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.hesvh.cn/Article/details/gbognugck.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/gshoowluh.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gbzwqzuxy.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gphauwcti.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.blog.fehbvm.com/Article/details/gmfxumwey.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/gatixazop.sHtML

JS:   #private 字段；其余公开
来源：http://3g.zdbjq.cn/Article/details/gmtkwphmr.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gutkjofom.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gvrmkhisw.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://mobile.hesvh.cn/Article/details/gzourzxqd.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/goctaqsux.sHtML

C#:   public / protected / private / internal
来源：http://www.m.share.zdbjq.cn/Article/details/gyxfpzejc.sHtML

[G11] getter / setter
来源：http://www.blog.hesvh.cn/Article/details/gkipwjxvc.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.zdbjq.cn/Article/details/glqzibaqe.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/guszeyyxs.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.hesvh.cn/Article/details/gqoqegpfm.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gaiaffsaz.sHtML

Java: public String getName() { return name; }
来源：http://blog.hesvh.cn/Article/details/gvgorhvbr.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.zdbjq.cn/Article/details/gszvvdaan.sHtML

Ruby: attr_accessor :name
来源：http://baike.zdbjq.cn/Article/details/glrsalqfg.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gvqjutzrx.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gedlfzcna.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.hesvh.cn/Article/details/gsnsylljx.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.blog.hesvh.cn/Article/details/gughhgpru.sHtML

JS:   toString() { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/gybtbmmeu.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gouzmscwv.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.zdbjq.cn/Article/details/gdxcsumad.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gmoplcguj.sHtML

Ruby: def to_s; @name; end
来源：http://3g.hesvh.cn/Article/details/ghpwhbkik.sHtML

C#:   public override string ToString() => Name;
来源：http://www.share.fehbvm.com/Article/details/gnwbzsyvl.sHtML

[G13] 判断对象类型
来源：http://www.blog.hesvh.cn/Article/details/gengppcoo.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/guttnxgtn.sHtML

PHP:  $u instanceof User
来源：http://wap.fehbvm.com/Article/details/giehxsfsp.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/glvwcmiiv.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/ghaxrjbgi.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gvugifezw.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.hesvh.cn/Article/details/gufexhtpn.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gfqnuyacg.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gjnyhdkod.sHtML

[G14] 数据类 / record
来源：http://www.m.share.fehbvm.com/Article/details/gzebkfvsr.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.zdbjq.cn/Article/details/gcnslmjeu.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gfhjwbpdl.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gmxdhgcmi.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gdcnsqszf.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.hesvh.cn/Article/details/guhwowyfn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.share.zdbjq.cn/Article/details/gcwtfbsqh.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gqxovrwlc.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gbnmlewjl.sHtML

[G15] 枚举
来源：http://www.share.hesvh.cn/Article/details/gfugitadc.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gnxtgaqsk.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.zdbjq.cn/Article/details/gohjzaqxm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.hesvh.cn/Article/details/gqerhkurp.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/giqmybwmt.sHtML

Java: enum Color { RED, GREEN }
来源：http://3g.fehbvm.com/Article/details/gkkazujnx.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gvznssbgm.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.fehbvm.com/Article/details/gplelkrhw.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/ggarhnflz.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.fehbvm.com/Article/details/glgguaqry.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gxgwaahxk.sHtML

PHP:  get_object_vars($obj);
来源：http://wap.fehbvm.com/Article/details/gcqotjkps.sHtML

JS:   Object.entries(obj)
来源：http://m.share.hesvh.cn/Article/details/gsrsaupkn.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gzzvugkzz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gepzdxoxe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.hesvh.cn/Article/details/gtvvtjtlj.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/geuiiidam.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gnhidynwt.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/girtlhxiq.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gccymsnrm.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/godyvrdfq.sHtML

[H01] try / catch 基础
来源：http://www.share.hesvh.cn/Article/details/gybrsgywq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gkyphbgod.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.hesvh.cn/Article/details/gllotdymz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.hesvh.cn/Article/details/garnctnkq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/guoqosmow.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.fehbvm.com/Article/details/gdiiokqdh.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.zdbjq.cn/Article/details/gsvagsphy.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/gttxyamml.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.hesvh.cn/Article/details/gglcapgin.sHtML

[H02] finally / ensure 收尾
来源：http://wap.zdbjq.cn/Article/details/ghaheaald.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.hesvh.cn/Article/details/gmfmaytcn.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://m.share.zdbjq.cn/Article/details/gemedimyp.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.zdbjq.cn/Article/details/geamoavbt.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/galnounoq.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gcfjsfhwx.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://blog.fehbvm.com/Article/details/gtrklcekt.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gaobyblsr.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gvptttvjc.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.fehbvm.com/Article/details/gnkruaqvq.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/gmsrycczf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gjfhazhcg.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gbmabrtko.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gfhmotgdb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/grroseyye.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.blog.zdbjq.cn/Article/details/gslnziizf.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gvhytcvjq.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gjkoezslj.sHtML

[H04] 自定义异常类型
来源：http://read.share.zdbjq.cn/Article/details/glllcvrtu.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.zdbjq.cn/Article/details/gzojinzci.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.share.zdbjq.cn/Article/details/goeqfrezt.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gtzlhydrf.sHtML

TS:   class MyError extends Error {}
来源：http://3g.fehbvm.com/Article/details/gtonlxcol.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gwnlszhrh.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.fehbvm.com/Article/details/gotewzcdm.sHtML

Ruby: class MyError < StandardError; end
来源：http://3g.fehbvm.com/Article/details/gqtsevetf.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gqhugtaon.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/giszuzgjz.sHtML

Py:   except ValueError as e:
来源：http://mobile.hesvh.cn/Article/details/gbpekydmy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://baike.hesvh.cn/Article/details/gcnhpghgo.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gqclnjuhm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gokqjcnbf.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://mobile.zdbjq.cn/Article/details/ggeprcxls.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.zdbjq.cn/Article/details/gjibzhmqx.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.zdbjq.cn/Article/details/gowdpfiqx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.hesvh.cn/Article/details/gyihldddn.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.zdbjq.cn/Article/details/gchuyugvd.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gbxrikanq.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gdmrdbhaz.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.blog.fehbvm.com/Article/details/gxzrjgvza.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/ginawajyk.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.hesvh.cn/Article/details/gjspmnrlz.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.hesvh.cn/Article/details/grwufhqyg.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.fehbvm.com/Article/details/gwbumeckm.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.hesvh.cn/Article/details/gnupxltiq.sHtML

[H07] 断言
来源：http://www.m.share.zdbjq.cn/Article/details/gqkuuhngr.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.hesvh.cn/Article/details/grpcxmjjr.sHtML

PHP:  assert($x > 0);
来源：http://www.blog.zdbjq.cn/Article/details/gedmetutt.sHtML

JS:   console.assert(x > 0);
来源：http://www.blog.hesvh.cn/Article/details/gporsmenp.sHtML

TS:   console.assert(x > 0);
来源：http://www.blog.fehbvm.com/Article/details/grglpocjn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://wap.zdbjq.cn/Article/details/ghimmvgpk.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://mobile.zdbjq.cn/Article/details/gnznvsrrj.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://www.m.share.zdbjq.cn/Article/details/gnfzamkic.sHtML

C#:   Debug.Assert(x > 0);
来源：http://baike.hesvh.cn/Article/details/gvflgahtk.sHtML

[H08] 获取错误信息与堆栈
来源：http://mobile.hesvh.cn/Article/details/gaflzxksh.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://read.share.hesvh.cn/Article/details/gxnkbdhij.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://mobile.fehbvm.com/Article/details/gnchqmjtm.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gfiqfrmbb.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://mobile.zdbjq.cn/Article/details/gwatlupfg.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://www.share.zdbjq.cn/Article/details/gvleybyzp.sHtML

Go:   err.Error()
来源：http://3g.fehbvm.com/Article/details/gbwqtitfs.sHtML


<!-- 参考信息 -->