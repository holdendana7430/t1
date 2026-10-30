代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fehbvm.com/Article/details/gjbdbucex.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/grhjclhwn.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fehbvm.com/Article/details/ggydnvrwn.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/geyjmdavr.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gmmhscbbf.sHtML

[F02] 逐行读取文件
来源：http://3g.fehbvm.com/Article/details/gkwuqbkoi.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/glgeflrne.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://baike.fehbvm.com/Article/details/gmlhyyinq.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/gciilurwu.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.zdbjq.cn/Article/details/gplmveomh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gjufrfqge.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/guyhfnapd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gaubbcqun.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.zdbjq.cn/Article/details/gxevgkxnw.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.zdbjq.cn/Article/details/gjvmqvrpp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/gwwxavpdl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/grhduhili.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/gfxevbjpt.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gaxghgulo.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.zdbjq.cn/Article/details/gegyujrvc.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gcjkdripi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/ghnhurdvu.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.zdbjq.cn/Article/details/gbayzmjok.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gaoumlfxm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.zdbjq.cn/Article/details/gbezdkfyj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gfuobolwx.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/ghxtiaebm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gpsnyqxxn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fehbvm.com/Article/details/ghghmulyb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/geimbidyv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.blog.hesvh.cn/Article/details/gdyqxxonk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.fehbvm.com/Article/details/gucngezdq.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gyzqxwmne.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gfcwqijex.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gupgbxwyn.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwkkpiuae.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gbdtmtbcm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gvxabmfiq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.hesvh.cn/Article/details/gwshuqked.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdmjlxaek.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gmfgdtfqi.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gsrruorcz.sHtML

Py:   os.remove("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gqjsgnczy.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gpyabesyv.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gfkupzwqq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gdoejwmxl.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/grhxkyjtp.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdxxdcgbh.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gvppkuhyt.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.zdbjq.cn/Article/details/gaudnhvez.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/gyrzsrija.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxtfvpye.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/gprscmbkr.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.fehbvm.com/Article/details/gccmvxlqy.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gknndyexy.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.fehbvm.com/Article/details/gbtcyqbym.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.m.share.zdbjq.cn/Article/details/gnojebhtp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.hesvh.cn/Article/details/gsqcyckrs.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.hesvh.cn/Article/details/gapruqdqa.sHtML

[F08] 遍历目录
来源：http://m.share.hesvh.cn/Article/details/gxeddzyti.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gsqhdzugl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.hesvh.cn/Article/details/gbvrzfjms.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/glaysbnkr.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/giwtjvcab.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gbwznzsnw.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/gctfcviiq.sHtML

Ruby: Dir.children("dir")
来源：http://blog.fehbvm.com/Article/details/gysacxuiq.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gkazpbvam.sHtML

[F09] 获取文件大小
来源：http://baike.hesvh.cn/Article/details/gklvqofhi.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghfhurecj.sHtML

PHP:  filesize("a.txt");
来源：http://blog.zdbjq.cn/Article/details/geireudxy.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/glrittnee.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gvivhgxha.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gdjfwdpqq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.fehbvm.com/Article/details/gwezhcbjz.sHtML

Ruby: File.size("a.txt")
来源：http://wap.zdbjq.cn/Article/details/ggioazrjc.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/gxcvlprss.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://www.blog.hesvh.cn/Article/details/gjmtjfpit.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/giakrnbvw.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/gvvkecbov.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gcxqyvblp.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gsdwkwitl.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.zdbjq.cn/Article/details/gpzehcpae.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gkfwyyyrn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gldxjhtea.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gesvgoilu.sHtML

[F11] 复制与移动文件
来源：http://mobile.fehbvm.com/Article/details/gojmrtzqy.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gsneqnuxs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.zdbjq.cn/Article/details/gcjlgsztz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gqfictwqs.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/golzytdoi.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gmkybfxzb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gbitykiog.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gtcgpmjbx.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gdfqvocep.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/ghirnbzeu.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.fehbvm.com/Article/details/guszmzfir.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.fehbvm.com/Article/details/gcofbrisc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://read.share.fehbvm.com/Article/details/gqgvjlftd.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/ghigylyiw.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.hesvh.cn/Article/details/gtpmrjtpx.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.hesvh.cn/Article/details/gdvluszup.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fehbvm.com/Article/details/gzkaskgbl.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.fehbvm.com/Article/details/gpmmtcdym.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gusnwhimx.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/glrjtxvmx.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmsjecupc.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gmxlkxzdw.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/ggsjybest.sHtML

PHP:  class User {}
来源：http://www.m.share.hesvh.cn/Article/details/gyxdooqhl.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/geggraptb.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/gvzyudsxv.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gnuoncnoi.sHtML

Go:   type User struct { Name string }
来源：http://wap.zdbjq.cn/Article/details/gpdbysopo.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/galfwnupe.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gtxxufyod.sHtML

[G02] 构造函数
来源：http://baike.hesvh.cn/Article/details/ghxbnnfqs.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://blog.fehbvm.com/Article/details/gmookigxh.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://baike.fehbvm.com/Article/details/gvpbaacll.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gubjcoklf.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.fehbvm.com/Article/details/gcmfytsdc.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.zdbjq.cn/Article/details/gmljcwfdc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gkriwlocx.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.hesvh.cn/Article/details/gayvvfsuo.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.zdbjq.cn/Article/details/gdeaklatn.sHtML

[G03] 实例属性
来源：http://blog.hesvh.cn/Article/details/gqzmgfmqr.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gudqglzmq.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gjhxigygh.sHtML

JS:   this.name = "x";
来源：http://blog.hesvh.cn/Article/details/gecdafyzd.sHtML

TS:   name: string = "x";
来源：http://wap.fehbvm.com/Article/details/gxxlfnnks.sHtML

Java: private String name;
来源：http://baike.hesvh.cn/Article/details/gjkudwlna.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://m.share.fehbvm.com/Article/details/gewenhdri.sHtML

Ruby: @name = "x"
来源：http://read.share.hesvh.cn/Article/details/gzpsuttlf.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.hesvh.cn/Article/details/ghtlodsxk.sHtML

[G04] 定义方法
来源：http://www.share.zdbjq.cn/Article/details/gqyifbzpp.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/ghnvhadxw.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gyfqyqdol.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkoqscaxt.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/glyacvtqm.sHtML

Java: String greet() { return name; }
来源：http://baike.hesvh.cn/Article/details/gnccuzbbi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/ginlqgbgu.sHtML

Ruby: def greet; @name; end
来源：http://www.share.zdbjq.cn/Article/details/gojmyobeg.sHtML

C#:   public string Greet() => Name;
来源：http://www.blog.hesvh.cn/Article/details/guzteelol.sHtML

[G05] 继承
来源：http://wap.fehbvm.com/Article/details/gamxifzgc.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gvgpaoenn.sHtML

PHP:  class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gprsssiov.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwmefofnv.sHtML

TS:   class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gxmtdycuk.sHtML

Java: class Admin extends User {}
来源：http://m.share.zdbjq.cn/Article/details/gjzobjzzp.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.hesvh.cn/Article/details/gpkstxsaj.sHtML

Ruby: class Admin < User; end
来源：http://wap.zdbjq.cn/Article/details/gpgvfjeta.sHtML

C#:   class Admin : User {}
来源：http://blog.fehbvm.com/Article/details/grnpvytnb.sHtML

[G06] 重写方法
来源：http://baike.zdbjq.cn/Article/details/gnplbhxqy.sHtML

Py:   def greet(self): return "admin"
来源：http://wap.fehbvm.com/Article/details/gxtfhojvp.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gmiaiufmh.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gnqgrtsye.sHtML

TS:   greet(): string { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gcgobfayk.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://3g.fehbvm.com/Article/details/gurjkqvwo.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gczfjduim.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.fehbvm.com/Article/details/gyzaffyvj.sHtML

C#:   public override string Greet() => "admin";
来源：http://wap.zdbjq.cn/Article/details/gzapsobrr.sHtML

[G07] 调用父类方法
来源：http://read.share.zdbjq.cn/Article/details/gbqhycspw.sHtML

Py:   super().greet()
来源：http://m.share.hesvh.cn/Article/details/gqyyzsegr.sHtML

PHP:  parent::greet();
来源：http://m.share.zdbjq.cn/Article/details/gzgprjxwy.sHtML

JS:   super.greet();
来源：http://read.share.zdbjq.cn/Article/details/gzxzuptdy.sHtML

TS:   super.greet();
来源：http://baike.fehbvm.com/Article/details/gcwajqeem.sHtML

Java: super.greet();
来源：http://mobile.zdbjq.cn/Article/details/giubrotor.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://mobile.zdbjq.cn/Article/details/ghyzpnkmy.sHtML

Ruby: super
来源：http://3g.hesvh.cn/Article/details/gxchxwfaj.sHtML

C#:   base.Greet();
来源：http://m.share.fehbvm.com/Article/details/gddedzsxe.sHtML

[G08] 静态方法与属性
来源：http://read.share.zdbjq.cn/Article/details/gynpfbrxz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://mobile.hesvh.cn/Article/details/guxifxpbw.sHtML

PHP:  public static function f() {}
来源：http://wap.zdbjq.cn/Article/details/ggamugoaj.sHtML

JS:   static f() {}
来源：http://3g.zdbjq.cn/Article/details/gnebamhil.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gjbyswqfc.sHtML

Java: static void f() {}
来源：http://www.share.hesvh.cn/Article/details/gbhkepxvr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.m.share.fehbvm.com/Article/details/gftgkoxvr.sHtML

Ruby: def self.f; end
来源：http://www.share.fehbvm.com/Article/details/gfyjmvwdt.sHtML

C#:   public static void F() {}
来源：http://wap.fehbvm.com/Article/details/gdfgcwihh.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gzmlhmorx.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gsgkaamre.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.fehbvm.com/Article/details/giywfwndr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.blog.zdbjq.cn/Article/details/gddfjfgmu.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.blog.zdbjq.cn/Article/details/gdyfrggfo.sHtML

Java: interface Shape { double area(); }
来源：http://www.share.hesvh.cn/Article/details/gelnglrqs.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gzykisnfy.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://baike.fehbvm.com/Article/details/giorhfcor.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.fehbvm.com/Article/details/gndveicpa.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gaufnqgaa.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/gsipwybij.sHtML

PHP:  public / protected / private
来源：http://3g.fehbvm.com/Article/details/gudmiyjwf.sHtML

JS:   #private 字段；其余公开
来源：http://baike.zdbjq.cn/Article/details/glgqxmntc.sHtML

TS:   public / protected / private
来源：http://m.share.hesvh.cn/Article/details/gkivatmhl.sHtML

Java: public / protected / private / 默认包级
来源：http://m.share.hesvh.cn/Article/details/ghpkbfgnk.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://blog.fehbvm.com/Article/details/gdbwpggoq.sHtML

Ruby: public / protected / private
来源：http://read.share.fehbvm.com/Article/details/glevwbnvr.sHtML

C#:   public / protected / private / internal
来源：http://www.share.hesvh.cn/Article/details/glzqehmrb.sHtML

[G11] getter / setter
来源：http://blog.zdbjq.cn/Article/details/gpozqvqmp.sHtML

Py:   @property 与 @x.setter
来源：http://www.share.hesvh.cn/Article/details/guyzsmkor.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.share.zdbjq.cn/Article/details/gshwzblwk.sHtML

JS:   get name() { return this._name; }
来源：http://www.blog.fehbvm.com/Article/details/gjchmvlhp.sHtML

TS:   get name(): string { return this._name; }
来源：http://mobile.fehbvm.com/Article/details/gagirxuqw.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/grtfrwnll.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gbjtriuyj.sHtML

Ruby: attr_accessor :name
来源：http://m.share.hesvh.cn/Article/details/gemgwjlop.sHtML

C#:   public string Name { get; set; }
来源：http://wap.hesvh.cn/Article/details/gebjflisy.sHtML

[G12] 对象转字符串
来源：http://wap.zdbjq.cn/Article/details/gaewrflwu.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.zdbjq.cn/Article/details/gyifnohnt.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gjflmadnw.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.zdbjq.cn/Article/details/gwmxquhbn.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gvkzgcnaf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.hesvh.cn/Article/details/ggsccsfpw.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.m.share.zdbjq.cn/Article/details/gufdehumb.sHtML

Ruby: def to_s; @name; end
来源：http://wap.hesvh.cn/Article/details/gbizsgjtp.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.zdbjq.cn/Article/details/gywftrqji.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gvtgrkfeb.sHtML

Py:   isinstance(u, User)
来源：http://blog.zdbjq.cn/Article/details/gwaldmvyk.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gawucnyxs.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gphhcljwx.sHtML

TS:   u instanceof User
来源：http://www.share.hesvh.cn/Article/details/gryjrtxaa.sHtML

Java: u instanceof User
来源：http://baike.zdbjq.cn/Article/details/gltvghmwn.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.fehbvm.com/Article/details/gdrcvkbsw.sHtML

Ruby: u.is_a?(User)
来源：http://blog.zdbjq.cn/Article/details/gvicazwoz.sHtML

C#:   u is User
来源：http://www.blog.hesvh.cn/Article/details/gxvmwrgkw.sHtML

[G14] 数据类 / record
来源：http://3g.fehbvm.com/Article/details/gdesyftip.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://baike.hesvh.cn/Article/details/gsqmqcpci.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.hesvh.cn/Article/details/gnyorhgbx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://wap.fehbvm.com/Article/details/gyqbaknky.sHtML

TS:   type User = { name: string; age: number };
来源：http://www.blog.fehbvm.com/Article/details/gqmxicqvu.sHtML

Java: record User(String name, int age) {}
来源：http://read.share.fehbvm.com/Article/details/gghiapcul.sHtML

Go:   type User struct { Name string; Age int }
来源：http://wap.zdbjq.cn/Article/details/gvhiivfea.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gboezngme.sHtML

C#:   record User(string Name, int Age);
来源：http://mobile.fehbvm.com/Article/details/gaoqimnni.sHtML

[G15] 枚举
来源：http://baike.zdbjq.cn/Article/details/gbqagthjt.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.blog.zdbjq.cn/Article/details/gfamgdkcx.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.blog.fehbvm.com/Article/details/gzrsoarju.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/ggovbwxgu.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gwzrpfyjg.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gcqhsehkm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.zdbjq.cn/Article/details/gtkfkpyjf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.share.zdbjq.cn/Article/details/gofuqpfib.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/ggbryyvld.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.zdbjq.cn/Article/details/gjsqdiqfq.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://wap.zdbjq.cn/Article/details/ggkxklwdq.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.hesvh.cn/Article/details/ggzwjiwiu.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gutzmzftf.sHtML

TS:   Object.entries(obj)
来源：http://baike.fehbvm.com/Article/details/gpjbcztiv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.blog.zdbjq.cn/Article/details/gnwtetmqu.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.fehbvm.com/Article/details/ghqfcyjfn.sHtML

Ruby: obj.instance_variables
来源：http://read.share.zdbjq.cn/Article/details/gjktwadlo.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/gwsppnixr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gjbbkxjqk.sHtML

H. 异常与错误处理
来源：http://read.share.hesvh.cn/Article/details/gseqrvgnq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gnyhrbavf.sHtML

[H01] try / catch 基础
来源：http://wap.fehbvm.com/Article/details/gegqjzzyi.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.hesvh.cn/Article/details/gnpfcbouq.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.zdbjq.cn/Article/details/gqieyzsyt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gwyodwhog.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://read.share.fehbvm.com/Article/details/gphixcxjr.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.blog.zdbjq.cn/Article/details/glpndsljy.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.zdbjq.cn/Article/details/gzbbktzyc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.m.share.fehbvm.com/Article/details/gmekqooiq.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://m.share.hesvh.cn/Article/details/gcqsddcdz.sHtML

[H02] finally / ensure 收尾
来源：http://www.share.hesvh.cn/Article/details/geqsabvff.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://3g.hesvh.cn/Article/details/gdofdyqpw.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gwfclpiqq.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gnldjvchq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.fehbvm.com/Article/details/gxsewnzsf.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gjmpfrpmz.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.fehbvm.com/Article/details/gecrzjgxa.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.hesvh.cn/Article/details/gftnosnid.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/grraznnea.sHtML

[H03] 主动抛出异常
来源：http://www.blog.zdbjq.cn/Article/details/gphfvgbjz.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.fehbvm.com/Article/details/gvdmxvggh.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/ggohktizj.sHtML

JS:   throw new Error("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gepfqxuse.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gtftnzdci.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.m.share.fehbvm.com/Article/details/gsawkgnif.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://read.share.fehbvm.com/Article/details/gmzdqhlek.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.blog.zdbjq.cn/Article/details/gyzmftydj.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/gzmjakcdz.sHtML

[H04] 自定义异常类型
来源：http://m.share.zdbjq.cn/Article/details/gflnigugn.sHtML

Py:   class MyError(Exception): pass
来源：http://mobile.hesvh.cn/Article/details/gcchjjngq.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbrwblses.sHtML

JS:   class MyError extends Error {}
来源：http://www.share.zdbjq.cn/Article/details/gobobbfks.sHtML

TS:   class MyError extends Error {}
来源：http://blog.fehbvm.com/Article/details/geniuercm.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gsqbmkjbi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.hesvh.cn/Article/details/galezuwzy.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.zdbjq.cn/Article/details/gbyjhqonh.sHtML

C#:   class MyException : Exception {}
来源：http://m.share.hesvh.cn/Article/details/gnrinyply.sHtML

[H05] 捕获特定类型
来源：http://wap.fehbvm.com/Article/details/gaabsuymc.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gcyntwvyp.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.hesvh.cn/Article/details/gcqngpvfw.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/ganrgdogy.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://3g.hesvh.cn/Article/details/gwfmocuvj.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://3g.zdbjq.cn/Article/details/gfhmyzjuo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://blog.hesvh.cn/Article/details/gtllwdrml.sHtML

Ruby: rescue ArgumentError => e
来源：http://3g.hesvh.cn/Article/details/gelryebog.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.blog.fehbvm.com/Article/details/grgyrketp.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gplrcchrt.sHtML


<!-- 参考信息 -->