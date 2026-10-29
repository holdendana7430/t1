代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/granguone.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gpvvuacdp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gdkgtpled.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/giqcuridq.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.hesvh.cn/Article/details/gtbacngkr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.fehbvm.com/Article/details/gpxwtzpax.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/godiwyokr.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/ghmofeogm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/glgiaqpcv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fehbvm.com/Article/details/gcfndalwr.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/glryakgps.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gjeiavhsb.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://wap.zdbjq.cn/Article/details/gfytulvfk.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fehbvm.com/Article/details/gdruqccak.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/ghdujhtxj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gntdreuti.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.hesvh.cn/Article/details/ggpynalsf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.zdbjq.cn/Article/details/gtqdmewvu.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/glpweqbhc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/geunzjyxe.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gsrzmzqkp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gjzrtatfs.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.zdbjq.cn/Article/details/gtolvmemz.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gshrojpgn.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.hesvh.cn/Article/details/ggupwtitv.sHtML

[F06] 删除文件
来源：http://wap.zdbjq.cn/Article/details/glsizslnn.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwtautcuz.sHtML

PHP:  unlink("a.txt");
来源：http://blog.zdbjq.cn/Article/details/gqmrmwtlf.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqnnzwnse.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gkakxjuvi.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gmbknxlxd.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gzmgnyugd.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gtegzyxno.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gdrbwxzbb.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/gwireudvs.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.zdbjq.cn/Article/details/gupbdvljg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.share.fehbvm.com/Article/details/gxigdktbw.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/givfllxzu.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gjabpxeiq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gkkeubyjd.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/gzostbuzd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.zdbjq.cn/Article/details/gveacvtjx.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gtphfkusm.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/grqsddwqe.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gpyqxdevf.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.fehbvm.com/Article/details/gvdgsppld.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/guptehvfu.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.zdbjq.cn/Article/details/gsjanvzij.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gfgfzcgya.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/giuyxadkx.sHtML

Ruby: Dir.children("dir")
来源：http://baike.fehbvm.com/Article/details/gcphfxbjg.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gsxhblhij.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gzfercdur.sHtML

Py:   os.path.getsize("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gxyrsydcb.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.hesvh.cn/Article/details/ghwxaldse.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.hesvh.cn/Article/details/giqyubajq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gtxjexrlu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gwgudrytb.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fehbvm.com/Article/details/gtcsnxfow.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gnmmkmeyw.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.fehbvm.com/Article/details/ghecmcilj.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.zdbjq.cn/Article/details/gztohdkid.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/gdbiogbah.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/grloxzvxm.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gnhcjgval.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gmdswqwcw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.fehbvm.com/Article/details/gsswxtdog.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gwelxtsvc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gawmukrsa.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gygiscizu.sHtML

[F11] 复制与移动文件
来源：http://3g.zdbjq.cn/Article/details/gaqirbysx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gjnquochs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/gtvuufrdu.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gmdnintoo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gzqdtuxhw.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gsiqfuxrn.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.hesvh.cn/Article/details/gwderaqgb.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gzdumfffe.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.zdbjq.cn/Article/details/gyvriioef.sHtML

[F12] CSV 读写
来源：http://wap.hesvh.cn/Article/details/gtidrgxor.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.hesvh.cn/Article/details/gjvwbqaae.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/guabropus.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.hesvh.cn/Article/details/gpafvkwpy.sHtML

TS:   // 同上
来源：http://www.blog.fehbvm.com/Article/details/gzkngonne.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gxalukowl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.fehbvm.com/Article/details/gqevglslg.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gywicazmm.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://baike.zdbjq.cn/Article/details/gbzlldiji.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gfypwfexv.sHtML

G. 面向对象
来源：http://3g.zdbjq.cn/Article/details/gezymvyjc.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glvchtfxv.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gzqrsuovt.sHtML

Py:   class User: pass
来源：http://blog.hesvh.cn/Article/details/gofkkesof.sHtML

PHP:  class User {}
来源：http://baike.fehbvm.com/Article/details/gevfsfavk.sHtML

JS:   class User {}
来源：http://www.m.share.fehbvm.com/Article/details/gqelqtbzv.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gcrktjmla.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/grdqcdkhu.sHtML

Go:   type User struct { Name string }
来源：http://3g.zdbjq.cn/Article/details/gmcdukikh.sHtML

Ruby: class User; end
来源：http://read.share.zdbjq.cn/Article/details/ggjvyinre.sHtML

C#:   class User {}
来源：http://www.blog.zdbjq.cn/Article/details/gdoyurphf.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/ghgkjpfbk.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.zdbjq.cn/Article/details/ggrtznjdg.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://blog.zdbjq.cn/Article/details/glsuizvjc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gnekplepj.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.zdbjq.cn/Article/details/gqoirqpej.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gmwqfelrs.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.fehbvm.com/Article/details/grqzmlhjq.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/gbmnhlhbf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gbtskevqg.sHtML

[G03] 实例属性
来源：http://wap.hesvh.cn/Article/details/graiedyvg.sHtML

Py:   self.name = "x"
来源：http://baike.fehbvm.com/Article/details/gcklgnbsy.sHtML

PHP:  public string $name = "x";
来源：http://read.share.zdbjq.cn/Article/details/gpcffmbdt.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gnzpbaxhv.sHtML

TS:   name: string = "x";
来源：http://m.share.zdbjq.cn/Article/details/ggxfndrfd.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gfaxmzzim.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.fehbvm.com/Article/details/gryfekowm.sHtML

Ruby: @name = "x"
来源：http://mobile.zdbjq.cn/Article/details/guhjtzglx.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://wap.zdbjq.cn/Article/details/gmydqkabh.sHtML

[G04] 定义方法
来源：http://wap.fehbvm.com/Article/details/gxsngkmfn.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/glmlvxrbt.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.hesvh.cn/Article/details/gyjskojer.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.zdbjq.cn/Article/details/gnkptnlux.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/giipejoiu.sHtML

Java: String greet() { return name; }
来源：http://mobile.hesvh.cn/Article/details/ggydxzosn.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.fehbvm.com/Article/details/gxzflstos.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/gnwjcskwn.sHtML

C#:   public string Greet() => Name;
来源：http://www.share.hesvh.cn/Article/details/gsitnhexi.sHtML

[G05] 继承
来源：http://m.share.hesvh.cn/Article/details/gapieynvs.sHtML

Py:   class Admin(User): pass
来源：http://mobile.hesvh.cn/Article/details/ggzzkdamj.sHtML

PHP:  class Admin extends User {}
来源：http://wap.zdbjq.cn/Article/details/glxgzkrqr.sHtML

JS:   class Admin extends User {}
来源：http://3g.zdbjq.cn/Article/details/gbgvkmhtt.sHtML

TS:   class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gfgmclblh.sHtML

Java: class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gmirroltc.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.blog.zdbjq.cn/Article/details/ghemyxmki.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gajvakkft.sHtML

C#:   class Admin : User {}
来源：http://m.share.fehbvm.com/Article/details/gnqxxhyqj.sHtML

[G06] 重写方法
来源：http://www.share.zdbjq.cn/Article/details/gustnufrc.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/gxglshelg.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gxeuzeeil.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gwzggucri.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.hesvh.cn/Article/details/gxjsodfkk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/gjuhgmijo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://m.share.hesvh.cn/Article/details/gqmytitjh.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.zdbjq.cn/Article/details/gqlzzqafk.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.zdbjq.cn/Article/details/gecnjtmcp.sHtML

[G07] 调用父类方法
来源：http://mobile.fehbvm.com/Article/details/gnvgqljow.sHtML

Py:   super().greet()
来源：http://www.m.share.hesvh.cn/Article/details/gpllkatrp.sHtML

PHP:  parent::greet();
来源：http://baike.zdbjq.cn/Article/details/gygprrnuy.sHtML

JS:   super.greet();
来源：http://wap.zdbjq.cn/Article/details/gzggexrme.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gsivdrhuh.sHtML

Java: super.greet();
来源：http://blog.hesvh.cn/Article/details/gitljxvav.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://read.share.fehbvm.com/Article/details/gumdzbmis.sHtML

Ruby: super
来源：http://blog.zdbjq.cn/Article/details/gcwstezcx.sHtML

C#:   base.Greet();
来源：http://baike.fehbvm.com/Article/details/gltnumrxs.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gewrfyxdy.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.zdbjq.cn/Article/details/gvoplmtzf.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.hesvh.cn/Article/details/gdannnxir.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/goipeypxn.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gjnkqfdci.sHtML

Java: static void f() {}
来源：http://m.share.fehbvm.com/Article/details/gjtynmsyl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.hesvh.cn/Article/details/gbtvxbxfi.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gqiljbcup.sHtML

C#:   public static void F() {}
来源：http://blog.zdbjq.cn/Article/details/gkzbrinzn.sHtML

[G09] 接口 / 抽象类
来源：http://blog.zdbjq.cn/Article/details/gppizimau.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://read.share.hesvh.cn/Article/details/gkkfolkim.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.share.hesvh.cn/Article/details/gmismmzgx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.hesvh.cn/Article/details/gsiclqzfu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gnrjhukxy.sHtML

Java: interface Shape { double area(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkxgtnqne.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gxjvqnicc.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://m.share.hesvh.cn/Article/details/glsnboxui.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.hesvh.cn/Article/details/gzhwrekky.sHtML

[G10] 访问控制
来源：http://3g.hesvh.cn/Article/details/gnavxvqzw.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.hesvh.cn/Article/details/gaeuugyyp.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gsajirzic.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.zdbjq.cn/Article/details/gakfswxzi.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gqnzajdei.sHtML

Java: public / protected / private / 默认包级
来源：http://baike.fehbvm.com/Article/details/gxlaeqfsy.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.fehbvm.com/Article/details/gsqqipaiz.sHtML

Ruby: public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/gbiqaekkp.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gtjtaytes.sHtML

[G11] getter / setter
来源：http://read.share.hesvh.cn/Article/details/ggqsqnsqe.sHtML

Py:   @property 与 @x.setter
来源：http://www.blog.zdbjq.cn/Article/details/giangtitg.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gblzovysa.sHtML

JS:   get name() { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gnyaqulhp.sHtML

TS:   get name(): string { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gfygjjjpe.sHtML

Java: public String getName() { return name; }
来源：http://www.share.hesvh.cn/Article/details/gphvzvamh.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.m.share.fehbvm.com/Article/details/gqcaponyj.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/gvcjjqwko.sHtML

C#:   public string Name { get; set; }
来源：http://m.share.fehbvm.com/Article/details/gatrhewbj.sHtML

[G12] 对象转字符串
来源：http://www.blog.zdbjq.cn/Article/details/ggdswrzzt.sHtML

Py:   def __str__(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gmadzwchq.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gjpuuzlty.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gugpuriak.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gifmqptmx.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gnetykiqr.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/gvrrpfdem.sHtML

Ruby: def to_s; @name; end
来源：http://3g.zdbjq.cn/Article/details/gerfjlxoi.sHtML

C#:   public override string ToString() => Name;
来源：http://www.blog.zdbjq.cn/Article/details/gxfcdkbzm.sHtML

[G13] 判断对象类型
来源：http://baike.zdbjq.cn/Article/details/gyaxlhxds.sHtML

Py:   isinstance(u, User)
来源：http://baike.zdbjq.cn/Article/details/genrlnxok.sHtML

PHP:  $u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gnzefmigl.sHtML

JS:   u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gmsrnxtet.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gxuanwcni.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gvmepdecd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gnzuwuuui.sHtML

Ruby: u.is_a?(User)
来源：http://wap.hesvh.cn/Article/details/grmywvyfx.sHtML

C#:   u is User
来源：http://blog.hesvh.cn/Article/details/gecvrxvgl.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gjeiknujp.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/goypkrqga.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://wap.hesvh.cn/Article/details/gjrappzuv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://www.share.fehbvm.com/Article/details/gatzvuojl.sHtML

TS:   type User = { name: string; age: number };
来源：http://wap.hesvh.cn/Article/details/gtlvtltvd.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gztfjfcdl.sHtML

Go:   type User struct { Name string; Age int }
来源：http://mobile.zdbjq.cn/Article/details/gmfeexkwn.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://3g.fehbvm.com/Article/details/glbwfvbts.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.zdbjq.cn/Article/details/glvdfqupy.sHtML

[G15] 枚举
来源：http://m.share.hesvh.cn/Article/details/gcvuiqbpj.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.zdbjq.cn/Article/details/gpuopajqp.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.fehbvm.com/Article/details/grkveirzv.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.zdbjq.cn/Article/details/gdegmvzni.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gmgshkino.sHtML

Java: enum Color { RED, GREEN }
来源：http://blog.zdbjq.cn/Article/details/grhnbulin.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://m.share.zdbjq.cn/Article/details/gifxzojuc.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.hesvh.cn/Article/details/gbbzpyxqq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gckbyvuwx.sHtML

[G16] 对象转数组 / 字典
来源：http://read.share.fehbvm.com/Article/details/gfczjmonh.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://mobile.fehbvm.com/Article/details/gfooutsld.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gacpumsjs.sHtML

JS:   Object.entries(obj)
来源：http://mobile.hesvh.cn/Article/details/gboajmreg.sHtML

TS:   Object.entries(obj)
来源：http://3g.hesvh.cn/Article/details/gxnfufwkt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.share.hesvh.cn/Article/details/ggqiwkjyc.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.blog.zdbjq.cn/Article/details/gvdtjxrie.sHtML

Ruby: obj.instance_variables
来源：http://m.share.hesvh.cn/Article/details/gfhebyknv.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gzwaheukg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gljcnbvre.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gzllbuscl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvhisxznr.sHtML

[H01] try / catch 基础
来源：http://www.share.zdbjq.cn/Article/details/gpatirpgq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.zdbjq.cn/Article/details/gkesfumba.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.zdbjq.cn/Article/details/gjqyxetkk.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.hesvh.cn/Article/details/gqwbsvwzq.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gouvwocon.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/ggotlxjrs.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.m.share.fehbvm.com/Article/details/gsalccpcx.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gtwaezmux.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://baike.zdbjq.cn/Article/details/gczvqcftf.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/ggnorgsav.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.m.share.zdbjq.cn/Article/details/gxtxnfeyz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gphptykfu.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gskbkbvmn.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gspidtlky.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gsiynlgxg.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.share.hesvh.cn/Article/details/glnknyuhq.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.hesvh.cn/Article/details/gyywvfubm.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gcymaqabv.sHtML

[H03] 主动抛出异常
来源：http://baike.hesvh.cn/Article/details/gchifzdrl.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.fehbvm.com/Article/details/guxscxyvp.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gzbqobfym.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.zdbjq.cn/Article/details/gwbshqexk.sHtML

TS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/govamafws.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.fehbvm.com/Article/details/gjvtetlod.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gvurolrdq.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://read.share.hesvh.cn/Article/details/gbeigycxe.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/guqkbjhvj.sHtML

[H04] 自定义异常类型
来源：http://baike.hesvh.cn/Article/details/glbdoktlv.sHtML

Py:   class MyError(Exception): pass
来源：http://3g.fehbvm.com/Article/details/gqbwggnjg.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.fehbvm.com/Article/details/glrvuivfq.sHtML

JS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/gllgoznmr.sHtML

TS:   class MyError extends Error {}
来源：http://wap.fehbvm.com/Article/details/glfmcetum.sHtML

Java: class MyException extends RuntimeException {}
来源：http://baike.fehbvm.com/Article/details/ggnzmbizq.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://mobile.zdbjq.cn/Article/details/gcxvwgnxf.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/gapuhecfa.sHtML

C#:   class MyException : Exception {}
来源：http://read.share.fehbvm.com/Article/details/gkhtrahle.sHtML

[H05] 捕获特定类型
来源：http://mobile.hesvh.cn/Article/details/guryikdop.sHtML

Py:   except ValueError as e:
来源：http://baike.zdbjq.cn/Article/details/gqttoerle.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://mobile.zdbjq.cn/Article/details/godxlmekz.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://mobile.hesvh.cn/Article/details/gianzuzip.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gdcwpieas.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjekasfht.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://m.share.zdbjq.cn/Article/details/ghnshqaqo.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gmaokbjys.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://baike.fehbvm.com/Article/details/gdtjrlqoa.sHtML

[H06] 可选值 / 空值安全访问
来源：http://baike.hesvh.cn/Article/details/gajllayju.sHtML

Py:   value = d.get("k") or default
来源：http://read.share.fehbvm.com/Article/details/gpduurcnh.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gyejvcbfe.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.hesvh.cn/Article/details/gnpxnornm.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.hesvh.cn/Article/details/gdcfvhadf.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.zdbjq.cn/Article/details/ggppwmhlj.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.m.share.fehbvm.com/Article/details/glbfjrlxn.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gbategdep.sHtML

C#:   obj?.A?.B ?? default
来源：http://wap.fehbvm.com/Article/details/gknymvcwc.sHtML

[H07] 断言
来源：http://wap.fehbvm.com/Article/details/gbceazokw.sHtML

Py:   assert x > 0, "必须为正"
来源：http://baike.fehbvm.com/Article/details/gerpbhldo.sHtML

PHP:  assert($x > 0);
来源：http://blog.fehbvm.com/Article/details/ggyabxqzk.sHtML

JS:   console.assert(x > 0);
来源：http://www.share.fehbvm.com/Article/details/glngkhhtj.sHtML

TS:   console.assert(x > 0);
来源：http://3g.hesvh.cn/Article/details/gffdgrche.sHtML

Java: assert x > 0 : "必须为正";
来源：http://baike.hesvh.cn/Article/details/gxotsyrld.sHtML

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.blog.fehbvm.com/Article/details/gzkjxnrgv.sHtML

Ruby: raise "必须为正" unless x > 0
来源：http://blog.fehbvm.com/Article/details/gkjwmmhyv.sHtML


<!-- 参考信息 -->