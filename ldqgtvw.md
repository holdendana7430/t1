代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fehbvm.com/Article/details/gphuadarp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gqsygstyi.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gubuwjhyv.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.zdbjq.cn/Article/details/gaqmjepjz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.share.hesvh.cn/Article/details/givcpmqri.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gmxngeqpd.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.hesvh.cn/Article/details/gwneldjqz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.fehbvm.com/Article/details/gilubozoh.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gghxfhapi.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/grpryrwrj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/ggstartik.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/gycrmfook.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.hesvh.cn/Article/details/gwezpdgjj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.zdbjq.cn/Article/details/gybchslev.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/giohqsmtn.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gmlbkvkxl.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gnrelteec.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.hesvh.cn/Article/details/gvxxgrnai.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gnwmftoug.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gixcfqfnz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/gfajuuzms.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gqmrtkqpv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.fehbvm.com/Article/details/gyaxyoniw.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fehbvm.com/Article/details/geckpgeab.sHtML

[F05] 判断文件或目录是否存在
来源：http://m.share.fehbvm.com/Article/details/gzyinkotm.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/geyfbecgp.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.fehbvm.com/Article/details/gjkoddqmq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gmilalqzt.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gwmdttcox.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gmenhnuky.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.zdbjq.cn/Article/details/gwluylorf.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsqiuwwbz.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gjdhvxyvf.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/grustcmwl.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/ggnwdmdck.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gogygmpzj.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gkzmcvqgy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyznxqrgh.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/geypqnblp.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.hesvh.cn/Article/details/gujsegnpb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gnjqiqxna.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gdiybsghr.sHtML

[F07] 创建目录（含多级）
来源：http://blog.fehbvm.com/Article/details/gqslzasdo.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gxnnyjfey.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.zdbjq.cn/Article/details/gbedmgdjb.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gngidzeru.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/ggkqequei.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.share.fehbvm.com/Article/details/gzcmajhbt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gsslqtljg.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/gnrgeesrh.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://read.share.zdbjq.cn/Article/details/geefllcra.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/guwlqzblm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://wap.hesvh.cn/Article/details/gkndutach.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fehbvm.com/Article/details/gqqtwniyr.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gmvowojpp.sHtML

TS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gvxuzwuln.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gwugwhfzu.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://baike.zdbjq.cn/Article/details/grhkpxwrq.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/grplodfzt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.fehbvm.com/Article/details/glqvdtwmp.sHtML

[F09] 获取文件大小
来源：http://wap.zdbjq.cn/Article/details/gadvvegcj.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gbsydwhjv.sHtML

PHP:  filesize("a.txt");
来源：http://wap.hesvh.cn/Article/details/gopxlkqrw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://mobile.zdbjq.cn/Article/details/gnggokacs.sHtML

TS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gowfgiatk.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/geemayczl.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.hesvh.cn/Article/details/gtqvqflmh.sHtML

Ruby: File.size("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gfhqmrafz.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.fehbvm.com/Article/details/gasxpovht.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://baike.hesvh.cn/Article/details/gtxaqnrne.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gytxzyjsg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gjuymmozb.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gooyzozkw.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwschimkw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gtyusynvf.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glhdsahjj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/geumsvufo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gakwdgsqw.sHtML

[F11] 复制与移动文件
来源：http://read.share.fehbvm.com/Article/details/gyqesphsa.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzfhegrku.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.hesvh.cn/Article/details/gififeptz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gtrvrlrgj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gnykvvxzj.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.fehbvm.com/Article/details/gjlifzptb.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/gtvizdkcz.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.hesvh.cn/Article/details/gcntliryn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/glozavfys.sHtML

[F12] CSV 读写
来源：http://read.share.fehbvm.com/Article/details/gchobehcv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://read.share.hesvh.cn/Article/details/gaavamsdk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gtgnqnloi.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fehbvm.com/Article/details/guhkevwym.sHtML

TS:   // 同上
来源：http://3g.zdbjq.cn/Article/details/ghoblzubc.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fehbvm.com/Article/details/grkxicenr.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.share.zdbjq.cn/Article/details/gwcfvppxi.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.zdbjq.cn/Article/details/genngkvbe.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gbmvpmfmn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxvdnzxnq.sHtML

G. 面向对象
来源：http://www.m.share.zdbjq.cn/Article/details/gvgfejujg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdwuxgvnh.sHtML

[G01] 定义类
来源：http://wap.fehbvm.com/Article/details/gleerhztt.sHtML

Py:   class User: pass
来源：http://3g.zdbjq.cn/Article/details/gtbkikrvy.sHtML

PHP:  class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gshblprmc.sHtML

JS:   class User {}
来源：http://blog.fehbvm.com/Article/details/gttoymofj.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/genedjfjx.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gasjnpztw.sHtML

Go:   type User struct { Name string }
来源：http://mobile.hesvh.cn/Article/details/gxhmrfcyf.sHtML

Ruby: class User; end
来源：http://blog.fehbvm.com/Article/details/glggiinxi.sHtML

C#:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gcfeazdua.sHtML

[G02] 构造函数
来源：http://3g.zdbjq.cn/Article/details/gsuokqbpy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://3g.zdbjq.cn/Article/details/gcahqyftp.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.blog.zdbjq.cn/Article/details/gmpuebvga.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://baike.fehbvm.com/Article/details/gylkwopup.sHtML

TS:   constructor(public name: string) {}
来源：http://blog.hesvh.cn/Article/details/gemxuuqvi.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gdizhpczc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.zdbjq.cn/Article/details/gsbfektlp.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.zdbjq.cn/Article/details/gvwlzekgw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://mobile.fehbvm.com/Article/details/ggdmkhghs.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gdvygcscr.sHtML

Py:   self.name = "x"
来源：http://www.blog.hesvh.cn/Article/details/gequmatsj.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gwiffixbx.sHtML

JS:   this.name = "x";
来源：http://m.share.zdbjq.cn/Article/details/gszlnlecn.sHtML

TS:   name: string = "x";
来源：http://3g.zdbjq.cn/Article/details/glmwxaofg.sHtML

Java: private String name;
来源：http://baike.fehbvm.com/Article/details/gotnextbs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.hesvh.cn/Article/details/gexiwfork.sHtML

Ruby: @name = "x"
来源：http://www.share.zdbjq.cn/Article/details/grfqutvwm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gminzlktm.sHtML

[G04] 定义方法
来源：http://baike.zdbjq.cn/Article/details/gmjghqvau.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gmvhxjiok.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.fehbvm.com/Article/details/gtonnniep.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/grkgxyxjk.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fehbvm.com/Article/details/gyvjklzps.sHtML

Java: String greet() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gwllqjtlo.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.hesvh.cn/Article/details/gsmyhsxer.sHtML

Ruby: def greet; @name; end
来源：http://blog.zdbjq.cn/Article/details/grxzwqiwr.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.hesvh.cn/Article/details/goxjrooat.sHtML

[G05] 继承
来源：http://mobile.fehbvm.com/Article/details/gvicdtgeh.sHtML

Py:   class Admin(User): pass
来源：http://read.share.hesvh.cn/Article/details/gtphnoxpo.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gpujhfopq.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gaoqtmwkn.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gawsvybdu.sHtML

Java: class Admin extends User {}
来源：http://baike.fehbvm.com/Article/details/gifadspfq.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://mobile.fehbvm.com/Article/details/gnvkeiknu.sHtML

Ruby: class Admin < User; end
来源：http://www.blog.zdbjq.cn/Article/details/gfkfycjia.sHtML

C#:   class Admin : User {}
来源：http://m.share.zdbjq.cn/Article/details/glkhfsqsg.sHtML

[G06] 重写方法
来源：http://baike.fehbvm.com/Article/details/gmmkbjjzg.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.hesvh.cn/Article/details/giddhuibi.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggsyiavtd.sHtML

JS:   greet() { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gngjqbaco.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.blog.hesvh.cn/Article/details/gdvqvhztw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://m.share.zdbjq.cn/Article/details/gaezwmnvd.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.hesvh.cn/Article/details/gfbdivxfc.sHtML

Ruby: def greet; "admin"; end
来源：http://blog.fehbvm.com/Article/details/gbyoteiul.sHtML

C#:   public override string Greet() => "admin";
来源：http://www.blog.fehbvm.com/Article/details/gmrhfanco.sHtML

[G07] 调用父类方法
来源：http://baike.hesvh.cn/Article/details/gbnoejnug.sHtML

Py:   super().greet()
来源：http://www.share.zdbjq.cn/Article/details/godpygpst.sHtML

PHP:  parent::greet();
来源：http://mobile.zdbjq.cn/Article/details/gxxtkaxbt.sHtML

JS:   super.greet();
来源：http://3g.fehbvm.com/Article/details/ghdfxkxzv.sHtML

TS:   super.greet();
来源：http://baike.zdbjq.cn/Article/details/gdppmrhgt.sHtML

Java: super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gyuhhyldh.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.m.share.hesvh.cn/Article/details/gfgvbwudz.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gseopcuyv.sHtML

C#:   base.Greet();
来源：http://baike.zdbjq.cn/Article/details/gjcxwdopt.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gnlpsqzda.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.hesvh.cn/Article/details/gpecxbkii.sHtML

PHP:  public static function f() {}
来源：http://www.blog.fehbvm.com/Article/details/goundfqfp.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/ggpobalmt.sHtML

TS:   static f(): void {}
来源：http://m.share.hesvh.cn/Article/details/gzzpvxyas.sHtML

Java: static void f() {}
来源：http://m.share.zdbjq.cn/Article/details/gdrbeavmr.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.hesvh.cn/Article/details/gdgweqzsi.sHtML

Ruby: def self.f; end
来源：http://www.share.zdbjq.cn/Article/details/gcpzfnhzu.sHtML

C#:   public static void F() {}
来源：http://wap.zdbjq.cn/Article/details/gsuzfmsux.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gbxdurcaf.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/ghtplrrsk.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/ggjapyqbx.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gmzvdkppy.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gsiovaoql.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.fehbvm.com/Article/details/gymhebxbj.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.fehbvm.com/Article/details/gvsdlllvw.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gqcdsinhf.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.share.zdbjq.cn/Article/details/gmppvptsq.sHtML

[G10] 访问控制
来源：http://baike.zdbjq.cn/Article/details/gmwoxoggl.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.fehbvm.com/Article/details/gpjwntvnz.sHtML

PHP:  public / protected / private
来源：http://www.blog.zdbjq.cn/Article/details/gixsdfqnq.sHtML

JS:   #private 字段；其余公开
来源：http://mobile.fehbvm.com/Article/details/gxlazcgxb.sHtML

TS:   public / protected / private
来源：http://blog.fehbvm.com/Article/details/girbdhdkg.sHtML

Java: public / protected / private / 默认包级
来源：http://wap.hesvh.cn/Article/details/gktegsbul.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.share.zdbjq.cn/Article/details/gopulgdhk.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/gfgzntdaw.sHtML

C#:   public / protected / private / internal
来源：http://3g.hesvh.cn/Article/details/goziywrdi.sHtML

[G11] getter / setter
来源：http://baike.hesvh.cn/Article/details/gfozhhlcb.sHtML

Py:   @property 与 @x.setter
来源：http://m.share.hesvh.cn/Article/details/graurbody.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://mobile.zdbjq.cn/Article/details/gdgmdfhyl.sHtML

JS:   get name() { return this._name; }
来源：http://mobile.hesvh.cn/Article/details/gejdaiupd.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.zdbjq.cn/Article/details/ghasgehey.sHtML

Java: public String getName() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gismomswo.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/guyvvxfhi.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/grvlldhuc.sHtML

C#:   public string Name { get; set; }
来源：http://blog.zdbjq.cn/Article/details/gcmyjacdw.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gzwnupbiw.sHtML

Py:   def __str__(self): return self.name
来源：http://read.share.hesvh.cn/Article/details/gipxvfmov.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gcroedfdq.sHtML

JS:   toString() { return this.name; }
来源：http://read.share.fehbvm.com/Article/details/gcipnqgei.sHtML

TS:   toString(): string { return this.name; }
来源：http://blog.zdbjq.cn/Article/details/grzkbxznt.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.fehbvm.com/Article/details/gcjtlmsnm.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://blog.hesvh.cn/Article/details/ghqiuuzkd.sHtML

Ruby: def to_s; @name; end
来源：http://wap.zdbjq.cn/Article/details/gkmfwrfkk.sHtML

C#:   public override string ToString() => Name;
来源：http://blog.hesvh.cn/Article/details/gcwesykzl.sHtML

[G13] 判断对象类型
来源：http://3g.fehbvm.com/Article/details/gsrgjitft.sHtML

Py:   isinstance(u, User)
来源：http://read.share.hesvh.cn/Article/details/gogtucfmz.sHtML

PHP:  $u instanceof User
来源：http://mobile.hesvh.cn/Article/details/gjvtyqyya.sHtML

JS:   u instanceof User
来源：http://baike.zdbjq.cn/Article/details/ggguqcnvp.sHtML

TS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gnkmnqfwv.sHtML

Java: u instanceof User
来源：http://www.share.hesvh.cn/Article/details/ghzccizyy.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://read.share.zdbjq.cn/Article/details/gvrkhlwpa.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.zdbjq.cn/Article/details/geyzmqihf.sHtML

C#:   u is User
来源：http://wap.zdbjq.cn/Article/details/gcykeobvg.sHtML

[G14] 数据类 / record
来源：http://m.share.hesvh.cn/Article/details/ghgzswyfa.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.share.zdbjq.cn/Article/details/gkrpgqarn.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.hesvh.cn/Article/details/giswtjzvg.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://3g.fehbvm.com/Article/details/gutufoimw.sHtML

TS:   type User = { name: string; age: number };
来源：http://mobile.fehbvm.com/Article/details/gyspafkhi.sHtML

Java: record User(String name, int age) {}
来源：http://3g.hesvh.cn/Article/details/gqgotymyi.sHtML

Go:   type User struct { Name string; Age int }
来源：http://blog.hesvh.cn/Article/details/gpnjdhiim.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/gczlzwwso.sHtML

C#:   record User(string Name, int Age);
来源：http://m.share.hesvh.cn/Article/details/gydxrjxac.sHtML

[G15] 枚举
来源：http://www.blog.zdbjq.cn/Article/details/gngtxxgpy.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.hesvh.cn/Article/details/gvfkaajhv.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://wap.zdbjq.cn/Article/details/gapiicejo.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://wap.hesvh.cn/Article/details/gzebqsvbw.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.blog.zdbjq.cn/Article/details/ghitojacy.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gknqtuppm.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://baike.zdbjq.cn/Article/details/ggcemgpcf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://3g.zdbjq.cn/Article/details/gkfofnimn.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://wap.zdbjq.cn/Article/details/gjsixtnjk.sHtML

[G16] 对象转数组 / 字典
来源：http://www.share.fehbvm.com/Article/details/gbiiwbvwv.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://m.share.zdbjq.cn/Article/details/gaeejzajo.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gictmbbsl.sHtML

JS:   Object.entries(obj)
来源：http://blog.fehbvm.com/Article/details/gghevksjh.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/gpadqfjxe.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.fehbvm.com/Article/details/gbulnmyls.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.fehbvm.com/Article/details/gkunqdnzh.sHtML

Ruby: obj.instance_variables
来源：http://baike.zdbjq.cn/Article/details/gyzddrqsb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gdfmfrmuq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grhdqdonc.sHtML

H. 异常与错误处理
来源：http://m.share.zdbjq.cn/Article/details/gdiibulug.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gaiqzumrl.sHtML

[H01] try / catch 基础
来源：http://baike.fehbvm.com/Article/details/ggirtfecb.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://blog.fehbvm.com/Article/details/gndofsucl.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://3g.zdbjq.cn/Article/details/ggzcsfyvc.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://m.share.zdbjq.cn/Article/details/gaougbmml.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://baike.fehbvm.com/Article/details/gsycxvpfy.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gxifsasrk.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.zdbjq.cn/Article/details/gujlcykky.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gysdrpiik.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://wap.zdbjq.cn/Article/details/geopohnbk.sHtML

[H02] finally / ensure 收尾
来源：http://www.blog.hesvh.cn/Article/details/gjwxaxqjq.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gxdrpselv.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/ggenzihal.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/grdzyxgwi.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.m.share.hesvh.cn/Article/details/gsltbekft.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gzslkzukl.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://m.share.zdbjq.cn/Article/details/gwposlkdi.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.zdbjq.cn/Article/details/grufgxejf.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gidsedppp.sHtML

[H03] 主动抛出异常
来源：http://www.blog.hesvh.cn/Article/details/gjwruqrji.sHtML

Py:   raise ValueError("错误信息")
来源：http://blog.zdbjq.cn/Article/details/gmqgbfbnb.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/ghsixicpi.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gmgejmnti.sHtML

TS:   throw new Error("错误信息");
来源：http://wap.zdbjq.cn/Article/details/grurfurjq.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/ggqfrdqib.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.hesvh.cn/Article/details/gltxkiugj.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.hesvh.cn/Article/details/gctzaigcr.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gwcknptge.sHtML

[H04] 自定义异常类型
来源：http://www.blog.zdbjq.cn/Article/details/gnmvsmyrq.sHtML

Py:   class MyError(Exception): pass
来源：http://www.blog.hesvh.cn/Article/details/glqdtsngt.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gacxvpizh.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.zdbjq.cn/Article/details/gedmdvakl.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gxlbihqlk.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.hesvh.cn/Article/details/gufqtiwkk.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.zdbjq.cn/Article/details/gijdlzkke.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.blog.hesvh.cn/Article/details/gubjlaxzw.sHtML

C#:   class MyException : Exception {}
来源：http://blog.fehbvm.com/Article/details/grsxsfbgq.sHtML

[H05] 捕获特定类型
来源：http://www.blog.hesvh.cn/Article/details/gcvnvnrer.sHtML

Py:   except ValueError as e:
来源：http://mobile.zdbjq.cn/Article/details/gfapzjlbf.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://m.share.fehbvm.com/Article/details/gqqgcspfm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gkafdfuqj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.share.zdbjq.cn/Article/details/gsabpzmtc.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://baike.fehbvm.com/Article/details/ghsmlqhkx.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.fehbvm.com/Article/details/gkgqvfdjv.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.hesvh.cn/Article/details/geynzupbc.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/gdgtzfehk.sHtML

[H06] 可选值 / 空值安全访问
来源：http://wap.hesvh.cn/Article/details/gfmswxajl.sHtML

Py:   value = d.get("k") or default
来源：http://www.m.share.zdbjq.cn/Article/details/gfcamfejm.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/gyarmkuec.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://baike.fehbvm.com/Article/details/gzxttsdls.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://wap.zdbjq.cn/Article/details/glriisbbt.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.share.hesvh.cn/Article/details/gjeaaihrq.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gkclesmje.sHtML

Ruby: d&.dig(:a, :b)
来源：http://blog.hesvh.cn/Article/details/gyaqbrynu.sHtML

C#:   obj?.A?.B ?? default
来源：http://3g.fehbvm.com/Article/details/gznvwckhz.sHtML


<!-- 参考信息 -->