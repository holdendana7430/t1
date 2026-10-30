代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gxvtgrrnv.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gqklulyag.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.hesvh.cn/Article/details/gqsvzndci.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.zdbjq.cn/Article/details/gixlkrncr.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/glfmeakud.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/ggotdgkpb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gtdvarltm.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.zdbjq.cn/Article/details/gcwiwqzie.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.zdbjq.cn/Article/details/gqdvywsyh.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gmwrwkznw.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gyxxavphx.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gvrlwvfbk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gycdxxwpx.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gmlrrfwtx.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gagtszinp.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gfjiyiqij.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.hesvh.cn/Article/details/grvnnkjkn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gaiaaojer.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/gahanilvd.sHtML

[F04] 追加写入文件
来源：http://3g.zdbjq.cn/Article/details/gxsdgfysl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://3g.fehbvm.com/Article/details/gxuwriont.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gdjgtzuot.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gkczvkkfq.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gymzkogkd.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gortqgaoe.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/gfzhmsksp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gbhnhsefm.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.fehbvm.com/Article/details/gryckdgct.sHtML

[F05] 判断文件或目录是否存在
来源：http://wap.fehbvm.com/Article/details/gqktxliqs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gfeymhpmw.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gqewgaxyp.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gcauidfdt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtcvomprl.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/ghkiefekl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/guuoadikm.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gcsdvoaca.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gjwohzrqm.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gtxkqwkdj.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkagxenvf.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gvlxxzuky.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghqgwoscg.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmpvtmzed.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/grtfjdwjw.sHtML

Go:   os.Remove("a.txt")
来源：http://baike.fehbvm.com/Article/details/ghlwukcal.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.fehbvm.com/Article/details/gkjywlrgb.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gnlyfmulg.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gcqhfgogc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gecrtegux.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.hesvh.cn/Article/details/gwctrwgsn.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.hesvh.cn/Article/details/gnntjuype.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/gqwrvayoc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gpslucllr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://wap.hesvh.cn/Article/details/gcucghmoz.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.hesvh.cn/Article/details/glgrqhtxv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/glgoncxqj.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/gjtcbmrwg.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gfqcfsfwb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://wap.fehbvm.com/Article/details/girbdoida.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gmtkfauzq.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gvyfuqkbw.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/ggckszjoy.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/gynjfvcvv.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.fehbvm.com/Article/details/gojrghvqi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.blog.fehbvm.com/Article/details/gbwbgljox.sHtML

[F09] 获取文件大小
来源：http://mobile.fehbvm.com/Article/details/gaiesmdpw.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.hesvh.cn/Article/details/gxtfbjapi.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gnscyltss.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/ghjogynvj.sHtML

TS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/grkriqzrl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gxhdfwkjz.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gvmddcsfk.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gzjvpecez.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.m.share.fehbvm.com/Article/details/gmmhgpver.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/gukcgagoq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/gcdtiirdc.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.fehbvm.com/Article/details/gczacsnyr.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxrjqkxmq.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/ggztffewv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.zdbjq.cn/Article/details/gaiivgznb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gezsnnksd.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmqizygct.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gykkyjdux.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.hesvh.cn/Article/details/gwsjgnluf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/getcohnrh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.share.fehbvm.com/Article/details/gebvwndln.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gkfrixzth.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/gvjunqrcf.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.zdbjq.cn/Article/details/gmnfigcyv.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://3g.fehbvm.com/Article/details/gotpyjvly.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gujwczzhh.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.hesvh.cn/Article/details/gnzjjehmp.sHtML

[F12] CSV 读写
来源：http://www.m.share.zdbjq.cn/Article/details/gsiuraxeq.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.blog.hesvh.cn/Article/details/gnprzsutg.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.share.hesvh.cn/Article/details/gzlmxwigg.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fehbvm.com/Article/details/gnezwwehh.sHtML

TS:   // 同上
来源：http://baike.hesvh.cn/Article/details/gjayxlwvn.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://mobile.zdbjq.cn/Article/details/gdthopgnu.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.blog.zdbjq.cn/Article/details/gfafwflna.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fehbvm.com/Article/details/gikzaxmvn.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://mobile.fehbvm.com/Article/details/goljbktst.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggcvkdndx.sHtML

G. 面向对象
来源：http://m.share.hesvh.cn/Article/details/gjtputajh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/grwvtghfv.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gsalnhfwm.sHtML

Py:   class User: pass
来源：http://www.blog.hesvh.cn/Article/details/gkgoemphj.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/glrqkndfn.sHtML

JS:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gjjludlnx.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gjtjhbdad.sHtML

Java: class User {}
来源：http://3g.hesvh.cn/Article/details/gowxlbkpc.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/gceuclxci.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/gxzfpryox.sHtML

C#:   class User {}
来源：http://m.share.zdbjq.cn/Article/details/gxqwnwyzp.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gofpagfjt.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.fehbvm.com/Article/details/gqmibmsep.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gmjsqfkpi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gmlgcmpbv.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gsisrcwpm.sHtML

Java: User(String name) { this.name = name; }
来源：http://wap.fehbvm.com/Article/details/gcmpdlwlg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.share.hesvh.cn/Article/details/geawhwmko.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.fehbvm.com/Article/details/gfwefmjnf.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gzxposkdp.sHtML

[G03] 实例属性
来源：http://wap.zdbjq.cn/Article/details/gwbmynlaj.sHtML

Py:   self.name = "x"
来源：http://www.share.hesvh.cn/Article/details/grduhrhys.sHtML

PHP:  public string $name = "x";
来源：http://www.share.fehbvm.com/Article/details/gtvargtjq.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/glzfwqyvh.sHtML

TS:   name: string = "x";
来源：http://www.blog.fehbvm.com/Article/details/gwwgsvaal.sHtML

Java: private String name;
来源：http://m.share.zdbjq.cn/Article/details/gdlduvlqe.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.zdbjq.cn/Article/details/glzlqxxpq.sHtML

Ruby: @name = "x"
来源：http://www.share.hesvh.cn/Article/details/garamnaim.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gmybardss.sHtML

[G04] 定义方法
来源：http://3g.hesvh.cn/Article/details/gsikikhez.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/ghxehobuc.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gsdnlfsdp.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdflbaxxo.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.zdbjq.cn/Article/details/guxitduin.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/giyafkptx.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://baike.zdbjq.cn/Article/details/gikrzwewa.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/grdifffsb.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/guipmtxaq.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gzutqmisa.sHtML

Py:   class Admin(User): pass
来源：http://3g.fehbvm.com/Article/details/gsxlumghb.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/ghcrswcho.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.fehbvm.com/Article/details/gkxppivso.sHtML

TS:   class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gnsytehrd.sHtML

Java: class Admin extends User {}
来源：http://mobile.zdbjq.cn/Article/details/gnnzoxlhy.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gcbnbvgdx.sHtML

Ruby: class Admin < User; end
来源：http://baike.zdbjq.cn/Article/details/gykygxldd.sHtML

C#:   class Admin : User {}
来源：http://m.share.hesvh.cn/Article/details/gtkmwcddl.sHtML

[G06] 重写方法
来源：http://read.share.zdbjq.cn/Article/details/gkdekfwtw.sHtML

Py:   def greet(self): return "admin"
来源：http://www.blog.fehbvm.com/Article/details/gydfgaihw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://3g.hesvh.cn/Article/details/ghgvlmgep.sHtML

JS:   greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gdyicbuik.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/glgmgasca.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gqqpkhjzg.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.fehbvm.com/Article/details/gnsyjfoey.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.hesvh.cn/Article/details/gbkxgspfm.sHtML

C#:   public override string Greet() => "admin";
来源：http://m.share.fehbvm.com/Article/details/gcedbmmuq.sHtML

[G07] 调用父类方法
来源：http://www.m.share.hesvh.cn/Article/details/gnulqbvkl.sHtML

Py:   super().greet()
来源：http://www.share.fehbvm.com/Article/details/gotovefak.sHtML

PHP:  parent::greet();
来源：http://read.share.zdbjq.cn/Article/details/gqjrwoqcu.sHtML

JS:   super.greet();
来源：http://mobile.hesvh.cn/Article/details/gurgomsfd.sHtML

TS:   super.greet();
来源：http://blog.hesvh.cn/Article/details/gdsnqennv.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gtwmvkxsp.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.fehbvm.com/Article/details/ggkpgsrwv.sHtML

Ruby: super
来源：http://wap.hesvh.cn/Article/details/gsmkthvsm.sHtML

C#:   base.Greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gnepfparf.sHtML

[G08] 静态方法与属性
来源：http://blog.hesvh.cn/Article/details/gqevtkjvh.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.blog.zdbjq.cn/Article/details/gzfsfsedv.sHtML

PHP:  public static function f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/geqrwrfms.sHtML

JS:   static f() {}
来源：http://read.share.zdbjq.cn/Article/details/gehqtsojs.sHtML

TS:   static f(): void {}
来源：http://read.share.hesvh.cn/Article/details/gtdtutbju.sHtML

Java: static void f() {}
来源：http://blog.fehbvm.com/Article/details/gfxqpatfl.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://wap.zdbjq.cn/Article/details/gvckygada.sHtML

Ruby: def self.f; end
来源：http://www.share.hesvh.cn/Article/details/grxvpgykn.sHtML

C#:   public static void F() {}
来源：http://www.blog.hesvh.cn/Article/details/gyoggvaff.sHtML

[G09] 接口 / 抽象类
来源：http://blog.hesvh.cn/Article/details/gcmwvyoni.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.share.zdbjq.cn/Article/details/gbnasapba.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gbczawnjr.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://mobile.zdbjq.cn/Article/details/gzwvowsne.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqwkppxjl.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gsrxennhc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://www.blog.hesvh.cn/Article/details/gpugcwurr.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.m.share.hesvh.cn/Article/details/gsifmspqw.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gbybiwvbf.sHtML

[G10] 访问控制
来源：http://blog.zdbjq.cn/Article/details/gwetxjgny.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://www.share.zdbjq.cn/Article/details/gsrnnofxx.sHtML

PHP:  public / protected / private
来源：http://www.m.share.zdbjq.cn/Article/details/goamcxdhk.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gatqtvhhj.sHtML

TS:   public / protected / private
来源：http://www.blog.hesvh.cn/Article/details/ggdyfjymw.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gtzntyreg.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.fehbvm.com/Article/details/gvvtkxnce.sHtML

Ruby: public / protected / private
来源：http://read.share.hesvh.cn/Article/details/gpbvvgqmh.sHtML

C#:   public / protected / private / internal
来源：http://baike.zdbjq.cn/Article/details/gosptpmkw.sHtML

[G11] getter / setter
来源：http://www.m.share.hesvh.cn/Article/details/ghcjgbcme.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/gvaakrbhw.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://3g.zdbjq.cn/Article/details/gnwddbpgd.sHtML

JS:   get name() { return this._name; }
来源：http://www.share.zdbjq.cn/Article/details/gxwiiinsc.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.hesvh.cn/Article/details/gynfjyopi.sHtML

Java: public String getName() { return name; }
来源：http://blog.zdbjq.cn/Article/details/gtiaureii.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gddbkcabf.sHtML

Ruby: attr_accessor :name
来源：http://www.m.share.zdbjq.cn/Article/details/gsrxmeqcb.sHtML

C#:   public string Name { get; set; }
来源：http://www.share.hesvh.cn/Article/details/gyzspnyum.sHtML

[G12] 对象转字符串
来源：http://blog.hesvh.cn/Article/details/gqztnldpu.sHtML

Py:   def __str__(self): return self.name
来源：http://wap.fehbvm.com/Article/details/gfincbplc.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.zdbjq.cn/Article/details/gcacoxdpp.sHtML

JS:   toString() { return this.name; }
来源：http://wap.hesvh.cn/Article/details/guyqgbifs.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwsqpanjb.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gwrgxnonm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gptbznvna.sHtML

Ruby: def to_s; @name; end
来源：http://wap.fehbvm.com/Article/details/gywbipybu.sHtML

C#:   public override string ToString() => Name;
来源：http://mobile.hesvh.cn/Article/details/garhrjotq.sHtML

[G13] 判断对象类型
来源：http://blog.zdbjq.cn/Article/details/ghxxvdiwh.sHtML

Py:   isinstance(u, User)
来源：http://mobile.hesvh.cn/Article/details/gkzestmef.sHtML

PHP:  $u instanceof User
来源：http://read.share.zdbjq.cn/Article/details/gtntrbvsg.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gjnmlokqa.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gwvggvdcn.sHtML

Java: u instanceof User
来源：http://www.m.share.hesvh.cn/Article/details/gxjjkanwq.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://wap.zdbjq.cn/Article/details/gbrvjbzaj.sHtML

Ruby: u.is_a?(User)
来源：http://3g.zdbjq.cn/Article/details/gujadrnmt.sHtML

C#:   u is User
来源：http://3g.zdbjq.cn/Article/details/gyygopkbt.sHtML

[G14] 数据类 / record
来源：http://www.share.hesvh.cn/Article/details/gxnpeigro.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://blog.zdbjq.cn/Article/details/gljkzcrkz.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://baike.zdbjq.cn/Article/details/gbkvgvvfx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.fehbvm.com/Article/details/gblnrtssa.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.fehbvm.com/Article/details/gjovvidul.sHtML

Java: record User(String name, int age) {}
来源：http://3g.zdbjq.cn/Article/details/gydsicnyg.sHtML

Go:   type User struct { Name string; Age int }
来源：http://baike.fehbvm.com/Article/details/gtjwdulgq.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://baike.fehbvm.com/Article/details/gfzdwpzkr.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gwrhlbpje.sHtML

[G15] 枚举
来源：http://www.share.zdbjq.cn/Article/details/gavhlpyrl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.m.share.hesvh.cn/Article/details/gnvmpbqzv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.hesvh.cn/Article/details/gontrsrrh.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://baike.fehbvm.com/Article/details/gqwjyczko.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gxnsuofgq.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gosasvacw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.zdbjq.cn/Article/details/gikttbuip.sHtML

Ruby: Color = %i[red green].freeze
来源：http://m.share.hesvh.cn/Article/details/gdntxwahq.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.hesvh.cn/Article/details/gddmgjssn.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.zdbjq.cn/Article/details/gmiolhfgm.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gnoagmgum.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/guqvybvwi.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gwfwtfpdz.sHtML

TS:   Object.entries(obj)
来源：http://mobile.fehbvm.com/Article/details/gvuiuiouy.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://read.share.fehbvm.com/Article/details/goaznzohs.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://m.share.zdbjq.cn/Article/details/ggdnvvcbj.sHtML

Ruby: obj.instance_variables
来源：http://www.m.share.hesvh.cn/Article/details/gfwceprhh.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gnowibcin.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggjlrpbwu.sHtML

H. 异常与错误处理
来源：http://blog.zdbjq.cn/Article/details/gftkznrpe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gszyhylea.sHtML

[H01] try / catch 基础
来源：http://read.share.zdbjq.cn/Article/details/gwupnwejo.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.fehbvm.com/Article/details/gwaczuzof.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.fehbvm.com/Article/details/gavqmnmmt.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.fehbvm.com/Article/details/gvdsgsefy.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.hesvh.cn/Article/details/gdtydebyo.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gkreksqbx.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.share.fehbvm.com/Article/details/gsfhywqou.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gkjkjblaz.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.share.zdbjq.cn/Article/details/gxjfvanew.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/geiolxhph.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.zdbjq.cn/Article/details/gnolqachx.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/gmckrjzgk.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://blog.fehbvm.com/Article/details/gkxqcvzfq.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gjliteyqg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gzckpdftv.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://wap.fehbvm.com/Article/details/gbmgvjgga.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.hesvh.cn/Article/details/grelcejmp.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.hesvh.cn/Article/details/gxuquitpw.sHtML

[H03] 主动抛出异常
来源：http://3g.fehbvm.com/Article/details/gmdxgmqot.sHtML

Py:   raise ValueError("错误信息")
来源：http://www.share.hesvh.cn/Article/details/gffnkqrxl.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/ghyrgpzff.sHtML

JS:   throw new Error("错误信息");
来源：http://www.share.fehbvm.com/Article/details/grtrmgzwj.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.hesvh.cn/Article/details/gzwkybiha.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://3g.hesvh.cn/Article/details/gylzrpham.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://wap.zdbjq.cn/Article/details/gxcoawina.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gibneygqr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://baike.fehbvm.com/Article/details/gntcjrhvs.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gkcvmwumn.sHtML

Py:   class MyError(Exception): pass
来源：http://baike.fehbvm.com/Article/details/gluvajlru.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://read.share.zdbjq.cn/Article/details/gxdorzjzf.sHtML

JS:   class MyError extends Error {}
来源：http://www.blog.hesvh.cn/Article/details/gtmmtwyhe.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.fehbvm.com/Article/details/gfbtgivoh.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.share.hesvh.cn/Article/details/gpyawnqdi.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.share.zdbjq.cn/Article/details/gxmenqktz.sHtML

Ruby: class MyError < StandardError; end
来源：http://mobile.fehbvm.com/Article/details/glrbuawpg.sHtML

C#:   class MyException : Exception {}
来源：http://www.blog.zdbjq.cn/Article/details/gkupfljor.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gufclhvxb.sHtML

Py:   except ValueError as e:
来源：http://read.share.hesvh.cn/Article/details/gmitrnawy.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.blog.zdbjq.cn/Article/details/gydzvqwlg.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.blog.hesvh.cn/Article/details/gbvmfdorn.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://wap.hesvh.cn/Article/details/gljcveopl.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghyyyqjbc.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gseckfubq.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/gwgdnzkjz.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.zdbjq.cn/Article/details/gbjaqpoiz.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.m.share.zdbjq.cn/Article/details/ghblgfqms.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.hesvh.cn/Article/details/gvcnunlfa.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gytvvpklf.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.hesvh.cn/Article/details/gazezexzk.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gcrrcvpeq.sHtML


<!-- 参考信息 -->