代发 wailian999

[F05] 判断文件或目录是否存在
来源：http://baike.zdbjq.cn/Article/details/gsnswagth.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gmqowtpzs.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gvfkvqikc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gwdgcimyq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gajdibhqe.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gjurlrjjt.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gxgskwfev.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gxrytwjcb.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/gnhomadoo.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gulagnjoy.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxkzclhxg.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gktcoratl.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gqnhxmaxy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkrepiwyv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gwmpvfurp.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfowsidoa.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gzemcbadf.sHtML

C#:   File.Delete("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gztcbivck.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.hesvh.cn/Article/details/gtjfsbzkq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.hesvh.cn/Article/details/gdhauhynq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.zdbjq.cn/Article/details/gnsajobpj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gkihniiok.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gpvrrontt.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gmmzrutpz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.fehbvm.com/Article/details/gimovdgak.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.zdbjq.cn/Article/details/gukinbipo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/ggeilhvdv.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gpehmklmg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.blog.fehbvm.com/Article/details/gzmhykaex.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.fehbvm.com/Article/details/gbcfkjpzu.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gkpwpebwb.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gmlxtbxqc.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.blog.hesvh.cn/Article/details/gfvxxdbzz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gvtfqozcx.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.hesvh.cn/Article/details/gmyrtxjmk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/grirbzmad.sHtML

[F09] 获取文件大小
来源：http://blog.zdbjq.cn/Article/details/glzpqkpjo.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gujcvojkn.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gwgptzhyg.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gscccknlx.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/gvugujfrk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/giqzemfkf.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gpcntiyhp.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gydzjhutd.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.fehbvm.com/Article/details/gimzinadh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.zdbjq.cn/Article/details/gprcfsyle.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/ggzoczbcm.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gtjvorqnm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gkgdhosum.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/ggihnthyg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.hesvh.cn/Article/details/gatdujdsg.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvenhssni.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/guadglids.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gfogttaqg.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gqsvqtrxr.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggblyptod.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gvwmwxlgi.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gbanprmgm.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gmohfckxj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gvaqebgzk.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gheippeky.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/guyohlyrr.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gaivqhbhq.sHtML

[F12] CSV 读写
来源：http://blog.fehbvm.com/Article/details/glvksxzms.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://m.share.zdbjq.cn/Article/details/gzuyggmdi.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.fehbvm.com/Article/details/gnsyfkbdg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/gartgijbh.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/ggvmcgmht.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gzxcnniyv.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/grmwmabjk.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/gwanmqxdo.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/ghkpoqopz.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gurcdlliv.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/giynqldns.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzmpuaqmk.sHtML

[G01] 定义类
来源：http://www.blog.zdbjq.cn/Article/details/gtqaojffl.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/ggsbwdxfc.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gicbkfyxm.sHtML

JS:   class User {}
来源：http://wap.zdbjq.cn/Article/details/gxkhleduo.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.zdbjq.cn/Article/details/gsizlyruy.sHtML

Java: class User {}
来源：http://baike.hesvh.cn/Article/details/gmqmcpqmr.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/grullupes.sHtML

Ruby: class User; end
来源：http://www.blog.zdbjq.cn/Article/details/gvxnqyznu.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/ghwwksthc.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/gmohtffhn.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.hesvh.cn/Article/details/grkuvqxrd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/gvjwvyihh.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/guinmmlqz.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.hesvh.cn/Article/details/gjqwogzwo.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfuxlshka.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.fehbvm.com/Article/details/gybqzwkfr.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fehbvm.com/Article/details/gnhmfxuiu.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gxqymwxvu.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gtjalydyv.sHtML

Py:   self.name = "x"
来源：http://mobile.zdbjq.cn/Article/details/gciresemx.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/garrvtwsh.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/ggzczdjce.sHtML

TS:   name: string = "x";
来源：http://www.share.hesvh.cn/Article/details/gkngsxllt.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gjhigpxyn.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/gyjdcvnjk.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/gjqtvyjnv.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.zdbjq.cn/Article/details/gcrdikify.sHtML

[G04] 定义方法
来源：http://m.share.fehbvm.com/Article/details/gvpdomymb.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gademojpu.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gxhvmgkzu.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gqbmitwiy.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gwnsbhcuo.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gbphlcoqh.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gmueergsi.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.hesvh.cn/Article/details/gepcpauvc.sHtML

C#:   public string Greet() => Name;
来源：http://3g.zdbjq.cn/Article/details/gplgtiaiv.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gyowsuisr.sHtML

Py:   class Admin(User): pass
来源：http://mobile.zdbjq.cn/Article/details/geaefzyat.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gxaaysdnx.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gskxsusen.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gashpijqe.sHtML

Java: class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/ghgplemvn.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/grfbqupjk.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gscaagoqw.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gqzksuxcj.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gbvmfxlla.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gjazdrcdi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.hesvh.cn/Article/details/giwnwdexz.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gufbmrkat.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gdlxuonqs.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gbylmynvt.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://mobile.fehbvm.com/Article/details/gbbpvwgcu.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.hesvh.cn/Article/details/gtemnfiie.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.zdbjq.cn/Article/details/gvtvdmpyy.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gimcqcboc.sHtML

Py:   super().greet()
来源：http://3g.zdbjq.cn/Article/details/ghmztpyvm.sHtML

PHP:  parent::greet();
来源：http://wap.zdbjq.cn/Article/details/gmipshxkg.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/grekitjhn.sHtML

TS:   super.greet();
来源：http://mobile.fehbvm.com/Article/details/gghuqbbxw.sHtML

Java: super.greet();
来源：http://www.blog.zdbjq.cn/Article/details/guuddctkf.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.fehbvm.com/Article/details/gtzoalhyy.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gjxrfgbnv.sHtML

C#:   base.Greet();
来源：http://read.share.zdbjq.cn/Article/details/gtwiijydm.sHtML

[G08] 静态方法与属性
来源：http://www.blog.fehbvm.com/Article/details/gaitrnfku.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://blog.zdbjq.cn/Article/details/gqukccyxp.sHtML

PHP:  public static function f() {}
来源：http://3g.hesvh.cn/Article/details/gfqbsrbnq.sHtML

JS:   static f() {}
来源：http://mobile.fehbvm.com/Article/details/gljwvgans.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gygktyfhe.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gbmegbciz.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gugnosbcs.sHtML

Ruby: def self.f; end
来源：http://www.m.share.zdbjq.cn/Article/details/gbwsvvecj.sHtML

C#:   public static void F() {}
来源：http://m.share.hesvh.cn/Article/details/gqagiuxkb.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.hesvh.cn/Article/details/gveppeaiv.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://mobile.hesvh.cn/Article/details/gwtafnbwq.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/glmpjaewg.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.zdbjq.cn/Article/details/gzszsqvkk.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.zdbjq.cn/Article/details/gpekntzvq.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/grwtalnuf.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.fehbvm.com/Article/details/gmclnujar.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/goiqxbhsz.sHtML

C#:   interface IShape { double Area(); }
来源：http://wap.zdbjq.cn/Article/details/gaibeinmv.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/girsybzbu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/ggcrelmra.sHtML

PHP:  public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gjxbgeyle.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.zdbjq.cn/Article/details/ggftrnrvz.sHtML

TS:   public / protected / private
来源：http://mobile.zdbjq.cn/Article/details/gybnofzzx.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.fehbvm.com/Article/details/gqucljnfg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gwspvtctw.sHtML

Ruby: public / protected / private
来源：http://m.share.fehbvm.com/Article/details/gxxqlggpq.sHtML

C#:   public / protected / private / internal
来源：http://mobile.zdbjq.cn/Article/details/glgycbkhp.sHtML

[G11] getter / setter
来源：http://wap.fehbvm.com/Article/details/gbiozzari.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gmwioirox.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gsubfpuug.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gzhgitpwr.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gpycqawfo.sHtML

Java: public String getName() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gtfqhoziu.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gwglrhbgi.sHtML

Ruby: attr_accessor :name
来源：http://3g.zdbjq.cn/Article/details/gxycahauv.sHtML

C#:   public string Name { get; set; }
来源：http://www.m.share.fehbvm.com/Article/details/gfdrsipbi.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gtawwcvku.sHtML

Py:   def __str__(self): return self.name
来源：http://baike.zdbjq.cn/Article/details/gsszckxjv.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.share.hesvh.cn/Article/details/gnwpgfszz.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwezikfcd.sHtML

TS:   toString(): string { return this.name; }
来源：http://wap.fehbvm.com/Article/details/gcymbqnxq.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.zdbjq.cn/Article/details/gcpsnyypw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gyuacqldd.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gcxbnicdj.sHtML

C#:   public override string ToString() => Name;
来源：http://baike.hesvh.cn/Article/details/gisjvqful.sHtML

[G13] 判断对象类型
来源：http://www.m.share.fehbvm.com/Article/details/grxbjwozl.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gombjsdaa.sHtML

PHP:  $u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ggssyltgv.sHtML

JS:   u instanceof User
来源：http://3g.fehbvm.com/Article/details/gptevogyu.sHtML

TS:   u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gfnwnwajk.sHtML

Java: u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gptywgvhv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://3g.zdbjq.cn/Article/details/guredmzfa.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gfcwaaubx.sHtML

C#:   u is User
来源：http://read.share.zdbjq.cn/Article/details/gjnxloccy.sHtML

[G14] 数据类 / record
来源：http://mobile.hesvh.cn/Article/details/gbzpjvchz.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gfstemslc.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gynxctbwj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gqciyyznv.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.fehbvm.com/Article/details/gvilezima.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.hesvh.cn/Article/details/grnbaajmx.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/grqqzptwl.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mobile.hesvh.cn/Article/details/gqakqtyzc.sHtML

C#:   record User(string Name, int Age);
来源：http://www.share.zdbjq.cn/Article/details/gsosnwqiy.sHtML

[G15] 枚举
来源：http://mobile.zdbjq.cn/Article/details/gtgyszkok.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gjtzpfdrm.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.fehbvm.com/Article/details/gusgdzvwn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.fehbvm.com/Article/details/gtebmweke.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.hesvh.cn/Article/details/ghnpezlak.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.share.zdbjq.cn/Article/details/gxfbpduwo.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.hesvh.cn/Article/details/goybxzhsd.sHtML

Ruby: Color = %i[red green].freeze
来源：http://read.share.hesvh.cn/Article/details/geptvyxyj.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.fehbvm.com/Article/details/gvtdfpqsk.sHtML

[G16] 对象转数组 / 字典
来源：http://wap.fehbvm.com/Article/details/gqurejjuc.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.zdbjq.cn/Article/details/ggvrckeea.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/gskajlqbx.sHtML

JS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gcveytlvs.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/gnvylohwz.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.fehbvm.com/Article/details/gywyiudjn.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.fehbvm.com/Article/details/gsgwbvigp.sHtML

Ruby: obj.instance_variables
来源：http://read.share.hesvh.cn/Article/details/gcxuumygo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://mobile.zdbjq.cn/Article/details/gtqqjswoo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqdqisyzm.sHtML

H. 异常与错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/gsvndfvvz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwfmdpqnn.sHtML

[H01] try / catch 基础
来源：http://wap.zdbjq.cn/Article/details/gcetjxfol.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.zdbjq.cn/Article/details/ghswluzmq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://mobile.hesvh.cn/Article/details/gfxwhhqxt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gjpgecvyw.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gfatswene.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.fehbvm.com/Article/details/gbyzvodvy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://baike.fehbvm.com/Article/details/glrunvrah.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.zdbjq.cn/Article/details/gdfnclqyt.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.fehbvm.com/Article/details/gthivlqcx.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.zdbjq.cn/Article/details/gdhliqzjr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.fehbvm.com/Article/details/gbowgvjom.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gxknsgtys.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.zdbjq.cn/Article/details/gwebaccht.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gmhcnbgud.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gcznxmwnv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://read.share.hesvh.cn/Article/details/gmvzenvxu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://read.share.fehbvm.com/Article/details/gymbgupwf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gsalfhuyw.sHtML

[H03] 主动抛出异常
来源：http://wap.fehbvm.com/Article/details/gsqwgjqgy.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.zdbjq.cn/Article/details/gocnifjdm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.zdbjq.cn/Article/details/ggwhzjqbn.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gxkhhxtqr.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gnvooeacb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/grpxhmxqk.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/ggynsozrn.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://mobile.hesvh.cn/Article/details/gcrkovlmp.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.m.share.zdbjq.cn/Article/details/gtfputczq.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gjkhimmfg.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.fehbvm.com/Article/details/gekyiygcs.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gumlxdyea.sHtML

JS:   class MyError extends Error {}
来源：http://3g.zdbjq.cn/Article/details/gbjzpolcs.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/gdabcuzvh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gmquhtvzm.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.hesvh.cn/Article/details/gnvvlxfzo.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.hesvh.cn/Article/details/gtjtsqjoc.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.fehbvm.com/Article/details/gwwgxrfzd.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gsyccolca.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gxngjysux.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.hesvh.cn/Article/details/gcnoesixs.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://blog.hesvh.cn/Article/details/gaydrhlxf.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gryuatlxx.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/giwwarkil.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gblyynhwf.sHtML

Ruby: rescue ArgumentError => e
来源：http://mobile.hesvh.cn/Article/details/gcfilarlx.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gonzfruek.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gihjnaeqz.sHtML

Py:   value = d.get("k") or default
来源：http://3g.hesvh.cn/Article/details/gqvltubsy.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/gdslhafij.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gtuhodrbx.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gigqisnke.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gcswchbec.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/guaxrnlxp.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.m.share.zdbjq.cn/Article/details/gqhzfohvm.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gofdeveky.sHtML

[H07] 断言
来源：http://3g.zdbjq.cn/Article/details/giyfsrrbe.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.share.hesvh.cn/Article/details/gdfkajrle.sHtML

PHP:  assert($x > 0);
来源：http://blog.hesvh.cn/Article/details/gmtkfgoxi.sHtML

JS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gmimupygj.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/ghybhutiu.sHtML

Java: assert x > 0 : "必须为正";
来源：http://blog.hesvh.cn/Article/details/gnanqauvx.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.zdbjq.cn/Article/details/grknaiose.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://3g.zdbjq.cn/Article/details/ggdkzzrwi.sHtML

C#:   Debug.Assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/glhyzetkq.sHtML

[H08] 获取错误信息与堆栈
来源：http://www.share.hesvh.cn/Article/details/gcyxmgprc.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.zdbjq.cn/Article/details/gnsymgnog.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://blog.zdbjq.cn/Article/details/gnndygsby.sHtML

JS:   e.message;  e.stack
来源：http://www.share.fehbvm.com/Article/details/gcrhogqzo.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://www.m.share.zdbjq.cn/Article/details/ggnzprfub.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://3g.fehbvm.com/Article/details/gxmkawpov.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gvvoxqqyu.sHtML

Ruby: e.message;  e.backtrace
来源：http://3g.zdbjq.cn/Article/details/gtmgknvdk.sHtML

C#:   e.Message;  e.StackTrace
来源：http://www.m.share.hesvh.cn/Article/details/gqlvpiyrh.sHtML

[H09] 带错误码的异常
来源：http://blog.fehbvm.com/Article/details/gtiiwvvih.sHtML

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://blog.hesvh.cn/Article/details/gjaypzady.sHtML

PHP:  throw new RuntimeException("fail", 500);
来源：http://mobile.zdbjq.cn/Article/details/gwyuaodwg.sHtML

JS:   const err = new Error("fail");  err.code = 500;
来源：http://www.m.share.zdbjq.cn/Article/details/gfakelgcw.sHtML

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://3g.fehbvm.com/Article/details/gpbzlbnqg.sHtML

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://www.m.share.hesvh.cn/Article/details/ggpqztuvm.sHtML


<!-- 参考信息 -->