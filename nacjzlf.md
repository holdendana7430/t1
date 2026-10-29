代发 wailian999

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gfuxpqebi.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gxamnppsa.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gppyhkyba.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.fehbvm.com/Article/details/gpgozrkul.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://m.share.hesvh.cn/Article/details/gmlfukcxh.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.hesvh.cn/Article/details/gvgwnrrel.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gopsmcbli.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/gizvlyovg.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.fehbvm.com/Article/details/gsbhnjhcp.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.zdbjq.cn/Article/details/gawoundwo.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gezpkigjx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gbvyvxivc.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/geewzkxkl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gjdqrpdqa.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gvmyrmldt.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gsojwybny.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gycukrgqi.sHtML

[F06] 删除文件
来源：http://www.blog.zdbjq.cn/Article/details/gdmknvhou.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gpmtvqxzx.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmbcpohdw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gejrybbwi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gjksphzlz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gxdlljcmk.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gtcvhdrmk.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gdndliidu.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gwgxqvfpn.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gyuuusqjq.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.fehbvm.com/Article/details/gtpggeyhk.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://read.share.zdbjq.cn/Article/details/gdvzazgus.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/ggczqgwup.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gkqihxgym.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.fehbvm.com/Article/details/gtfhdsbwp.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.share.fehbvm.com/Article/details/gorbrgzgr.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/geidzworo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.zdbjq.cn/Article/details/gzxyqkjxi.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gimfmdvom.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.zdbjq.cn/Article/details/geiaephmr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gjiycmmfn.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gzajhyfzk.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gjmyhbltk.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gosgkcefs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.zdbjq.cn/Article/details/gaepermmt.sHtML

Ruby: Dir.children("dir")
来源：http://3g.zdbjq.cn/Article/details/goybbffbl.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.hesvh.cn/Article/details/getmedced.sHtML

[F09] 获取文件大小
来源：http://read.share.zdbjq.cn/Article/details/ghoogxkzi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzzgxozyh.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gnqhaamnj.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/ggxgpiwil.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.fehbvm.com/Article/details/gvnnoyimy.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.hesvh.cn/Article/details/ggufrojjp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fehbvm.com/Article/details/gtakxlkgn.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcxhsulyv.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://wap.zdbjq.cn/Article/details/gbzsyxdcs.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.zdbjq.cn/Article/details/gzjyjmfyn.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gurcsxuld.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/goedwbidj.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gccecovax.sHtML

TS:   path.extname("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gkyayluke.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.fehbvm.com/Article/details/gkuctojpr.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/govmekgpb.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gtredtskq.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.fehbvm.com/Article/details/gkyoqflxp.sHtML

[F11] 复制与移动文件
来源：http://blog.zdbjq.cn/Article/details/gqzcaweqh.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gznigjgrn.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/ghccgecqh.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gxgilznei.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/guodwllrl.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.hesvh.cn/Article/details/gimsebrtq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gczmmblvl.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjrxqtgoq.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gudhjawfn.sHtML

[F12] CSV 读写
来源：http://mobile.fehbvm.com/Article/details/gxviesczp.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.fehbvm.com/Article/details/gsjjtkikz.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.zdbjq.cn/Article/details/gvcjblygp.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.zdbjq.cn/Article/details/gzmjkgzzz.sHtML

TS:   // 同上
来源：http://mobile.fehbvm.com/Article/details/gixeyyvdz.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.zdbjq.cn/Article/details/gcuslerav.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.hesvh.cn/Article/details/gxwrovjol.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gluypqrhl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gjvqtpvgx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grmjdrklo.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gdbgabkpi.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gcaiopnip.sHtML

[G01] 定义类
来源：http://3g.hesvh.cn/Article/details/gmkiuxvad.sHtML

Py:   class User: pass
来源：http://mobile.zdbjq.cn/Article/details/ghofoyzyc.sHtML

PHP:  class User {}
来源：http://www.share.hesvh.cn/Article/details/gqpzwlivn.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gyglcszcn.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.fehbvm.com/Article/details/gnsjlboih.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gwyodigan.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gqxolmvfs.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/gxsvcxkwf.sHtML

C#:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjfaekzmx.sHtML

[G02] 构造函数
来源：http://www.share.hesvh.cn/Article/details/gssspgyyi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.fehbvm.com/Article/details/gumxlvnsz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://3g.zdbjq.cn/Article/details/gosqdzycu.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/gbukizkwo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.fehbvm.com/Article/details/gixggxpze.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/glhqbakzj.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gvivstpla.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gdtrvirsa.sHtML

C#:   public User(string name) { Name = name; }
来源：http://wap.zdbjq.cn/Article/details/gkgwmlacz.sHtML

[G03] 实例属性
来源：http://m.share.hesvh.cn/Article/details/gmjukyqwe.sHtML

Py:   self.name = "x"
来源：http://m.share.zdbjq.cn/Article/details/ggwcbltsu.sHtML

PHP:  public string $name = "x";
来源：http://3g.zdbjq.cn/Article/details/gumqxxbcz.sHtML

JS:   this.name = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gnseivqxx.sHtML

TS:   name: string = "x";
来源：http://m.share.hesvh.cn/Article/details/gzaajovdm.sHtML

Java: private String name;
来源：http://www.blog.zdbjq.cn/Article/details/goacbxbeb.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://read.share.zdbjq.cn/Article/details/gxqnpfgwo.sHtML

Ruby: @name = "x"
来源：http://www.blog.fehbvm.com/Article/details/gzuruahjc.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.hesvh.cn/Article/details/gthiypnhm.sHtML

[G04] 定义方法
来源：http://www.m.share.fehbvm.com/Article/details/gwlbsgydd.sHtML

Py:   def greet(self): return self.name
来源：http://wap.hesvh.cn/Article/details/gokwgjrzk.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.fehbvm.com/Article/details/gldlxpibp.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gbjjttpsh.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gecjakgzx.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/grbcyrlba.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.hesvh.cn/Article/details/gnruuhrix.sHtML

Ruby: def greet; @name; end
来源：http://blog.hesvh.cn/Article/details/gjosjclqd.sHtML

C#:   public string Greet() => Name;
来源：http://m.share.fehbvm.com/Article/details/gimhwaipq.sHtML

[G05] 继承
来源：http://www.share.zdbjq.cn/Article/details/gptgfgifw.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gjyyezeuu.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gjhnjcejt.sHtML

JS:   class Admin extends User {}
来源：http://wap.hesvh.cn/Article/details/gjltewgrn.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gggvqgbid.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gooyuvtrh.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.zdbjq.cn/Article/details/guetwqbnh.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gfbiodmyr.sHtML

C#:   class Admin : User {}
来源：http://wap.hesvh.cn/Article/details/gsggbbchy.sHtML

[G06] 重写方法
来源：http://wap.zdbjq.cn/Article/details/gphxkthsn.sHtML

Py:   def greet(self): return "admin"
来源：http://blog.hesvh.cn/Article/details/ghvnagwvj.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://baike.fehbvm.com/Article/details/gxcwoauxe.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gokjovmox.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gfuaepecc.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gjmcfrbyv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.hesvh.cn/Article/details/gdwxtioaj.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.hesvh.cn/Article/details/gkfnurnsx.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.share.zdbjq.cn/Article/details/gsnpvxrga.sHtML

[G07] 调用父类方法
来源：http://read.share.fehbvm.com/Article/details/gpeplepma.sHtML

Py:   super().greet()
来源：http://read.share.fehbvm.com/Article/details/gilyiyroz.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/goheotxem.sHtML

JS:   super.greet();
来源：http://read.share.hesvh.cn/Article/details/gkmfyiioy.sHtML

TS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gvbhrgcaa.sHtML

Java: super.greet();
来源：http://3g.hesvh.cn/Article/details/gpxsfeisp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.share.hesvh.cn/Article/details/ghfppgyjk.sHtML

Ruby: super
来源：http://mobile.zdbjq.cn/Article/details/gtdbgycrq.sHtML

C#:   base.Greet();
来源：http://3g.fehbvm.com/Article/details/gvpcafhtd.sHtML

[G08] 静态方法与属性
来源：http://baike.zdbjq.cn/Article/details/gnwmmralv.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.zdbjq.cn/Article/details/gsavprkby.sHtML

PHP:  public static function f() {}
来源：http://www.share.zdbjq.cn/Article/details/gvgbchtgl.sHtML

JS:   static f() {}
来源：http://wap.hesvh.cn/Article/details/gpdkcfcin.sHtML

TS:   static f(): void {}
来源：http://baike.zdbjq.cn/Article/details/gemzmwmbc.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gtfqcsozu.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://3g.hesvh.cn/Article/details/gpjwpyole.sHtML

Ruby: def self.f; end
来源：http://3g.hesvh.cn/Article/details/gnfkgdcah.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gspzbozlu.sHtML

[G09] 接口 / 抽象类
来源：http://www.m.share.fehbvm.com/Article/details/gtzctyrcu.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://3g.fehbvm.com/Article/details/gdeujanyt.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gbjzmkuzh.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.m.share.zdbjq.cn/Article/details/gsdzfmcoz.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.fehbvm.com/Article/details/gbqrfoope.sHtML

Java: interface Shape { double area(); }
来源：http://wap.fehbvm.com/Article/details/gxkbjhzfr.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://wap.fehbvm.com/Article/details/gartmyrnr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.blog.zdbjq.cn/Article/details/goaymftpp.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.hesvh.cn/Article/details/gnvjkxxjh.sHtML

[G10] 访问控制
来源：http://mobile.zdbjq.cn/Article/details/gbylcpndt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.fehbvm.com/Article/details/giqqygnfq.sHtML

PHP:  public / protected / private
来源：http://www.blog.fehbvm.com/Article/details/giebpwrxl.sHtML

JS:   #private 字段；其余公开
来源：http://m.share.hesvh.cn/Article/details/gctgopazq.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gkvzyedaa.sHtML

Java: public / protected / private / 默认包级
来源：http://blog.fehbvm.com/Article/details/gnzgtgyrz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.zdbjq.cn/Article/details/gtzduxoyu.sHtML

Ruby: public / protected / private
来源：http://www.share.fehbvm.com/Article/details/ghqeobqff.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/geyrntdrs.sHtML

[G11] getter / setter
来源：http://baike.fehbvm.com/Article/details/gqnhnirnw.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.hesvh.cn/Article/details/gsjzykjpb.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.hesvh.cn/Article/details/gheqzuqgu.sHtML

JS:   get name() { return this._name; }
来源：http://wap.fehbvm.com/Article/details/gcyzssafk.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjiubnmrz.sHtML

Java: public String getName() { return name; }
来源：http://wap.fehbvm.com/Article/details/glrrxydxt.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.share.fehbvm.com/Article/details/gjpssztrq.sHtML

Ruby: attr_accessor :name
来源：http://read.share.zdbjq.cn/Article/details/ggkakbphw.sHtML

C#:   public string Name { get; set; }
来源：http://www.blog.zdbjq.cn/Article/details/gmbemfpgr.sHtML

[G12] 对象转字符串
来源：http://baike.fehbvm.com/Article/details/gszfjuqqo.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.zdbjq.cn/Article/details/gzarcmgve.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gfukvsfay.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/ghlumpytp.sHtML

TS:   toString(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gcfvazlxs.sHtML

Java: @Override public String toString() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gaetzppki.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/gtvskrspu.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.fehbvm.com/Article/details/gfawvrnje.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.fehbvm.com/Article/details/gyihvyzsn.sHtML

[G13] 判断对象类型
来源：http://read.share.hesvh.cn/Article/details/gsnahxhsh.sHtML

Py:   isinstance(u, User)
来源：http://3g.zdbjq.cn/Article/details/gypwwadjh.sHtML

PHP:  $u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/ggtkqwhzt.sHtML

JS:   u instanceof User
来源：http://www.blog.hesvh.cn/Article/details/gxgzdyyhw.sHtML

TS:   u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gfjotnpys.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gamnvkbyz.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.hesvh.cn/Article/details/gvvnyybqo.sHtML

Ruby: u.is_a?(User)
来源：http://read.share.fehbvm.com/Article/details/gcnyohbme.sHtML

C#:   u is User
来源：http://baike.hesvh.cn/Article/details/gtoyfnjiu.sHtML

[G14] 数据类 / record
来源：http://wap.hesvh.cn/Article/details/gjpexlqok.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.zdbjq.cn/Article/details/gucpuykyj.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gkypevheu.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.fehbvm.com/Article/details/gqyajjguo.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.fehbvm.com/Article/details/gcveuxmmw.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.zdbjq.cn/Article/details/gjdlevwrl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gsjzjfwhd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.zdbjq.cn/Article/details/gfhddlugh.sHtML

C#:   record User(string Name, int Age);
来源：http://www.m.share.zdbjq.cn/Article/details/gbhvmcpwp.sHtML

[G15] 枚举
来源：http://mobile.fehbvm.com/Article/details/gohwkspjf.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.fehbvm.com/Article/details/gsqxlgrpv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gmoipuaje.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/glokbxvpg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gqipzzgdo.sHtML

Java: enum Color { RED, GREEN }
来源：http://wap.hesvh.cn/Article/details/gkrvoibhw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gjfxrocso.sHtML

Ruby: Color = %i[red green].freeze
来源：http://wap.hesvh.cn/Article/details/gfoewdfcd.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://m.share.fehbvm.com/Article/details/gmihskwkh.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gbtzfihgx.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/grhyurkxs.sHtML

PHP:  get_object_vars($obj);
来源：http://3g.zdbjq.cn/Article/details/gnxxftfiv.sHtML

JS:   Object.entries(obj)
来源：http://wap.hesvh.cn/Article/details/gmturiorf.sHtML

TS:   Object.entries(obj)
来源：http://3g.zdbjq.cn/Article/details/ghignouvp.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.zdbjq.cn/Article/details/goicdysxx.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.m.share.fehbvm.com/Article/details/gwdsbraom.sHtML

Ruby: obj.instance_variables
来源：http://blog.hesvh.cn/Article/details/gltyjiraa.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gygehlzdb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqxmyqmpt.sHtML

H. 异常与错误处理
来源：http://blog.hesvh.cn/Article/details/gyaupuiop.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggknlcvci.sHtML

[H01] try / catch 基础
来源：http://blog.zdbjq.cn/Article/details/gbyxxyccv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/ggbuakaez.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/galsfktul.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://baike.hesvh.cn/Article/details/gkrlnxkir.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.share.hesvh.cn/Article/details/gfvpkflcr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.hesvh.cn/Article/details/gnqqoxlot.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://read.share.zdbjq.cn/Article/details/gddtkkrcf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.fehbvm.com/Article/details/gujemapab.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.hesvh.cn/Article/details/gwspiipxn.sHtML

[H02] finally / ensure 收尾
来源：http://read.share.zdbjq.cn/Article/details/gelpihzxe.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gcubusbaf.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gmndkufpq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gtdtwdoyo.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://m.share.fehbvm.com/Article/details/gjwfiuxsp.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gfjhxaddn.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.hesvh.cn/Article/details/grfwzuevh.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://m.share.hesvh.cn/Article/details/ghkfltpwi.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/githxtxtk.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gtpexllor.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/ghkjwzczt.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gfkhhnfjz.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gdhxjavih.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.hesvh.cn/Article/details/gusvmqozx.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gsnekeshz.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.fehbvm.com/Article/details/gzwifzeaq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/glhxgcnpy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://mobile.fehbvm.com/Article/details/gddgoiuoh.sHtML

[H04] 自定义异常类型
来源：http://mobile.hesvh.cn/Article/details/gvskaxpll.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gizbgroyg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.fehbvm.com/Article/details/gljgrwlqk.sHtML

JS:   class MyError extends Error {}
来源：http://3g.hesvh.cn/Article/details/gicfpisdj.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggkzmaldo.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.fehbvm.com/Article/details/gqqoxpbpj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://read.share.zdbjq.cn/Article/details/gfbrdmyrv.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gthzyakwy.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.fehbvm.com/Article/details/gabjstojn.sHtML

[H05] 捕获特定类型
来源：http://mobile.zdbjq.cn/Article/details/gngwmxoid.sHtML

Py:   except ValueError as e:
来源：http://www.blog.fehbvm.com/Article/details/gzqlnkmvc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/gsuysvocn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.hesvh.cn/Article/details/glfonnxjs.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.fehbvm.com/Article/details/gredyiino.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.hesvh.cn/Article/details/ghtqebbqp.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/ghlshonbp.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/glyndvyhf.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://read.share.fehbvm.com/Article/details/gxexrgyxg.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.fehbvm.com/Article/details/gooxcabzk.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/geoxiudym.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gayfhgvry.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gbuywtnva.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/goxzjlsfu.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://baike.zdbjq.cn/Article/details/gefkhrrnp.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.fehbvm.com/Article/details/gmytjxycz.sHtML

Ruby: d&.dig(:a, :b)
来源：http://read.share.zdbjq.cn/Article/details/gsbkvspcy.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.zdbjq.cn/Article/details/guriuftvo.sHtML

[H07] 断言
来源：http://read.share.fehbvm.com/Article/details/gnmzkkcrj.sHtML

Py:   assert x > 0, "必须为正"
来源：http://read.share.hesvh.cn/Article/details/gqunhxiot.sHtML

PHP:  assert($x > 0);
来源：http://baike.fehbvm.com/Article/details/gyoopsunv.sHtML

JS:   console.assert(x > 0);
来源：http://www.m.share.fehbvm.com/Article/details/gnwpaeoda.sHtML

TS:   console.assert(x > 0);
来源：http://m.share.zdbjq.cn/Article/details/glqfbxnuc.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/guqtdwebl.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://blog.zdbjq.cn/Article/details/gkzdkdzrm.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://mobile.zdbjq.cn/Article/details/gqnyhslqy.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.zdbjq.cn/Article/details/ggmwqmkqt.sHtML

[H08] 获取错误信息与堆栈
来源：http://blog.fehbvm.com/Article/details/gdzfvzzar.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://3g.hesvh.cn/Article/details/gorjrbzhh.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.share.hesvh.cn/Article/details/gbjsnnfkn.sHtML

JS:   e.message;  e.stack
来源：http://m.share.zdbjq.cn/Article/details/grnagltkg.sHtML

TS:   e instanceof Error ? e.message : String(e)
来源：http://blog.zdbjq.cn/Article/details/gojyghtyi.sHtML

Java: e.getMessage();  e.printStackTrace()
来源：http://read.share.hesvh.cn/Article/details/ghxvylvou.sHtML

Go:   err.Error()
来源：http://www.blog.hesvh.cn/Article/details/gwivwowrb.sHtML


<!-- 参考信息 -->