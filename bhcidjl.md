代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.hesvh.cn/Article/details/gtjyzugmo.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/gqzzfrtru.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.fehbvm.com/Article/details/gfpnlqcpu.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gxixceqjb.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.hesvh.cn/Article/details/gmewpjqzp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.zdbjq.cn/Article/details/gmtevxbjq.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gsrozecgt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gqkvnaxqw.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/ghgiyuocd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gpbigrqbh.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gistszboa.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/ggkhoeyyx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gkydvmyem.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.fehbvm.com/Article/details/gdgyhkmny.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gwpyudbrm.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/geksqjxit.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gagglwmql.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gajnmlkoe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gmgljuwzh.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtsdnufvj.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gbxkuqmex.sHtML

[F06] 删除文件
来源：http://3g.fehbvm.com/Article/details/gsczcolvr.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbalalqal.sHtML

PHP:  unlink("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gvtoibhlt.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gdlnddigq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gflwqrspz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gdrnivltq.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcrfjlqzf.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gilokslqo.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gqvhafzln.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gyrmkzgli.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.zdbjq.cn/Article/details/giidzfafl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.zdbjq.cn/Article/details/gahuwhnxg.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gqodlnvwr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/ghxwwxnix.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gqzxivvth.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.fehbvm.com/Article/details/gqcncgdgj.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.fehbvm.com/Article/details/gkckwddru.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/guqxdhzmu.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gcgfuledi.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/ghygzcjkz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://3g.hesvh.cn/Article/details/gfxlusqix.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gdqovmwpz.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/grgnayker.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gqrlcveyb.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.zdbjq.cn/Article/details/gvtezkiii.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/gnoeozhwq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.hesvh.cn/Article/details/gcwdcloxg.sHtML

[F09] 获取文件大小
来源：http://www.blog.hesvh.cn/Article/details/gughjokha.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtaknwuwz.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/guzkxnpqy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/gsmxxuobq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/gnzgjtsnt.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gajbwkgif.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://mobile.fehbvm.com/Article/details/gpfxgyrge.sHtML

Ruby: File.size("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gwgvgebww.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/gndjeimas.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.m.share.hesvh.cn/Article/details/gcqeekyfj.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqxhhcjnf.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.fehbvm.com/Article/details/gjhkutgxc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/garajesga.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gcjjkzwyc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gpmopmokd.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gponuvjbx.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gypuhxbvw.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gamhlbfyv.sHtML

[F11] 复制与移动文件
来源：http://wap.fehbvm.com/Article/details/gapveiods.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gnticyxbf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gafsxqmxu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gntvzkvdh.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gmgbrwgny.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://mobile.hesvh.cn/Article/details/gvtowfxjz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://wap.zdbjq.cn/Article/details/gxernpkbg.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.zdbjq.cn/Article/details/gpedcrycj.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fehbvm.com/Article/details/gmtynpuhf.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gacadegti.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.fehbvm.com/Article/details/gkxqdzhgw.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/gcjhaptrk.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/ggfzesvvf.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gnhzotfku.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gkmverndm.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://baike.fehbvm.com/Article/details/gupxmpbqx.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.fehbvm.com/Article/details/gqgxocwpb.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.hesvh.cn/Article/details/gsxtjqesg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjuqozpws.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/grkszfnvu.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/giglgvsbh.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/gyldvwaak.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gykwtxsmy.sHtML

PHP:  class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gprfjqqvo.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/guwojvakm.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fehbvm.com/Article/details/gpwdwpule.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/ggzxfrncq.sHtML

Go:   type User struct { Name string }
来源：http://www.share.zdbjq.cn/Article/details/ggtkgrvrn.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/geqrnzcss.sHtML

C#:   class User {}
来源：http://m.share.fehbvm.com/Article/details/gbzzghlxh.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/ghzvfayma.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/gbjoqsszk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gvnqfyknx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gwfgpthbl.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/goveysqbo.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gwbqlfmsu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gfnqrqeqz.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gqxgdzggk.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.hesvh.cn/Article/details/gifoyuvvu.sHtML

[G03] 实例属性
来源：http://www.share.fehbvm.com/Article/details/godahfiqr.sHtML

Py:   self.name = "x"
来源：http://mobile.hesvh.cn/Article/details/gwqwcyvci.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gjjbeenmt.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/giktngsop.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gtynklrbz.sHtML

Java: private String name;
来源：http://3g.zdbjq.cn/Article/details/ggxtqawhk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://mobile.fehbvm.com/Article/details/gijkqvjgs.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gbvsygnzb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://baike.zdbjq.cn/Article/details/gmcdiyzpj.sHtML

[G04] 定义方法
来源：http://3g.fehbvm.com/Article/details/ginnmnoyk.sHtML

Py:   def greet(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/ghmjivaxp.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gmdjhiqeh.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gmqmuicoz.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gvwnebeul.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/guwsnqfme.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://read.share.hesvh.cn/Article/details/gjaepvcwk.sHtML

Ruby: def greet; @name; end
来源：http://blog.fehbvm.com/Article/details/gomycgqkv.sHtML

C#:   public string Greet() => Name;
来源：http://blog.fehbvm.com/Article/details/gglkeixvc.sHtML

[G05] 继承
来源：http://mobile.hesvh.cn/Article/details/gbidbogxb.sHtML

Py:   class Admin(User): pass
来源：http://www.blog.zdbjq.cn/Article/details/gyaennfwi.sHtML

PHP:  class Admin extends User {}
来源：http://m.share.fehbvm.com/Article/details/gkuknlvmn.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gpctkdahf.sHtML

TS:   class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gfpdnsnoz.sHtML

Java: class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/ghhlkqyvw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/gwqmsmifs.sHtML

Ruby: class Admin < User; end
来源：http://read.share.zdbjq.cn/Article/details/ggmutnbfh.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gdvjpdpxt.sHtML

[G06] 重写方法
来源：http://3g.fehbvm.com/Article/details/gowrcyvpr.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gbbmucsxl.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.blog.fehbvm.com/Article/details/gvspaoeea.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.zdbjq.cn/Article/details/gltbkfkae.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gftouyqdh.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gypamuafn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.fehbvm.com/Article/details/gdnllqfgn.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.hesvh.cn/Article/details/gesqwdvdr.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.zdbjq.cn/Article/details/gsxxbpwih.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/gcfdxzfwo.sHtML

Py:   super().greet()
来源：http://blog.hesvh.cn/Article/details/gdzqglprc.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gzzknlgwx.sHtML

JS:   super.greet();
来源：http://blog.zdbjq.cn/Article/details/gvfldxzqo.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gvvitoeuy.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gxengkdep.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/ggbvzbker.sHtML

Ruby: super
来源：http://www.share.hesvh.cn/Article/details/gfsfqjbmr.sHtML

C#:   base.Greet();
来源：http://m.share.hesvh.cn/Article/details/gwjfkxpwm.sHtML

[G08] 静态方法与属性
来源：http://3g.hesvh.cn/Article/details/gdwhvoows.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.hesvh.cn/Article/details/grnrixiem.sHtML

PHP:  public static function f() {}
来源：http://blog.fehbvm.com/Article/details/gyeflsdvq.sHtML

JS:   static f() {}
来源：http://m.share.zdbjq.cn/Article/details/gftatqomr.sHtML

TS:   static f(): void {}
来源：http://www.share.hesvh.cn/Article/details/gqfiqghxf.sHtML

Java: static void f() {}
来源：http://www.share.zdbjq.cn/Article/details/grkemuvtk.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.fehbvm.com/Article/details/gwalvikqj.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gbaehczcw.sHtML

C#:   public static void F() {}
来源：http://www.blog.zdbjq.cn/Article/details/glgrevtwc.sHtML

[G09] 接口 / 抽象类
来源：http://m.share.zdbjq.cn/Article/details/gclicbzex.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.zdbjq.cn/Article/details/gmsksxuhi.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gqhtgtiak.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.hesvh.cn/Article/details/gsxqffdnm.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.hesvh.cn/Article/details/gkmvyixpt.sHtML

Java: interface Shape { double area(); }
来源：http://blog.zdbjq.cn/Article/details/gtbtsvoqs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gxdigfqav.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.hesvh.cn/Article/details/gjnziwhci.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gkztsjlqm.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/ghwkkpszu.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://3g.fehbvm.com/Article/details/gtreorzyk.sHtML

PHP:  public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gyrdjqxys.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gulxijgkw.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gxahowdim.sHtML

Java: public / protected / private / 默认包级
来源：http://www.share.hesvh.cn/Article/details/gcfxxeuat.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.zdbjq.cn/Article/details/gtwlxeyrj.sHtML

Ruby: public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gxkaptcjn.sHtML

C#:   public / protected / private / internal
来源：http://baike.fehbvm.com/Article/details/gaciaokiw.sHtML

[G11] getter / setter
来源：http://3g.zdbjq.cn/Article/details/gcniykioz.sHtML

Py:   @property 与 @x.setter
来源：http://wap.hesvh.cn/Article/details/gkvjlmyyk.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://read.share.zdbjq.cn/Article/details/ghhuerhym.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gsladjlmh.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/glgfeoxzw.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/grhaclltw.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gvccbvogj.sHtML

Ruby: attr_accessor :name
来源：http://3g.hesvh.cn/Article/details/ggditfhda.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gqzsillil.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/grbwzzany.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gvnvrzrki.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gwgezwtct.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gzrzpyqgq.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gvpucjilm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gzlmiwlgz.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/goolmgenx.sHtML

Ruby: def to_s; @name; end
来源：http://read.share.fehbvm.com/Article/details/gflzfdkeu.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.fehbvm.com/Article/details/gtmjdnvys.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gkvvjevbx.sHtML

Py:   isinstance(u, User)
来源：http://read.share.fehbvm.com/Article/details/giscwtbht.sHtML

PHP:  $u instanceof User
来源：http://baike.fehbvm.com/Article/details/gdanqgnoa.sHtML

JS:   u instanceof User
来源：http://wap.fehbvm.com/Article/details/ghgzoawwm.sHtML

TS:   u instanceof User
来源：http://www.share.fehbvm.com/Article/details/gluvxnlqv.sHtML

Java: u instanceof User
来源：http://m.share.fehbvm.com/Article/details/ggugxalio.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.m.share.fehbvm.com/Article/details/gospebwgk.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/gfqwycoft.sHtML

C#:   u is User
来源：http://mobile.zdbjq.cn/Article/details/ghtbvavkj.sHtML

[G14] 数据类 / record
来源：http://www.m.share.hesvh.cn/Article/details/gzkprvyfv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://3g.hesvh.cn/Article/details/gmmfmgsil.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.share.zdbjq.cn/Article/details/gcpzdrowf.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gtedjtiif.sHtML

TS:   type User = { name: string; age: number };
来源：http://baike.hesvh.cn/Article/details/glapvgslx.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/gfcvehcho.sHtML

Go:   type User struct { Name string; Age int }
来源：http://3g.hesvh.cn/Article/details/gxevnbwte.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.hesvh.cn/Article/details/gflyxjsto.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.hesvh.cn/Article/details/gggsxshsq.sHtML

[G15] 枚举
来源：http://blog.hesvh.cn/Article/details/gevlfhgfl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://wap.fehbvm.com/Article/details/gqbhmuucy.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.hesvh.cn/Article/details/gjolmeitt.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.zdbjq.cn/Article/details/guiepuzaw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gxchsfalk.sHtML

Java: enum Color { RED, GREEN }
来源：http://m.share.zdbjq.cn/Article/details/gllpfgjux.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/gqjyulphk.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.fehbvm.com/Article/details/gtzilxasp.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.hesvh.cn/Article/details/gwemzcqnp.sHtML

[G16] 对象转数组 / 字典
来源：http://3g.hesvh.cn/Article/details/gdhnmuuir.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.fehbvm.com/Article/details/gwneqaosn.sHtML

PHP:  get_object_vars($obj);
来源：http://www.share.fehbvm.com/Article/details/grczpjuxy.sHtML

JS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gactimscy.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gnkbvydtw.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gjhtuhaqh.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.hesvh.cn/Article/details/gzlqcqbzc.sHtML

Ruby: obj.instance_variables
来源：http://baike.hesvh.cn/Article/details/grddabqfb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gdcwdigzq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsxewcjno.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gryypgwky.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gzsfjyodt.sHtML

[H01] try / catch 基础
来源：http://read.share.fehbvm.com/Article/details/gsxhvokmb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gqpwueucg.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.m.share.hesvh.cn/Article/details/glcroshdo.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gwpsejlig.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://3g.fehbvm.com/Article/details/gzoxsrfop.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/gnyffyitj.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mobile.hesvh.cn/Article/details/gulqfeziq.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://m.share.fehbvm.com/Article/details/gxbzbdues.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gjmqltket.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/gqqrrtkxc.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.hesvh.cn/Article/details/gzrudqnic.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gtgrayyvd.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gdshvhlod.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gyvelgkxb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gjubjtvxv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.blog.fehbvm.com/Article/details/gmvquybes.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gzacnawkl.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/glthmirbm.sHtML

[H03] 主动抛出异常
来源：http://www.share.fehbvm.com/Article/details/gcsgmsruw.sHtML

Py:   raise ValueError("错误信息")
来源：http://m.share.zdbjq.cn/Article/details/grvtxrsxm.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gsvgiexia.sHtML

JS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gceftqgju.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gpzsslbnc.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gbppginbg.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://3g.fehbvm.com/Article/details/gynejbczj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/gjiscyczz.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gbfpamspo.sHtML

[H04] 自定义异常类型
来源：http://3g.hesvh.cn/Article/details/gngdtasla.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.zdbjq.cn/Article/details/ghadatywi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/ghppxtfoq.sHtML

JS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/goebbvzlo.sHtML

TS:   class MyError extends Error {}
来源：http://www.share.fehbvm.com/Article/details/gphnzczkm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gsrowrwss.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://baike.hesvh.cn/Article/details/gdadzihyr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.hesvh.cn/Article/details/gqstrucvo.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gwtmwxlti.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/gwvvfdljq.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gduigxjhv.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://read.share.fehbvm.com/Article/details/gpfumdeik.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gvuihmkyc.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gqbdmawjw.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.hesvh.cn/Article/details/ggbvfoxjg.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://baike.zdbjq.cn/Article/details/ggrplhzoq.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gxqhervaj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://m.share.zdbjq.cn/Article/details/ggxbrvaag.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.zdbjq.cn/Article/details/gcnsqnsau.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.fehbvm.com/Article/details/gdiknjpyx.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gfukdsycf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.hesvh.cn/Article/details/gfrynmmge.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.hesvh.cn/Article/details/gbliiamov.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://mobile.zdbjq.cn/Article/details/gistfwyuw.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.zdbjq.cn/Article/details/gwggwrjjo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gvuldjszq.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/giqucnddp.sHtML

[H07] 断言
来源：http://www.m.share.hesvh.cn/Article/details/gbzaltgiz.sHtML

Py:   assert x > 0, "必须为正"
来源：http://blog.zdbjq.cn/Article/details/gpopdptwx.sHtML

PHP:  assert($x > 0);
来源：http://m.share.hesvh.cn/Article/details/gvkvcyofd.sHtML

JS:   console.assert(x > 0);
来源：http://wap.hesvh.cn/Article/details/gumkufsmn.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.fehbvm.com/Article/details/gpkzaoerk.sHtML

Java: assert x > 0 : "必须为正";
来源：http://read.share.zdbjq.cn/Article/details/gnlcfpwxu.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.hesvh.cn/Article/details/gertelxwe.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.fehbvm.com/Article/details/gjznxroha.sHtML

C#:   Debug.Assert(x > 0);
来源：http://3g.fehbvm.com/Article/details/gwxlwiktj.sHtML

[H08] 获取错误信息与堆栈
来源：http://wap.fehbvm.com/Article/details/gddfmzsqi.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gjmodfipk.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://baike.zdbjq.cn/Article/details/gdblvizhz.sHtML


<!-- 参考信息 -->