代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.hesvh.cn/Article/details/gkhhzjmrk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gxeqcljcc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.zdbjq.cn/Article/details/gnnlkkmmn.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.fehbvm.com/Article/details/gctfbgllw.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gkdylzcue.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/grlybqwrv.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/guxikcbbt.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gvoofveqs.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.zdbjq.cn/Article/details/geobxjuzs.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gvkktadng.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/gbjqrbdvw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.fehbvm.com/Article/details/gmygyvhbd.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.zdbjq.cn/Article/details/gzmvsdjrj.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.hesvh.cn/Article/details/grzuesfvr.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.hesvh.cn/Article/details/gyskgzylk.sHtML

[F04] 追加写入文件
来源：http://wap.fehbvm.com/Article/details/gnnkiprde.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gifmpgyjg.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gwjtjhabh.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gcwhntini.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gylgwiiao.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/grbaftptq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.hesvh.cn/Article/details/gasagemql.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gufyavogj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.zdbjq.cn/Article/details/ggcqneulu.sHtML

[F05] 判断文件或目录是否存在
来源：http://baike.hesvh.cn/Article/details/ggnajcpvs.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gctyaakeu.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.fehbvm.com/Article/details/gjyqjynmx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gzodeodaj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gxmkppdfh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gedofunin.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gehkcwflq.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gbbayauyh.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gydqwdydq.sHtML

[F06] 删除文件
来源：http://read.share.hesvh.cn/Article/details/gbnatkjqg.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gdfhflxds.sHtML

PHP:  unlink("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gctpxoelu.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gqqbswzqi.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gieabnlyd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gbbjvabsy.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/giskhiznk.sHtML

Ruby: File.delete("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gcqznnlcl.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gerjpffht.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gamrduiuw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://read.share.hesvh.cn/Article/details/gdhjwawrl.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gelohawdz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gjkdzwbul.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fehbvm.com/Article/details/gytjafuqq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://blog.hesvh.cn/Article/details/gjxjfqvch.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.hesvh.cn/Article/details/gxvmuredi.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/giamipwst.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.fehbvm.com/Article/details/gkxgjjbmb.sHtML

[F08] 遍历目录
来源：http://m.share.fehbvm.com/Article/details/gruebbjja.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://mobile.fehbvm.com/Article/details/gohuztwrl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.zdbjq.cn/Article/details/gjajugfwz.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gxyqllkkz.sHtML

TS:   fs.readdirSync("dir")
来源：http://wap.hesvh.cn/Article/details/gerhjjgvz.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.fehbvm.com/Article/details/gcgdqbhba.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.share.zdbjq.cn/Article/details/gncttfnbz.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gchjbqmnp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.zdbjq.cn/Article/details/gdoviiypm.sHtML

[F09] 获取文件大小
来源：http://mobile.hesvh.cn/Article/details/gvgotpegu.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gfwiuribs.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/glxrukotm.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fehbvm.com/Article/details/gkynfiitp.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gvzhkvpdu.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ghrcvbpkv.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://blog.zdbjq.cn/Article/details/gywexwebp.sHtML

Ruby: File.size("a.txt")
来源：http://m.share.hesvh.cn/Article/details/grvicosfp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.zdbjq.cn/Article/details/gspbdpxmc.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.zdbjq.cn/Article/details/grknanpph.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gzuqreyeb.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/grcnjaoqt.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.hesvh.cn/Article/details/gsdscxalq.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gekmfndyd.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.fehbvm.com/Article/details/gxrjfqwsw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gxbvlcdpj.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gqcftjqzs.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/girtkmnxw.sHtML

[F11] 复制与移动文件
来源：http://mobile.hesvh.cn/Article/details/gtmnwcvxx.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdqpkttyh.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://3g.fehbvm.com/Article/details/gmxrveeus.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmgfsoads.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/ghzdgqwna.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gmtnfssgq.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://read.share.zdbjq.cn/Article/details/gkqvitpqt.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/grkhtsflw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://blog.hesvh.cn/Article/details/gtwjnadab.sHtML

[F12] CSV 读写
来源：http://m.share.zdbjq.cn/Article/details/grezavzcr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gxwthpiql.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/ggyrdjgii.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/gjixauxdx.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gegulwkjp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.m.share.zdbjq.cn/Article/details/gwnbyeroz.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://mobile.fehbvm.com/Article/details/gzooptutq.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.zdbjq.cn/Article/details/gfqndfcol.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.zdbjq.cn/Article/details/gexmvpfqo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxvbbwjtl.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/grlgskzyq.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gefxuejpb.sHtML

[G01] 定义类
来源：http://www.share.zdbjq.cn/Article/details/gysnajgir.sHtML

Py:   class User: pass
来源：http://blog.fehbvm.com/Article/details/gmfwjhfei.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gulthyqiy.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gxslkodmx.sHtML

TS:   class User { name: string = ""; }
来源：http://www.blog.fehbvm.com/Article/details/gqgrviuxp.sHtML

Java: class User {}
来源：http://wap.hesvh.cn/Article/details/gbfdywapj.sHtML

Go:   type User struct { Name string }
来源：http://3g.fehbvm.com/Article/details/gjnpxumso.sHtML

Ruby: class User; end
来源：http://mobile.fehbvm.com/Article/details/gvovxeatp.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/gjutvwayz.sHtML

[G02] 构造函数
来源：http://mobile.zdbjq.cn/Article/details/gdsfinmpy.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/glkmjyklx.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/grifbicnn.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gxqfsuvzy.sHtML

TS:   constructor(public name: string) {}
来源：http://www.share.zdbjq.cn/Article/details/gdjnjcvsr.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gchxxigtu.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.zdbjq.cn/Article/details/gbjxggwbw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://mobile.hesvh.cn/Article/details/gpirxcjci.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.zdbjq.cn/Article/details/ghsgqbgqs.sHtML

[G03] 实例属性
来源：http://www.blog.fehbvm.com/Article/details/gwfmyunyk.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gayezkomr.sHtML

PHP:  public string $name = "x";
来源：http://www.share.zdbjq.cn/Article/details/gkxitezza.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/gsdmslqta.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gzgmtyfrm.sHtML

Java: private String name;
来源：http://wap.hesvh.cn/Article/details/giqftjtpx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gzkfuebzy.sHtML

Ruby: @name = "x"
来源：http://wap.zdbjq.cn/Article/details/gwxifuggn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gkreqbkqo.sHtML

[G04] 定义方法
来源：http://www.share.fehbvm.com/Article/details/gncbrhnpw.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.fehbvm.com/Article/details/gzkxcilrv.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gaslazdla.sHtML

JS:   greet() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/gscnmsptf.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gebptzxac.sHtML

Java: String greet() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gxdssygbv.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://blog.zdbjq.cn/Article/details/gqiwzeoag.sHtML

Ruby: def greet; @name; end
来源：http://www.blog.zdbjq.cn/Article/details/gjluzvkya.sHtML

C#:   public string Greet() => Name;
来源：http://blog.zdbjq.cn/Article/details/gfmhkrvsn.sHtML

[G05] 继承
来源：http://wap.zdbjq.cn/Article/details/gfeoktgmp.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/gmvjeuoad.sHtML

PHP:  class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gxrqccplk.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/gnehgaygk.sHtML

TS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/gehpjguvk.sHtML

Java: class Admin extends User {}
来源：http://read.share.zdbjq.cn/Article/details/ghnagudqu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gsyktjqcl.sHtML

Ruby: class Admin < User; end
来源：http://3g.hesvh.cn/Article/details/gygtizies.sHtML

C#:   class Admin : User {}
来源：http://www.share.hesvh.cn/Article/details/grkdimkov.sHtML

[G06] 重写方法
来源：http://www.blog.fehbvm.com/Article/details/gkgxtndnw.sHtML

Py:   def greet(self): return "admin"
来源：http://baike.zdbjq.cn/Article/details/gphqntjue.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/grnxgrwjt.sHtML

JS:   greet() { return "admin"; }
来源：http://www.m.share.fehbvm.com/Article/details/gzafxlakx.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gxhpupres.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/gpdjdtcrv.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://wap.hesvh.cn/Article/details/grfhorqry.sHtML

Ruby: def greet; "admin"; end
来源：http://3g.fehbvm.com/Article/details/gsgwsgmyi.sHtML

C#:   public override string Greet() => "admin";
来源：http://baike.hesvh.cn/Article/details/gqquezqeg.sHtML

[G07] 调用父类方法
来源：http://www.m.share.zdbjq.cn/Article/details/gdyzusuhl.sHtML

Py:   super().greet()
来源：http://read.share.zdbjq.cn/Article/details/gmkvdvfsp.sHtML

PHP:  parent::greet();
来源：http://www.share.fehbvm.com/Article/details/glilnfkjw.sHtML

JS:   super.greet();
来源：http://www.share.hesvh.cn/Article/details/gbdsrjahg.sHtML

TS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gwqlzdlhf.sHtML

Java: super.greet();
来源：http://baike.zdbjq.cn/Article/details/gblqayskv.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gudwnqvov.sHtML

Ruby: super
来源：http://mobile.fehbvm.com/Article/details/gztnrflgd.sHtML

C#:   base.Greet();
来源：http://read.share.fehbvm.com/Article/details/gxjdahddl.sHtML

[G08] 静态方法与属性
来源：http://www.share.hesvh.cn/Article/details/gukdxbxsf.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://baike.fehbvm.com/Article/details/giqxxpzih.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gdcvdqsij.sHtML

JS:   static f() {}
来源：http://www.share.zdbjq.cn/Article/details/gcyosexxh.sHtML

TS:   static f(): void {}
来源：http://3g.fehbvm.com/Article/details/gnsmlmxbq.sHtML

Java: static void f() {}
来源：http://wap.fehbvm.com/Article/details/gmabdsykv.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://read.share.fehbvm.com/Article/details/gjrgtnynx.sHtML

Ruby: def self.f; end
来源：http://m.share.fehbvm.com/Article/details/gljniweoq.sHtML

C#:   public static void F() {}
来源：http://baike.hesvh.cn/Article/details/gcnqpyywa.sHtML

[G09] 接口 / 抽象类
来源：http://read.share.hesvh.cn/Article/details/gnkcwdpbd.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gitlmbsdm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzzxjyule.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.share.zdbjq.cn/Article/details/gavsfeuqn.sHtML

TS:   interface Shape { area(): number; }
来源：http://mobile.fehbvm.com/Article/details/gjmltfhhx.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/gpmsaleah.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://blog.zdbjq.cn/Article/details/gmfhnfqhx.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://blog.hesvh.cn/Article/details/ghqntpmnx.sHtML

C#:   interface IShape { double Area(); }
来源：http://www.blog.hesvh.cn/Article/details/gjkgmtwcs.sHtML

[G10] 访问控制
来源：http://wap.zdbjq.cn/Article/details/gleuxkzht.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://wap.hesvh.cn/Article/details/ggognaphq.sHtML

PHP:  public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gnmdhbgip.sHtML

JS:   #private 字段；其余公开
来源：http://www.blog.fehbvm.com/Article/details/gjqbghbjp.sHtML

TS:   public / protected / private
来源：http://3g.fehbvm.com/Article/details/guipzfwmp.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.zdbjq.cn/Article/details/gapivkebv.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.fehbvm.com/Article/details/gepiewsla.sHtML

Ruby: public / protected / private
来源：http://baike.zdbjq.cn/Article/details/gdnwmhooh.sHtML

C#:   public / protected / private / internal
来源：http://wap.fehbvm.com/Article/details/gfgqsseem.sHtML

[G11] getter / setter
来源：http://read.share.zdbjq.cn/Article/details/gezouxxpq.sHtML

Py:   @property 与 @x.setter
来源：http://baike.zdbjq.cn/Article/details/gccvkalup.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/gdlbtewjp.sHtML

JS:   get name() { return this._name; }
来源：http://blog.zdbjq.cn/Article/details/gpfjzzkme.sHtML

TS:   get name(): string { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gmlbvupus.sHtML

Java: public String getName() { return name; }
来源：http://m.share.hesvh.cn/Article/details/gjgmutlua.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/gbjauufij.sHtML

Ruby: attr_accessor :name
来源：http://3g.fehbvm.com/Article/details/geavhzjrq.sHtML

C#:   public string Name { get; set; }
来源：http://wap.fehbvm.com/Article/details/gvbzpihdg.sHtML

[G12] 对象转字符串
来源：http://www.share.hesvh.cn/Article/details/gmkriahnm.sHtML

Py:   def __str__(self): return self.name
来源：http://www.m.share.zdbjq.cn/Article/details/gtphmvnoj.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.fehbvm.com/Article/details/gcfewxvdl.sHtML

JS:   toString() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/ghhhbdlmd.sHtML

TS:   toString(): string { return this.name; }
来源：http://read.share.hesvh.cn/Article/details/gyyxlbeye.sHtML

Java: @Override public String toString() { return name; }
来源：http://read.share.zdbjq.cn/Article/details/gpkqtvreu.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gowpuvnsx.sHtML

Ruby: def to_s; @name; end
来源：http://baike.hesvh.cn/Article/details/gtyzqatub.sHtML

C#:   public override string ToString() => Name;
来源：http://wap.zdbjq.cn/Article/details/ghxcbjmgi.sHtML

[G13] 判断对象类型
来源：http://wap.zdbjq.cn/Article/details/gqaeqxzkg.sHtML

Py:   isinstance(u, User)
来源：http://www.share.fehbvm.com/Article/details/gjzwphbnf.sHtML

PHP:  $u instanceof User
来源：http://m.share.hesvh.cn/Article/details/gmxpdjaxt.sHtML

JS:   u instanceof User
来源：http://blog.hesvh.cn/Article/details/gvtoqmdik.sHtML

TS:   u instanceof User
来源：http://www.blog.fehbvm.com/Article/details/gbyasazln.sHtML

Java: u instanceof User
来源：http://mobile.fehbvm.com/Article/details/golpsyouf.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://baike.fehbvm.com/Article/details/gpciytdcn.sHtML

Ruby: u.is_a?(User)
来源：http://www.share.fehbvm.com/Article/details/gzgbfynbb.sHtML

C#:   u is User
来源：http://3g.hesvh.cn/Article/details/gcncyhquo.sHtML

[G14] 数据类 / record
来源：http://3g.zdbjq.cn/Article/details/gzbujxtew.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gbvsvpgem.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.zdbjq.cn/Article/details/gbaoubglw.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://baike.zdbjq.cn/Article/details/gvlsndzwc.sHtML

TS:   type User = { name: string; age: number };
来源：http://blog.hesvh.cn/Article/details/gcangtagj.sHtML

Java: record User(String name, int age) {}
来源：http://baike.fehbvm.com/Article/details/gzzdpbuzn.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.hesvh.cn/Article/details/gnilzdcee.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.m.share.zdbjq.cn/Article/details/gxepflibo.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.hesvh.cn/Article/details/gjpaecnmx.sHtML

[G15] 枚举
来源：http://wap.hesvh.cn/Article/details/gqcmzikeq.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://baike.zdbjq.cn/Article/details/gadsolbia.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://read.share.zdbjq.cn/Article/details/gyguzelum.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://3g.hesvh.cn/Article/details/gcbdaoaxs.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://3g.hesvh.cn/Article/details/gvkaxsqvh.sHtML

Java: enum Color { RED, GREEN }
来源：http://mobile.zdbjq.cn/Article/details/gxpjtuauk.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.share.fehbvm.com/Article/details/gdwosmxtp.sHtML

Ruby: Color = %i[red green].freeze
来源：http://mobile.fehbvm.com/Article/details/gdddehpik.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://blog.zdbjq.cn/Article/details/gcnmfpeez.sHtML

[G16] 对象转数组 / 字典
来源：http://m.share.zdbjq.cn/Article/details/gbomaheuz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://3g.fehbvm.com/Article/details/gwwlemezg.sHtML

PHP:  get_object_vars($obj);
来源：http://www.blog.hesvh.cn/Article/details/gymjuwqhg.sHtML

JS:   Object.entries(obj)
来源：http://read.share.zdbjq.cn/Article/details/gfrxapmwc.sHtML

TS:   Object.entries(obj)
来源：http://mobile.zdbjq.cn/Article/details/grsyomjtj.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://blog.hesvh.cn/Article/details/gescjxqwy.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://baike.zdbjq.cn/Article/details/gdxblnklo.sHtML

Ruby: obj.instance_variables
来源：http://www.share.zdbjq.cn/Article/details/gborozoip.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/gwdatazbj.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmrdqkquu.sHtML

H. 异常与错误处理
来源：http://baike.zdbjq.cn/Article/details/gbddqgbrf.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gajbwcgti.sHtML

[H01] try / catch 基础
来源：http://wap.hesvh.cn/Article/details/gmycyfbjq.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.m.share.fehbvm.com/Article/details/gthmbljqo.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://blog.hesvh.cn/Article/details/gdxteprme.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://read.share.zdbjq.cn/Article/details/gcuesnami.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gjuafcqvg.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.hesvh.cn/Article/details/gjxllykdm.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://wap.fehbvm.com/Article/details/gxwkvravk.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://read.share.hesvh.cn/Article/details/ghhptyusp.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://mobile.fehbvm.com/Article/details/gsvzetoqx.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gdegwhoez.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://wap.hesvh.cn/Article/details/ghqhxhnay.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gmmzvbpeg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://3g.fehbvm.com/Article/details/gjhonabvg.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://wap.zdbjq.cn/Article/details/ggikdoavo.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/giaisoqpm.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.hesvh.cn/Article/details/gdjgqmddk.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://mobile.fehbvm.com/Article/details/gmoaynvsc.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://baike.hesvh.cn/Article/details/gfqxjbkvq.sHtML

[H03] 主动抛出异常
来源：http://read.share.hesvh.cn/Article/details/grxgonspm.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gvkjiyrcf.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://wap.hesvh.cn/Article/details/gvlptqkej.sHtML

JS:   throw new Error("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gksqkoehr.sHtML

TS:   throw new Error("错误信息");
来源：http://mobile.zdbjq.cn/Article/details/gufqmghqs.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://m.share.hesvh.cn/Article/details/gdfvasaar.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://blog.fehbvm.com/Article/details/gzmxnauiv.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.fehbvm.com/Article/details/grsyenhfa.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/grqilnkjm.sHtML

[H04] 自定义异常类型
来源：http://baike.fehbvm.com/Article/details/gmgrmymfu.sHtML

Py:   class MyError(Exception): pass
来源：http://www.share.zdbjq.cn/Article/details/gfuvbzkuj.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://blog.hesvh.cn/Article/details/gncjaprpl.sHtML

JS:   class MyError extends Error {}
来源：http://mobile.fehbvm.com/Article/details/gfmqrrywk.sHtML

TS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gplzksngb.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gvttuizrr.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://blog.zdbjq.cn/Article/details/gxvgpqibh.sHtML

Ruby: class MyError < StandardError; end
来源：http://m.share.hesvh.cn/Article/details/grglcyfvj.sHtML

C#:   class MyException : Exception {}
来源：http://www.m.share.fehbvm.com/Article/details/gxalttvjd.sHtML

[H05] 捕获特定类型
来源：http://mobile.fehbvm.com/Article/details/gsmgzflsd.sHtML

Py:   except ValueError as e:
来源：http://m.share.fehbvm.com/Article/details/gwfbpoapb.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.hesvh.cn/Article/details/ggzkbpgoj.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdyudaytj.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://www.blog.zdbjq.cn/Article/details/gctdwhcss.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.m.share.fehbvm.com/Article/details/giwhabock.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.m.share.fehbvm.com/Article/details/gzbmldxsh.sHtML

Ruby: rescue ArgumentError => e
来源：http://baike.zdbjq.cn/Article/details/gdbftoahj.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.share.hesvh.cn/Article/details/gsgtylmpw.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.blog.zdbjq.cn/Article/details/grjheystc.sHtML

Py:   value = d.get("k") or default
来源：http://blog.fehbvm.com/Article/details/giohtcwaf.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gskigrqmw.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/gsswpfjba.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://mobile.zdbjq.cn/Article/details/gcgjvualh.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://blog.fehbvm.com/Article/details/gcmpmmuge.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.share.zdbjq.cn/Article/details/gitorzqgh.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.blog.fehbvm.com/Article/details/gedxehxzp.sHtML

C#:   obj?.A?.B ?? default
来源：http://www.blog.fehbvm.com/Article/details/ghathcoit.sHtML


<!-- 参考信息 -->