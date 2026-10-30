代发 wailian999

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.zdbjq.cn/Article/details/ggvbmeoqe.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gfpiqsjjl.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gdyivsgqu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.hesvh.cn/Article/details/gyvukfafy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gacrcxqek.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gahnayplp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gbjjsujmf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/ggqggqlel.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gawjfdgws.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.fehbvm.com/Article/details/gmpqdrfms.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gbbyafyrf.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fehbvm.com/Article/details/gwuuenmwv.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gpogkhfeq.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gnvvnzguu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gsbskprwt.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/grizvgoxl.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gnvomklnp.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gukzuzgum.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fehbvm.com/Article/details/gknvzkkwc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.fehbvm.com/Article/details/gqfzvonuf.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gagmwyydh.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://mobile.fehbvm.com/Article/details/ghwykpyhs.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gokibnsrp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gosxymfmt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/glgkfasbl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gpotswxce.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/gqeqvnfbf.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gtikwdltr.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpeqvleyi.sHtML

[F06] 删除文件
来源：http://baike.fehbvm.com/Article/details/gxpzedgbo.sHtML

Py:   os.remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/grhswefam.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gdssolmpc.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fehbvm.com/Article/details/gsvmubpwe.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/glnxxwtbs.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gqowclyid.sHtML

Go:   os.Remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gezszvptc.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gpmcsidhh.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gcswuewpk.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gokkrofni.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://m.share.fehbvm.com/Article/details/gmcutnqub.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.hesvh.cn/Article/details/gtnomismv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gnvuwoeay.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gotnwodyi.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gxfrqsnzy.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gzfyveftk.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.hesvh.cn/Article/details/gelphnsil.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.fehbvm.com/Article/details/gridadegy.sHtML

[F08] 遍历目录
来源：http://m.share.zdbjq.cn/Article/details/gjalbowku.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/ghgyvjxfz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.zdbjq.cn/Article/details/gkgdphyxy.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gacltnzbv.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.zdbjq.cn/Article/details/giztiscxv.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gljrwoftd.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gxtjsdtja.sHtML

Ruby: Dir.children("dir")
来源：http://wap.fehbvm.com/Article/details/gtrvsrtbt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.zdbjq.cn/Article/details/garjehefa.sHtML

[F09] 获取文件大小
来源：http://m.share.zdbjq.cn/Article/details/gugvllkxc.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gufnhueuz.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gtfwcanhz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/grbwmdzsi.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.fehbvm.com/Article/details/ghqcynbuq.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gekiviloq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.fehbvm.com/Article/details/gukbzsxey.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/glfxxcmge.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://3g.zdbjq.cn/Article/details/gwlzdgngo.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gorklxcvu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gtcgyrbil.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.fehbvm.com/Article/details/gunjgpqqg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gslywveuv.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gzktlnbpc.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://3g.fehbvm.com/Article/details/gfeugofpj.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gcywzmpfi.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gamekhmov.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gdzxiotqg.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmladzgty.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpscukauf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.fehbvm.com/Article/details/gfxjpxocv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gsvsbokpr.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gkkvbpaqo.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://3g.fehbvm.com/Article/details/gcpjrnavi.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gwuezdrfx.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gghrebwlz.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.m.share.fehbvm.com/Article/details/gjxxqtwju.sHtML

[F12] CSV 读写
来源：http://mobile.zdbjq.cn/Article/details/gxwtdrrel.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.fehbvm.com/Article/details/gluzuedzq.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://m.share.zdbjq.cn/Article/details/gglkcjiqs.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.zdbjq.cn/Article/details/gouvbdxrh.sHtML

TS:   // 同上
来源：http://wap.fehbvm.com/Article/details/gyvvznpfi.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/givpatekl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/gkaztcklu.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gsrlyxdcu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/grgymidzx.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnkqyusft.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/guszcymqx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwtywdwhr.sHtML

[G01] 定义类
来源：http://www.blog.fehbvm.com/Article/details/gshxdgedt.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gchgeuawl.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/giqeniwrt.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gobwqbkxl.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gprrygnhn.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gyihjdgwt.sHtML

Go:   type User struct { Name string }
来源：http://m.share.hesvh.cn/Article/details/gjtywofje.sHtML

Ruby: class User; end
来源：http://baike.fehbvm.com/Article/details/gzbsfqfsr.sHtML

C#:   class User {}
来源：http://blog.hesvh.cn/Article/details/gfucsxybv.sHtML

[G02] 构造函数
来源：http://read.share.zdbjq.cn/Article/details/gjgedwoaw.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/grlarsqtz.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/goyhclsqd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.hesvh.cn/Article/details/gurbhnazi.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.zdbjq.cn/Article/details/gyqztfesv.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gkvuiajyh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.hesvh.cn/Article/details/gkhoaksiv.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.blog.zdbjq.cn/Article/details/gwksdfmaj.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.hesvh.cn/Article/details/gkorituqz.sHtML

[G03] 实例属性
来源：http://blog.zdbjq.cn/Article/details/gqixwnxae.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gtcgwktis.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/gbeqdsmal.sHtML

JS:   this.name = "x";
来源：http://blog.zdbjq.cn/Article/details/gcwddrcyp.sHtML

TS:   name: string = "x";
来源：http://blog.hesvh.cn/Article/details/gtvhgsxxr.sHtML

Java: private String name;
来源：http://www.m.share.zdbjq.cn/Article/details/gvtwuzvqk.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/guhtaxfsk.sHtML

Ruby: @name = "x"
来源：http://www.share.fehbvm.com/Article/details/grtfvugae.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.share.hesvh.cn/Article/details/gyguqbchp.sHtML

[G04] 定义方法
来源：http://3g.zdbjq.cn/Article/details/ggsumpdjn.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gdgzznbum.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.fehbvm.com/Article/details/gzatlzyap.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/ghvgsvtfv.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.hesvh.cn/Article/details/gkkwzhzbd.sHtML

Java: String greet() { return name; }
来源：http://blog.fehbvm.com/Article/details/gvylvyxcq.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.fehbvm.com/Article/details/gkvyjmixo.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gwspohdko.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/gfabffwbg.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/gevsfilth.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gjknvpoyc.sHtML

PHP:  class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gzruepsgh.sHtML

JS:   class Admin extends User {}
来源：http://3g.fehbvm.com/Article/details/gwrrwpjfz.sHtML

TS:   class Admin extends User {}
来源：http://www.share.fehbvm.com/Article/details/geuolcqgi.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gxniesgxu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gatupfjpl.sHtML

Ruby: class Admin < User; end
来源：http://3g.fehbvm.com/Article/details/ggpcukjqp.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gaofvuhgk.sHtML

[G06] 重写方法
来源：http://blog.zdbjq.cn/Article/details/gganbdmhn.sHtML

Py:   def greet(self): return "admin"
来源：http://3g.zdbjq.cn/Article/details/gucrnlbth.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gozlaufak.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gaccmdkgp.sHtML

TS:   greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gfjruqwgz.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gpgdttbqo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.zdbjq.cn/Article/details/gcvghzays.sHtML

Ruby: def greet; "admin"; end
来源：http://www.m.share.zdbjq.cn/Article/details/gqbwupxzy.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gvzpprrqj.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gvldvbpyn.sHtML

Py:   super().greet()
来源：http://read.share.hesvh.cn/Article/details/gjizeuiya.sHtML

PHP:  parent::greet();
来源：http://wap.fehbvm.com/Article/details/gomqacgai.sHtML

JS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gqtvnnnbt.sHtML

TS:   super.greet();
来源：http://www.m.share.hesvh.cn/Article/details/gnriruwxp.sHtML

Java: super.greet();
来源：http://www.share.hesvh.cn/Article/details/gvmdarteo.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.zdbjq.cn/Article/details/gfmrtgafm.sHtML

Ruby: super
来源：http://www.blog.hesvh.cn/Article/details/gvlvfjqba.sHtML

C#:   base.Greet();
来源：http://wap.fehbvm.com/Article/details/gsjqrzate.sHtML

[G08] 静态方法与属性
来源：http://blog.fehbvm.com/Article/details/glomvrqjo.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.fehbvm.com/Article/details/goejpgxxk.sHtML

PHP:  public static function f() {}
来源：http://m.share.fehbvm.com/Article/details/gaicovzks.sHtML

JS:   static f() {}
来源：http://www.blog.fehbvm.com/Article/details/grubacfyi.sHtML

TS:   static f(): void {}
来源：http://www.blog.fehbvm.com/Article/details/gqxrktpnz.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gsdnqvkkd.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/gekhjygwy.sHtML

Ruby: def self.f; end
来源：http://3g.fehbvm.com/Article/details/gbkanjjtm.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gialvjtnu.sHtML

[G09] 接口 / 抽象类
来源：http://blog.fehbvm.com/Article/details/gndqrdbll.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.fehbvm.com/Article/details/gtjhvkssp.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://wap.fehbvm.com/Article/details/gfgzeftjq.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://wap.hesvh.cn/Article/details/gilxmjiky.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.hesvh.cn/Article/details/gyjeqxtsf.sHtML

Java: interface Shape { double area(); }
来源：http://mobile.hesvh.cn/Article/details/guseqmgva.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://m.share.fehbvm.com/Article/details/gtakqcvvr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/ggwwzgwgo.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gdkijlesz.sHtML

[G10] 访问控制
来源：http://m.share.fehbvm.com/Article/details/ggmdltlee.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.m.share.hesvh.cn/Article/details/gkncdzizs.sHtML

PHP:  public / protected / private
来源：http://www.share.zdbjq.cn/Article/details/gbqdugqjx.sHtML

JS:   #private 字段；其余公开
来源：http://blog.fehbvm.com/Article/details/gigumarbu.sHtML

TS:   public / protected / private
来源：http://wap.hesvh.cn/Article/details/gnaumbisu.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.hesvh.cn/Article/details/gdfmsgrnz.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://wap.zdbjq.cn/Article/details/gnkmjyxgy.sHtML

Ruby: public / protected / private
来源：http://www.share.hesvh.cn/Article/details/giguqlfxk.sHtML

C#:   public / protected / private / internal
来源：http://baike.hesvh.cn/Article/details/gwalokrkg.sHtML

[G11] getter / setter
来源：http://www.share.fehbvm.com/Article/details/gdpjeplyv.sHtML

Py:   @property 与 @x.setter
来源：http://blog.hesvh.cn/Article/details/gxrfdjqyx.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpmslriga.sHtML

JS:   get name() { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gcxefnajr.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.zdbjq.cn/Article/details/gihngyhit.sHtML

Java: public String getName() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdlqsdzo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/geztkjuyk.sHtML

Ruby: attr_accessor :name
来源：http://wap.fehbvm.com/Article/details/ghaoslxry.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.hesvh.cn/Article/details/gnnnydyvf.sHtML

[G12] 对象转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxddhbauk.sHtML

Py:   def __str__(self): return self.name
来源：http://m.share.hesvh.cn/Article/details/ghppqltcm.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gvtetdabl.sHtML

JS:   toString() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gfrheciko.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gakpvjwpl.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.fehbvm.com/Article/details/gfewjypwn.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/goreqtzid.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gjizzilka.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gjbvkuwpe.sHtML

[G13] 判断对象类型
来源：http://www.m.share.zdbjq.cn/Article/details/gnqcynlsx.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/glzoycagk.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gslufsrmm.sHtML

JS:   u instanceof User
来源：http://baike.fehbvm.com/Article/details/gosuknijr.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/ghvpoipcn.sHtML

Java: u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gkutygyuv.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gbiqhctqq.sHtML

Ruby: u.is_a?(User)
来源：http://www.m.share.hesvh.cn/Article/details/gwznzvzmm.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gvmqcdmkn.sHtML

[G14] 数据类 / record
来源：http://wap.zdbjq.cn/Article/details/gyzxlmmql.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.zdbjq.cn/Article/details/gvxynnvfq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://mobile.fehbvm.com/Article/details/gajmptdlj.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.blog.zdbjq.cn/Article/details/gihernppg.sHtML

TS:   type User = { name: string; age: number };
来源：http://3g.fehbvm.com/Article/details/gehdpsouj.sHtML

Java: record User(String name, int age) {}
来源：http://wap.fehbvm.com/Article/details/gmenvjirt.sHtML

Go:   type User struct { Name string; Age int }
来源：http://read.share.fehbvm.com/Article/details/gsxlgkkfw.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.hesvh.cn/Article/details/gqajfcmnj.sHtML

C#:   record User(string Name, int Age);
来源：http://3g.zdbjq.cn/Article/details/gmtqyavuj.sHtML

[G15] 枚举
来源：http://baike.fehbvm.com/Article/details/gsulqsxus.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.hesvh.cn/Article/details/gnrbxlmld.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/ghodnjcdq.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://read.share.fehbvm.com/Article/details/gqwlhpbil.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.fehbvm.com/Article/details/gihpgqhtw.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.fehbvm.com/Article/details/ggvplrewg.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/gatguuthg.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gqthcslir.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gvkipdxcq.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gtjkhshun.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/grpwawjek.sHtML

PHP:  get_object_vars($obj);
来源：http://baike.fehbvm.com/Article/details/gdwayhsee.sHtML

JS:   Object.entries(obj)
来源：http://wap.fehbvm.com/Article/details/gayurakng.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gbjirucbj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.m.share.hesvh.cn/Article/details/gepzawocg.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://blog.zdbjq.cn/Article/details/ghcbyqgeg.sHtML

Ruby: obj.instance_variables
来源：http://wap.zdbjq.cn/Article/details/gqfebkkoz.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/gitjzmusx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwhkmlcca.sHtML

H. 异常与错误处理
来源：http://www.share.fehbvm.com/Article/details/gzmufshpw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gtrrispsp.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gjmalzngg.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gzmqehtsk.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.fehbvm.com/Article/details/gztrafsvz.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gcxtgirif.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gsyoevpaa.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://blog.hesvh.cn/Article/details/glmqwflmr.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://3g.hesvh.cn/Article/details/gcoeugbso.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.hesvh.cn/Article/details/ggazbnoqa.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://blog.zdbjq.cn/Article/details/giyqntami.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.hesvh.cn/Article/details/gheyzmfbd.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://baike.zdbjq.cn/Article/details/gvcvdpxeg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gltotngic.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/guklqmjdk.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://baike.fehbvm.com/Article/details/gtrmkfeht.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/glidtbeur.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://3g.fehbvm.com/Article/details/gmsayxcwd.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://baike.zdbjq.cn/Article/details/gnnkfzxje.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gavwehheq.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gcemsdyvc.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.m.share.hesvh.cn/Article/details/gzfgdiopd.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gtmyawjrn.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/ggrjucorq.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/gqqmjudzq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gjhswneey.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gtfgzvmwz.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/grlpiuduh.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gtqdbhwjq.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gydpgsbfk.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.zdbjq.cn/Article/details/giievxjzu.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/gjypihdwd.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/getzraews.sHtML

TS:   class MyError extends Error {}
来源：http://baike.hesvh.cn/Article/details/gluebxnne.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/griysiaqz.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gbgxcrgar.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.fehbvm.com/Article/details/gtvicinxa.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gzzcwslah.sHtML

[H05] 捕获特定类型
来源：http://read.share.zdbjq.cn/Article/details/gafcuhroz.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/ggughkzlx.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://3g.fehbvm.com/Article/details/gcwckwgzz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gjgnbssgm.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.fehbvm.com/Article/details/gapdfyyxg.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.hesvh.cn/Article/details/ggizqzycm.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.fehbvm.com/Article/details/gtcjqqvuc.sHtML

Ruby: rescue ArgumentError => e
来源：http://wap.hesvh.cn/Article/details/gukbzyknc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.fehbvm.com/Article/details/gofljralu.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gzdasamig.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.hesvh.cn/Article/details/gizvjtcek.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.hesvh.cn/Article/details/gvshyuamj.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://wap.hesvh.cn/Article/details/gurvztpbt.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.zdbjq.cn/Article/details/glmptptmp.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.hesvh.cn/Article/details/gdysvxoqk.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://mobile.fehbvm.com/Article/details/gdiuwmjno.sHtML

Ruby: d&.dig(:a, :b)
来源：http://baike.zdbjq.cn/Article/details/gsqubsuyv.sHtML

C#:   obj?.A?.B ?? default
来源：http://mobile.zdbjq.cn/Article/details/gaimklnwk.sHtML

[H07] 断言
来源：http://m.share.hesvh.cn/Article/details/ghwuxsqtk.sHtML

Py:   assert x > 0, "必须为正"
来源：http://wap.hesvh.cn/Article/details/ghjeabqjd.sHtML

PHP:  assert($x > 0);
来源：http://wap.zdbjq.cn/Article/details/gghyabtwf.sHtML

JS:   console.assert(x > 0);
来源：http://wap.fehbvm.com/Article/details/gwrvrmwnl.sHtML


<!-- 参考信息 -->