代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gzcfxkwvs.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://blog.fehbvm.com/Article/details/gwzbhrowe.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/ggfoferbo.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.zdbjq.cn/Article/details/grxxpwhbf.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gyoqvjzot.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.zdbjq.cn/Article/details/gznusrttj.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.fehbvm.com/Article/details/gxnrdjbzp.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.zdbjq.cn/Article/details/gromaouvc.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gjdmzdsoy.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.zdbjq.cn/Article/details/gwaxgquiq.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gzljibbaz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.zdbjq.cn/Article/details/gstlliozr.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gbvhmavxy.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.fehbvm.com/Article/details/gvofhjofi.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.zdbjq.cn/Article/details/gvjxxciic.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gevcpkmdd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/gisnwkqba.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/glbmhgiaw.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.fehbvm.com/Article/details/gppmcsnbg.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/gtyauohnh.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/galrkokal.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://3g.zdbjq.cn/Article/details/ghahjsvjq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://m.share.fehbvm.com/Article/details/ghwikhvoe.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://read.share.hesvh.cn/Article/details/gjqnfuonf.sHtML

[F05] 判断文件或目录是否存在
来源：http://read.share.fehbvm.com/Article/details/gbhuyfuzu.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.hesvh.cn/Article/details/gsydmqdnz.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gsczcnkvf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gqelahupi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gjreldlfm.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/gkholwneh.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.zdbjq.cn/Article/details/givyjygnf.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gpvuympum.sHtML

C#:   File.Exists("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gofwjbjgx.sHtML

[F06] 删除文件
来源：http://3g.hesvh.cn/Article/details/gkgleztis.sHtML

Py:   os.remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glzvspsvu.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gxwrzkkvb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxxqtarns.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gtgenhwmg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/ggyflgugy.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.hesvh.cn/Article/details/gbasovdjx.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gzepivxcg.sHtML

C#:   File.Delete("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/glemcsmbk.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gyxhsijtd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/gcgpyhgqq.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gdlmaubfh.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.hesvh.cn/Article/details/gygrystxr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gesndjreq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.zdbjq.cn/Article/details/gylfmmxhr.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/gwbkmhbzt.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.zdbjq.cn/Article/details/gcwwgyrud.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/givrxghvy.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gkuvuxiub.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.zdbjq.cn/Article/details/gakdbyyoh.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gqrvlrzhq.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/grydfyosm.sHtML

TS:   fs.readdirSync("dir")
来源：http://baike.fehbvm.com/Article/details/gxwlzgpfa.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.fehbvm.com/Article/details/gvyateioz.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gciryrpol.sHtML

Ruby: Dir.children("dir")
来源：http://m.share.zdbjq.cn/Article/details/guizmbnnf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gjabsorzc.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/gvowzdckt.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmmaczqmc.sHtML

PHP:  filesize("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gdnsbqjhb.sHtML

JS:   fs.statSync("a.txt").size
来源：http://blog.hesvh.cn/Article/details/goblnrhii.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gpqyklqna.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/ggytqzzsq.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.hesvh.cn/Article/details/gewstfrfy.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gwsipjbff.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://m.share.hesvh.cn/Article/details/givcmvznk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gqujewvup.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gzcfdhjup.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://m.share.fehbvm.com/Article/details/ghxwxwpff.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://baike.hesvh.cn/Article/details/gbaoeewhg.sHtML

TS:   path.extname("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwwvggdrv.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gcrflisex.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://baike.fehbvm.com/Article/details/gxsfeigby.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fehbvm.com/Article/details/goirpfybf.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gftloleaf.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gbrlqndfz.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/gmikaqriv.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://read.share.hesvh.cn/Article/details/gwcgmfycx.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gdttdyadj.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gufemggnk.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gatqbvjeh.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/gdsoucdcr.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://baike.fehbvm.com/Article/details/gdopzlsct.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.hesvh.cn/Article/details/gydfnjvfe.sHtML

[F12] CSV 读写
来源：http://www.share.fehbvm.com/Article/details/gpfyxrpdk.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.share.hesvh.cn/Article/details/gejwpabtf.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://mobile.fehbvm.com/Article/details/gbfmiajxc.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.blog.fehbvm.com/Article/details/gufwtjtlk.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gbmzxntpd.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://m.share.hesvh.cn/Article/details/gjnsomrfd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/glgxyrzvj.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.zdbjq.cn/Article/details/gpteyfqcv.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.zdbjq.cn/Article/details/glmvjnzcb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmbgwffdq.sHtML

G. 面向对象
来源：http://wap.fehbvm.com/Article/details/gvlvxcvxl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glgfhqozy.sHtML

[G01] 定义类
来源：http://www.blog.hesvh.cn/Article/details/gylkjmxal.sHtML

Py:   class User: pass
来源：http://read.share.fehbvm.com/Article/details/govjeuvbr.sHtML

PHP:  class User {}
来源：http://mobile.fehbvm.com/Article/details/gopgdppif.sHtML

JS:   class User {}
来源：http://read.share.zdbjq.cn/Article/details/ghpzucpil.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gcguxgjtn.sHtML

Java: class User {}
来源：http://www.blog.fehbvm.com/Article/details/gjuraduqf.sHtML

Go:   type User struct { Name string }
来源：http://read.share.hesvh.cn/Article/details/gwliakcbq.sHtML

Ruby: class User; end
来源：http://m.share.fehbvm.com/Article/details/gaxsmmpci.sHtML

C#:   class User {}
来源：http://mobile.fehbvm.com/Article/details/gxpyadihf.sHtML

[G02] 构造函数
来源：http://m.share.hesvh.cn/Article/details/gbznxsgac.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.fehbvm.com/Article/details/gljcmwjae.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.zdbjq.cn/Article/details/ggigvrpig.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.hesvh.cn/Article/details/gxbcarxix.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.zdbjq.cn/Article/details/gekowgbvy.sHtML

Java: User(String name) { this.name = name; }
来源：http://baike.hesvh.cn/Article/details/gsfinepmx.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://3g.fehbvm.com/Article/details/gqykcmetf.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://3g.hesvh.cn/Article/details/gfuogvuwe.sHtML

C#:   public User(string name) { Name = name; }
来源：http://read.share.zdbjq.cn/Article/details/ghuazhrst.sHtML

[G03] 实例属性
来源：http://read.share.fehbvm.com/Article/details/ggpuleuda.sHtML

Py:   self.name = "x"
来源：http://3g.hesvh.cn/Article/details/gzpourzeo.sHtML

PHP:  public string $name = "x";
来源：http://baike.fehbvm.com/Article/details/gdpnoujgq.sHtML

JS:   this.name = "x";
来源：http://wap.zdbjq.cn/Article/details/ggmixsufe.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gmkawzmxj.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gixpuorfj.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gucjsebfw.sHtML

Ruby: @name = "x"
来源：http://read.share.zdbjq.cn/Article/details/gptzcnljq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.fehbvm.com/Article/details/gndmhqpwd.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gbeuxvdsn.sHtML

Py:   def greet(self): return self.name
来源：http://www.share.zdbjq.cn/Article/details/gtvcdldon.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/gwngslanm.sHtML

JS:   greet() { return this.name; }
来源：http://3g.zdbjq.cn/Article/details/gwdgqptal.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/glnerggne.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/gxlapzscy.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gxkwyruxy.sHtML

Ruby: def greet; @name; end
来源：http://mobile.zdbjq.cn/Article/details/guvnyweat.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/glnwjqtej.sHtML

[G05] 继承
来源：http://blog.fehbvm.com/Article/details/gzgjuaygp.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fehbvm.com/Article/details/gvhkyziht.sHtML

PHP:  class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/gmhxnpwvu.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gqgsdlpnp.sHtML

TS:   class Admin extends User {}
来源：http://blog.fehbvm.com/Article/details/gzefaqboz.sHtML

Java: class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxakyfzzd.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://blog.hesvh.cn/Article/details/gejlkvujp.sHtML

Ruby: class Admin < User; end
来源：http://m.share.hesvh.cn/Article/details/gioohwlwk.sHtML

C#:   class Admin : User {}
来源：http://www.share.zdbjq.cn/Article/details/gprtoiand.sHtML

[G06] 重写方法
来源：http://blog.hesvh.cn/Article/details/gqiglnvfv.sHtML

Py:   def greet(self): return "admin"
来源：http://read.share.zdbjq.cn/Article/details/gcwvociff.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://www.m.share.hesvh.cn/Article/details/gujcvjnsb.sHtML

JS:   greet() { return "admin"; }
来源：http://blog.zdbjq.cn/Article/details/gokbqgavo.sHtML

TS:   greet(): string { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gmnvhdyev.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gkpdwrrqn.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://baike.hesvh.cn/Article/details/gocpdkkfu.sHtML

Ruby: def greet; "admin"; end
来源：http://baike.zdbjq.cn/Article/details/gvvkqcodg.sHtML

C#:   public override string Greet() => "admin";
来源：http://mobile.fehbvm.com/Article/details/gfrbeaysq.sHtML

[G07] 调用父类方法
来源：http://wap.fehbvm.com/Article/details/gbnimmnmq.sHtML

Py:   super().greet()
来源：http://www.m.share.zdbjq.cn/Article/details/gzzdadxfi.sHtML

PHP:  parent::greet();
来源：http://www.share.hesvh.cn/Article/details/ghbtixsoi.sHtML

JS:   super.greet();
来源：http://m.share.zdbjq.cn/Article/details/gvfzeewuc.sHtML

TS:   super.greet();
来源：http://www.blog.hesvh.cn/Article/details/gutcljcci.sHtML

Java: super.greet();
来源：http://www.share.zdbjq.cn/Article/details/gnnddlgfw.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gnthgnlur.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gokmcmmqf.sHtML

C#:   base.Greet();
来源：http://mobile.zdbjq.cn/Article/details/gsoxnnxkj.sHtML

[G08] 静态方法与属性
来源：http://www.m.share.zdbjq.cn/Article/details/gpmkcnetz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://wap.fehbvm.com/Article/details/gspobqrcy.sHtML

PHP:  public static function f() {}
来源：http://mobile.fehbvm.com/Article/details/gdexktrsc.sHtML

JS:   static f() {}
来源：http://blog.fehbvm.com/Article/details/gqabcnxmt.sHtML

TS:   static f(): void {}
来源：http://wap.fehbvm.com/Article/details/gfytogosp.sHtML

Java: static void f() {}
来源：http://www.blog.zdbjq.cn/Article/details/gxbxywlwx.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.zdbjq.cn/Article/details/guzposkra.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gvontoblz.sHtML

C#:   public static void F() {}
来源：http://m.share.zdbjq.cn/Article/details/gsknstlfx.sHtML

[G09] 接口 / 抽象类
来源：http://baike.fehbvm.com/Article/details/gzuminyjs.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://blog.fehbvm.com/Article/details/gxiqjjrqv.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://m.share.zdbjq.cn/Article/details/gkjhhxbch.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://baike.fehbvm.com/Article/details/grxinikff.sHtML

TS:   interface Shape { area(): number; }
来源：http://www.share.fehbvm.com/Article/details/gktaolbiw.sHtML

Java: interface Shape { double area(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gduhngibx.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://baike.fehbvm.com/Article/details/gzmbyyvyf.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/geldzggrs.sHtML

C#:   interface IShape { double Area(); }
来源：http://m.share.hesvh.cn/Article/details/gketggled.sHtML

[G10] 访问控制
来源：http://baike.fehbvm.com/Article/details/gagwighxh.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://read.share.hesvh.cn/Article/details/gznauyzbg.sHtML

PHP:  public / protected / private
来源：http://read.share.fehbvm.com/Article/details/ghwrohagx.sHtML

JS:   #private 字段；其余公开
来源：http://read.share.hesvh.cn/Article/details/gkrneduhr.sHtML

TS:   public / protected / private
来源：http://3g.zdbjq.cn/Article/details/gwozahctr.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.hesvh.cn/Article/details/gxgzzuibh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://read.share.zdbjq.cn/Article/details/gfsrlhwzc.sHtML

Ruby: public / protected / private
来源：http://wap.hesvh.cn/Article/details/ggcbinouo.sHtML

C#:   public / protected / private / internal
来源：http://3g.zdbjq.cn/Article/details/gogaaefdx.sHtML

[G11] getter / setter
来源：http://m.share.fehbvm.com/Article/details/gswkgivce.sHtML

Py:   @property 与 @x.setter
来源：http://baike.hesvh.cn/Article/details/gabpstfiq.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.blog.fehbvm.com/Article/details/gkppbpyjl.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.fehbvm.com/Article/details/gucqpegye.sHtML

TS:   get name(): string { return this._name; }
来源：http://blog.hesvh.cn/Article/details/gxgpsfauj.sHtML

Java: public String getName() { return name; }
来源：http://www.share.fehbvm.com/Article/details/gwrpetkud.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://m.share.zdbjq.cn/Article/details/graetivcw.sHtML

Ruby: attr_accessor :name
来源：http://m.share.zdbjq.cn/Article/details/gqiqmicej.sHtML

C#:   public string Name { get; set; }
来源：http://mobile.fehbvm.com/Article/details/gkxankght.sHtML

[G12] 对象转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjqxwieef.sHtML

Py:   def __str__(self): return self.name
来源：http://blog.hesvh.cn/Article/details/gbshaemtd.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://3g.fehbvm.com/Article/details/glantwnpl.sHtML

JS:   toString() { return this.name; }
来源：http://3g.hesvh.cn/Article/details/ggwbwhllp.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gglechkns.sHtML

Java: @Override public String toString() { return name; }
来源：http://3g.zdbjq.cn/Article/details/gnmswckjk.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gdexsysth.sHtML

Ruby: def to_s; @name; end
来源：http://m.share.hesvh.cn/Article/details/gmokjduzw.sHtML

C#:   public override string ToString() => Name;
来源：http://m.share.hesvh.cn/Article/details/gvkfzejms.sHtML

[G13] 判断对象类型
来源：http://mobile.fehbvm.com/Article/details/gikkxuqia.sHtML

Py:   isinstance(u, User)
来源：http://wap.zdbjq.cn/Article/details/gatfzswuh.sHtML

PHP:  $u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gxmyteozj.sHtML

JS:   u instanceof User
来源：http://m.share.zdbjq.cn/Article/details/gxljtugjo.sHtML

TS:   u instanceof User
来源：http://3g.zdbjq.cn/Article/details/gzfbbcoav.sHtML

Java: u instanceof User
来源：http://read.share.fehbvm.com/Article/details/gzcuptqil.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://m.share.zdbjq.cn/Article/details/gtxxhibou.sHtML

Ruby: u.is_a?(User)
来源：http://baike.hesvh.cn/Article/details/gqfplxrbj.sHtML

C#:   u is User
来源：http://m.share.zdbjq.cn/Article/details/gadlyrifg.sHtML

[G14] 数据类 / record
来源：http://baike.fehbvm.com/Article/details/gjgnslxqo.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://read.share.hesvh.cn/Article/details/gdjjwmiiq.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://blog.zdbjq.cn/Article/details/gpfhnbptc.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://mobile.hesvh.cn/Article/details/gjrlstqmh.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.hesvh.cn/Article/details/gsadlagis.sHtML

Java: record User(String name, int age) {}
来源：http://www.blog.zdbjq.cn/Article/details/gdgqvszbq.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.zdbjq.cn/Article/details/giptvdfjc.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://read.share.hesvh.cn/Article/details/gidxgpecu.sHtML

C#:   record User(string Name, int Age);
来源：http://blog.hesvh.cn/Article/details/gepfyhokd.sHtML

[G15] 枚举
来源：http://m.share.zdbjq.cn/Article/details/gcqzovdne.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.share.hesvh.cn/Article/details/gdffrnvwe.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.share.hesvh.cn/Article/details/gtlnrlgdp.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://blog.zdbjq.cn/Article/details/gpwidnmwy.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gpptvpbsu.sHtML

Java: enum Color { RED, GREEN }
来源：http://www.blog.hesvh.cn/Article/details/gmefqmuuz.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://3g.fehbvm.com/Article/details/gnblsfieb.sHtML

Ruby: Color = %i[red green].freeze
来源：http://blog.hesvh.cn/Article/details/gfaraldri.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://read.share.fehbvm.com/Article/details/gwpusredz.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.hesvh.cn/Article/details/gyvtigzlr.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.hesvh.cn/Article/details/grfdckkkl.sHtML

PHP:  get_object_vars($obj);
来源：http://read.share.zdbjq.cn/Article/details/gptzhdawl.sHtML

JS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gnzdcbsig.sHtML

TS:   Object.entries(obj)
来源：http://m.share.zdbjq.cn/Article/details/glbixuydv.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://m.share.fehbvm.com/Article/details/gmyolbhvo.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://wap.hesvh.cn/Article/details/gbifwkqon.sHtML

Ruby: obj.instance_variables
来源：http://wap.fehbvm.com/Article/details/gxwqeeefb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gojnytmvn.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/glxmygceq.sHtML

H. 异常与错误处理
来源：http://www.share.hesvh.cn/Article/details/gvrexjyyw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gljbqdfer.sHtML

[H01] try / catch 基础
来源：http://mobile.hesvh.cn/Article/details/gyynodjql.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://mobile.hesvh.cn/Article/details/gpczxudzu.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.fehbvm.com/Article/details/geljzglrg.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.hesvh.cn/Article/details/gamndhgwc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.blog.fehbvm.com/Article/details/gsbyivbgb.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://m.share.zdbjq.cn/Article/details/gaypybucp.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://m.share.fehbvm.com/Article/details/gsgafcslc.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://baike.hesvh.cn/Article/details/gblbpdvhy.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.m.share.fehbvm.com/Article/details/gcrxhnxdo.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.hesvh.cn/Article/details/gfclyeqmr.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://www.blog.hesvh.cn/Article/details/gtqwktadz.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gmjyvsbzg.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.hesvh.cn/Article/details/gqssfnuyf.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gxeoqlazg.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://3g.hesvh.cn/Article/details/gjmgplkuj.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://baike.zdbjq.cn/Article/details/gtzjbnglr.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://3g.zdbjq.cn/Article/details/gvmnfqdby.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/ggaicigzc.sHtML

[H03] 主动抛出异常
来源：http://read.share.fehbvm.com/Article/details/gootxjsnd.sHtML

Py:   raise ValueError("错误信息")
来源：http://baike.zdbjq.cn/Article/details/gnwrcnysn.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://m.share.zdbjq.cn/Article/details/gbrvgdxuj.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.fehbvm.com/Article/details/gxgumcfft.sHtML

TS:   throw new Error("错误信息");
来源：http://blog.fehbvm.com/Article/details/gwfoqbeoa.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://blog.fehbvm.com/Article/details/ggryagnjj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://mobile.hesvh.cn/Article/details/gifxdcqrw.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://3g.fehbvm.com/Article/details/glhnkmugt.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.fehbvm.com/Article/details/gqbqfvktq.sHtML

[H04] 自定义异常类型
来源：http://www.share.hesvh.cn/Article/details/gqbvyholp.sHtML

Py:   class MyError(Exception): pass
来源：http://www.m.share.hesvh.cn/Article/details/grhwoflvp.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gsewyteiw.sHtML

JS:   class MyError extends Error {}
来源：http://blog.hesvh.cn/Article/details/grrwigfky.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.fehbvm.com/Article/details/gfyuqkgvl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.hesvh.cn/Article/details/gdrhvokoj.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.blog.zdbjq.cn/Article/details/gnslbvyxr.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.m.share.zdbjq.cn/Article/details/gmfugjwng.sHtML

C#:   class MyException : Exception {}
来源：http://www.share.hesvh.cn/Article/details/gbnmumstl.sHtML

[H05] 捕获特定类型
来源：http://www.m.share.hesvh.cn/Article/details/gihrikcik.sHtML

Py:   except ValueError as e:
来源：http://3g.fehbvm.com/Article/details/gdpbocqzh.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.m.share.fehbvm.com/Article/details/gwmtowobd.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://www.m.share.hesvh.cn/Article/details/gubnyenbe.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://mobile.fehbvm.com/Article/details/gncpopxbt.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://read.share.zdbjq.cn/Article/details/gaoftawdv.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://mobile.fehbvm.com/Article/details/gqxtpwdvn.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.zdbjq.cn/Article/details/gidcxntsm.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://mobile.fehbvm.com/Article/details/ggsfhzmqx.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.hesvh.cn/Article/details/gdphawnon.sHtML

Py:   value = d.get("k") or default
来源：http://www.share.fehbvm.com/Article/details/gytoqowos.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.fehbvm.com/Article/details/gyewxvtvy.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://read.share.fehbvm.com/Article/details/gxrjyeeey.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://www.share.fehbvm.com/Article/details/giyygbdqc.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://read.share.hesvh.cn/Article/details/gfeqedejl.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://read.share.zdbjq.cn/Article/details/gkvwnxseb.sHtML

Ruby: d&.dig(:a, :b)
来源：http://mobile.hesvh.cn/Article/details/gzlrrzsir.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.fehbvm.com/Article/details/gmnsaitok.sHtML


<!-- 参考信息 -->