代发 wailian999

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gkrhhmlsh.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://mobile.zdbjq.cn/Article/details/gnyosumip.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/ghubgvlhp.sHtML

[F04] 追加写入文件
来源：http://mobile.hesvh.cn/Article/details/gxjiwmyui.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gwxmuwkql.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gmoumfnqv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/ghubdmwpl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/guxromgxn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.zdbjq.cn/Article/details/grfqzfevg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gkcnqmbix.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.zdbjq.cn/Article/details/guplsonkq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/gnqzmrrth.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gfchnbyjc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.hesvh.cn/Article/details/gryrwndox.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gljvcsexv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ganohrmaj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtqdgzdfx.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gwjkxgkzq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/glrrmniot.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gfzmvopcn.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gnvsxthre.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gxryvvssq.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glioddgtm.sHtML

PHP:  unlink("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gbhwhvdgf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/grtygwhjq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gltkkipzj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gpojkfnml.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gedojrthk.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.hesvh.cn/Article/details/gmwxeupcb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gmueuejfi.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gbvmuxtqw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gjwooajws.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gxzspzvob.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gagrqrrhx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/goyfxbyhb.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gwuerytnl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/guwzpvzms.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/guwndjhel.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/grbnlarhx.sHtML

[F08] 遍历目录
来源：http://3g.zdbjq.cn/Article/details/gdmosntth.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.fehbvm.com/Article/details/gksmpndgi.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gpjroquyf.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/gjkfhjhyu.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gegqcvgku.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gxylqefki.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gwerrpmuq.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.zdbjq.cn/Article/details/guvwgmkdw.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/giticbqmx.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gjhkoxrau.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.zdbjq.cn/Article/details/guuqvpoqv.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/guwyzgtcf.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.zdbjq.cn/Article/details/gmnonvakd.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/gitrxsfrk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gzqdmzwij.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gdugwidrp.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gaokrfczy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.hesvh.cn/Article/details/gbdcxnhsd.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.share.fehbvm.com/Article/details/gaxevrttu.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gudiwosrn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gzjqxsdvx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gslfbranc.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwcyleltg.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gvgxmszso.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gldtfvanq.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/ggbmgepim.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/grzpouaex.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/gcglkmdzb.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.fehbvm.com/Article/details/guznkejek.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gnowmqudr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gwmigacnx.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gukhcgtas.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gflgaexno.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fehbvm.com/Article/details/gannjwfml.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwqrvjsai.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fehbvm.com/Article/details/gpfhwhjnz.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gdcimmpxq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://mobile.zdbjq.cn/Article/details/gejelsebl.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.m.share.zdbjq.cn/Article/details/grcwfcwxe.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.zdbjq.cn/Article/details/gwetiuacp.sHtML

TS:   // 同上
来源：http://read.share.fehbvm.com/Article/details/gfqlmcadn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.zdbjq.cn/Article/details/gpcqywdse.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gxtmhhllc.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gsvvrijug.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://3g.fehbvm.com/Article/details/gkyxgnkkc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpcbwtbpb.sHtML

G. 面向对象
来源：http://read.share.fehbvm.com/Article/details/grfruuxyg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gsvqkymha.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gtwjcbqmq.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/ggwconnph.sHtML

PHP:  class User {}
来源：http://www.blog.hesvh.cn/Article/details/gfettxopa.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gkuxmczim.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.zdbjq.cn/Article/details/gqwapcsza.sHtML

Java: class User {}
来源：http://mobile.zdbjq.cn/Article/details/ggwyapmyu.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gjrnhtkoi.sHtML

Ruby: class User; end
来源：http://www.m.share.fehbvm.com/Article/details/gjwmhhcfm.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gbixwdlye.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gxiluokff.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.hesvh.cn/Article/details/gfpynlfqn.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.hesvh.cn/Article/details/gpxhaxaqv.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://3g.fehbvm.com/Article/details/gjbgexgny.sHtML

TS:   constructor(public name: string) {}
来源：http://3g.zdbjq.cn/Article/details/gpcxqrlwv.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.zdbjq.cn/Article/details/gohpttcqh.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gfrzkfwdm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/grvekqenf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/geakessep.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/glbwirqea.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gxwnlqbyk.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gzzowjcpk.sHtML

JS:   this.name = "x";
来源：http://www.blog.hesvh.cn/Article/details/glrddflal.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/glcbbvtwr.sHtML

Java: private String name;
来源：http://www.share.zdbjq.cn/Article/details/gpqzvxewl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.fehbvm.com/Article/details/gohnswcsf.sHtML

Ruby: @name = "x"
来源：http://baike.zdbjq.cn/Article/details/gvahzydmp.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.hesvh.cn/Article/details/gzxykkdlw.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gfzszazah.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.hesvh.cn/Article/details/gajgepnkh.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://read.share.hesvh.cn/Article/details/gyvtnofrw.sHtML

JS:   greet() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gjccpjsex.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gocnyowbz.sHtML

Java: String greet() { return name; }
来源：http://blog.hesvh.cn/Article/details/gtymiwmbb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gswuankhi.sHtML

Ruby: def greet; @name; end
来源：http://m.share.zdbjq.cn/Article/details/ggwgvbgak.sHtML

C#:   public string Greet() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/guvuhvszi.sHtML

[G05] 继承
来源：http://wap.hesvh.cn/Article/details/gsqpcqvhc.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.hesvh.cn/Article/details/gpwpppsrc.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gaeuxtgaf.sHtML

JS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gufbotorb.sHtML

TS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gtzwzhmvx.sHtML

Java: class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gxywrmnxw.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/garifjjxy.sHtML

Ruby: class Admin < User; end
来源：http://baike.fehbvm.com/Article/details/gkzfynlci.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gmfjodxcd.sHtML

[G06] 重写方法
来源：http://3g.hesvh.cn/Article/details/gteymkmdr.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.hesvh.cn/Article/details/gzkvjinzy.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.zdbjq.cn/Article/details/gxppyxlgu.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.hesvh.cn/Article/details/gtbukzhlv.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gdscmhzmg.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/grjgfdmfb.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.m.share.hesvh.cn/Article/details/gkdacfiir.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gpzojgmht.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gowxpldje.sHtML

[G07] 调用父类方法
来源：http://www.blog.zdbjq.cn/Article/details/gwrjdhhgq.sHtML

Py:   super().greet()
来源：http://blog.zdbjq.cn/Article/details/gglczlaxs.sHtML

PHP:  parent::greet();
来源：http://mobile.hesvh.cn/Article/details/gkwufuvqh.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gsjadvmga.sHtML

TS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gevbfzmay.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/ggacqituj.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://wap.zdbjq.cn/Article/details/gggzogwph.sHtML

Ruby: super
来源：http://wap.zdbjq.cn/Article/details/gdnwaorwx.sHtML

C#:   base.Greet();
来源：http://www.share.fehbvm.com/Article/details/gtztstyay.sHtML

[G08] 静态方法与属性
来源：http://mobile.fehbvm.com/Article/details/gpoauvcje.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://m.share.fehbvm.com/Article/details/gdojjyhrx.sHtML

PHP:  public static function f() {}
来源：http://mobile.zdbjq.cn/Article/details/gnstcrkmi.sHtML

JS:   static f() {}
来源：http://mobile.hesvh.cn/Article/details/grrizkvtb.sHtML

TS:   static f(): void {}
来源：http://m.share.zdbjq.cn/Article/details/gfjlujbuj.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gwezmpygs.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://m.share.zdbjq.cn/Article/details/galgvbqnl.sHtML

Ruby: def self.f; end
来源：http://baike.zdbjq.cn/Article/details/gtnozmzhj.sHtML

C#:   public static void F() {}
来源：http://mobile.fehbvm.com/Article/details/gulwpxqau.sHtML

[G09] 接口 / 抽象类
来源：http://mobile.hesvh.cn/Article/details/gghejhiff.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.fehbvm.com/Article/details/gamqsivte.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.fehbvm.com/Article/details/gckeslbhe.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.fehbvm.com/Article/details/ggjmaniav.sHtML

TS:   interface Shape { area(): number; }
来源：http://m.share.hesvh.cn/Article/details/gtakicwee.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.zdbjq.cn/Article/details/gtrqdumnq.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://3g.zdbjq.cn/Article/details/gxebxfhtm.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.zdbjq.cn/Article/details/guzyeeocd.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gcfxxevfe.sHtML

[G10] 访问控制
来源：http://3g.zdbjq.cn/Article/details/gdwkssayt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.zdbjq.cn/Article/details/gghptdhfl.sHtML

PHP:  public / protected / private
来源：http://blog.fehbvm.com/Article/details/gnsrlnvem.sHtML

JS:   #private 字段；其余公开
来源：http://baike.fehbvm.com/Article/details/gyughjdqr.sHtML

TS:   public / protected / private
来源：http://baike.hesvh.cn/Article/details/gqqojaotg.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/gbzfxbojo.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.m.share.hesvh.cn/Article/details/gdugiuoxm.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gmylqavqn.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/geljcqjpz.sHtML

[G11] getter / setter
来源：http://read.share.fehbvm.com/Article/details/gqhizpags.sHtML

Py:   @property 与 @x.setter
来源：http://mobile.fehbvm.com/Article/details/gbedncrmo.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gomemxgdl.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/ghrpwevda.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.m.share.hesvh.cn/Article/details/gkippwspg.sHtML

Java: public String getName() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gmxjfemzm.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://3g.fehbvm.com/Article/details/gmpbtsjsv.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.hesvh.cn/Article/details/gqlkwtmur.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gfsnftqsz.sHtML

[G12] 对象转字符串
来源：http://mobile.hesvh.cn/Article/details/gqtqdklfo.sHtML

Py:   def __str__(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gugsgzbcp.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gdppflfhf.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gshvsatki.sHtML

TS:   toString(): string { return this.name; }
来源：http://m.share.hesvh.cn/Article/details/glbiohfwn.sHtML

Java: @Override public String toString() { return name; }
来源：http://baike.hesvh.cn/Article/details/gggztaokw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.fehbvm.com/Article/details/gocnrikzr.sHtML

Ruby: def to_s; @name; end
来源：http://www.blog.hesvh.cn/Article/details/glnjqqirk.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.hesvh.cn/Article/details/geudqvfde.sHtML

[G13] 判断对象类型
来源：http://www.share.hesvh.cn/Article/details/gkjwmaupl.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.fehbvm.com/Article/details/gjxfoyfwx.sHtML

PHP:  $u instanceof User
来源：http://wap.zdbjq.cn/Article/details/gmrgvnlcs.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gnezsqozy.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gctktquwb.sHtML

Java: u instanceof User
来源：http://3g.fehbvm.com/Article/details/goigzlosp.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.fehbvm.com/Article/details/gdqtdngpm.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gvgywhjjl.sHtML

C#:   u is User
来源：http://blog.zdbjq.cn/Article/details/guytesggj.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gzfmcjqrv.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gkyxmcvhz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://www.m.share.hesvh.cn/Article/details/gxxcagbjw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.zdbjq.cn/Article/details/gcdxktouw.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gtyqnsjub.sHtML

Java: record User(String name, int age) {}
来源：http://mobile.zdbjq.cn/Article/details/golzszjtw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gisrwctke.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.hesvh.cn/Article/details/gvigzwkhg.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.hesvh.cn/Article/details/gryorinee.sHtML

[G15] 枚举
来源：http://wap.zdbjq.cn/Article/details/gdhjygpyx.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.fehbvm.com/Article/details/gjlitlvrf.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://mobile.zdbjq.cn/Article/details/gvvamsndn.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.blog.fehbvm.com/Article/details/glswngznt.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/ggxjemxic.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.fehbvm.com/Article/details/gunhnkqey.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/gxfcnxuoo.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.blog.zdbjq.cn/Article/details/gtmeupikv.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/grnvnmdko.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.fehbvm.com/Article/details/gqsqycrme.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://blog.hesvh.cn/Article/details/gnbengpiq.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.fehbvm.com/Article/details/ggqpelsuj.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gpccfwxzj.sHtML

TS:   Object.entries(obj)
来源：http://www.share.fehbvm.com/Article/details/gnobyrtlg.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gspsngaqf.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://mobile.zdbjq.cn/Article/details/gjyvtzkuo.sHtML

Ruby: obj.instance_variables
来源：http://www.blog.hesvh.cn/Article/details/gcevmldvx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gzymffznp.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gebnnzqko.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gyuqakcoz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggmqzrqlb.sHtML

[H01] try / catch 基础
来源：http://www.m.share.hesvh.cn/Article/details/gqxtbapjx.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gzladyylx.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://m.share.fehbvm.com/Article/details/gwahfvzpj.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gddzysvio.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gfvrxnadz.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.share.hesvh.cn/Article/details/gxeiqyczi.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.hesvh.cn/Article/details/gyousfgga.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://3g.zdbjq.cn/Article/details/gpjnaexaz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.hesvh.cn/Article/details/gfpuhpaxu.sHtML

[H02] finally / ensure 收尾
来源：http://www.m.share.zdbjq.cn/Article/details/gshbqvisq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.share.zdbjq.cn/Article/details/glmycnfzd.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.fehbvm.com/Article/details/gxgolpjyf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gljewmzfr.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gwsshqrkb.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gmfoxlusy.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.fehbvm.com/Article/details/gjrxjzvfn.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://blog.zdbjq.cn/Article/details/gpdvkrsbz.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ghkogasdy.sHtML

[H03] 主动抛出异常
来源：http://mobile.hesvh.cn/Article/details/gmrownrpa.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.fehbvm.com/Article/details/gavgsvynx.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gqwbhvmbj.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.fehbvm.com/Article/details/gvptcqbwf.sHtML

TS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gtfvajcvn.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gmfaqvcat.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gnlwsrlux.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://m.share.hesvh.cn/Article/details/gvnlcvwed.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gdppsoohd.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/ggeeclxap.sHtML

Py:   class MyError(Exception): pass
来源：http://blog.hesvh.cn/Article/details/gacakqubf.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.blog.hesvh.cn/Article/details/gxwywbmto.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/ggkwymgrw.sHtML

TS:   class MyError extends Error {}
来源：http://read.share.zdbjq.cn/Article/details/gkonaybgf.sHtML

Java: class MyException extends RuntimeException {}
来源：http://blog.zdbjq.cn/Article/details/giuvquvjb.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://3g.hesvh.cn/Article/details/gcrkzwntl.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gzmmkzhyn.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/geihhqrdq.sHtML

[H05] 捕获特定类型
来源：http://www.share.hesvh.cn/Article/details/gbkkpfhkw.sHtML

Py:   except ValueError as e:
来源：http://wap.zdbjq.cn/Article/details/gfrhzkicc.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://blog.zdbjq.cn/Article/details/gmkjushcy.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://baike.zdbjq.cn/Article/details/gktwxxtbb.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.fehbvm.com/Article/details/gvcrithfn.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://wap.fehbvm.com/Article/details/gjdneuebq.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gzmakfmsd.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.zdbjq.cn/Article/details/gtlvkrfxm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gvntksozx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.zdbjq.cn/Article/details/gmqnvdlad.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.fehbvm.com/Article/details/glnmmblnf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gwddmcjrf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.fehbvm.com/Article/details/gcujfdcxj.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://3g.zdbjq.cn/Article/details/grosxvrdo.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://wap.fehbvm.com/Article/details/ghzrikcpx.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://blog.hesvh.cn/Article/details/gdfuurnvo.sHtML

Ruby: d&.dig(:a, :b)
来源：http://m.share.hesvh.cn/Article/details/guoxuijgc.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.share.zdbjq.cn/Article/details/gucrsjzgy.sHtML

[H07] 断言
来源：http://baike.hesvh.cn/Article/details/gaxcjedyx.sHtML

Py:   assert x > 0, "必须为正"
来源：http://www.blog.fehbvm.com/Article/details/giyafsfam.sHtML

PHP:  assert($x > 0);
来源：http://www.share.zdbjq.cn/Article/details/gxsyoxjki.sHtML

JS:   console.assert(x > 0);
来源：http://mobile.zdbjq.cn/Article/details/gugaxmjcm.sHtML

TS:   console.assert(x > 0);
来源：http://read.share.hesvh.cn/Article/details/ghiegxugn.sHtML

Java: assert x > 0 : "必须为正";
来源：http://mobile.hesvh.cn/Article/details/gmtxeihuz.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://baike.fehbvm.com/Article/details/gttaafkuy.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://baike.zdbjq.cn/Article/details/gzkosydso.sHtML

C#:   Debug.Assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/gedqlcfoy.sHtML

[H08] 获取错误信息与堆栈
来源：http://m.share.fehbvm.com/Article/details/gkpkgvudm.sHtML

Py:   str(e);  traceback.format_exc()
来源：http://m.share.hesvh.cn/Article/details/gyzicogdb.sHtML

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://www.blog.hesvh.cn/Article/details/geruubrmd.sHtML


<!-- 参考信息 -->