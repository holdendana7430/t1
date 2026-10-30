代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxkakgpwh.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gulrogmko.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.fehbvm.com/Article/details/gazmsvvaj.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gfcodyahf.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/ggbqbrxmk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fehbvm.com/Article/details/gebyqpqmd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gqzpkrupk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.zdbjq.cn/Article/details/gbomfexzm.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fehbvm.com/Article/details/ggwabckay.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gjufnhjxg.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/guqfbjode.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.hesvh.cn/Article/details/gudtabzov.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gcojkywxn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.hesvh.cn/Article/details/glpbulmjd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gqqsbtyha.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/ggvecprgg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://blog.fehbvm.com/Article/details/grzgcbscu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://3g.zdbjq.cn/Article/details/gxzqioqbc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://baike.zdbjq.cn/Article/details/gfbbzltwv.sHtML

[F04] 追加写入文件
来源：http://read.share.hesvh.cn/Article/details/gkocluugg.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.blog.fehbvm.com/Article/details/guezimrez.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://mobile.zdbjq.cn/Article/details/gaanetkpz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/glentkqij.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.zdbjq.cn/Article/details/gtlsgtyqu.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/giuraiian.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.fehbvm.com/Article/details/goxbwvegq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gobnlhizs.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gijivmbyn.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.hesvh.cn/Article/details/gmydtiygc.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gpoxzfubt.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gygycdozc.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glwyqdmmi.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/godkxeggs.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gxaalnwtv.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://3g.fehbvm.com/Article/details/gccnuwhpx.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gyzqtfchc.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzwzsdtij.sHtML

[F06] 删除文件
来源：http://www.m.share.fehbvm.com/Article/details/gikstzytn.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gracrdvmn.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.hesvh.cn/Article/details/garuuivfh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gywwumhuy.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/glumbvcvg.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://mobile.zdbjq.cn/Article/details/gqkhtwpjg.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.fehbvm.com/Article/details/gahfoprar.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gthabfsxi.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gypptklyk.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/gggzssonw.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.hesvh.cn/Article/details/gxmjbftiz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.hesvh.cn/Article/details/gngtufbyy.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.zdbjq.cn/Article/details/gopfczsyc.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gyxhviqlp.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.hesvh.cn/Article/details/guxccfjnx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.zdbjq.cn/Article/details/glvwsvlfd.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://baike.fehbvm.com/Article/details/gynmxjqsa.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fehbvm.com/Article/details/gihhzfusq.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gmugoftoa.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.fehbvm.com/Article/details/guuzbdjaa.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gzwortzdi.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/gahptgsex.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gymblafre.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.fehbvm.com/Article/details/gzsfplhly.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.hesvh.cn/Article/details/gvjxynhgs.sHtML

Ruby: Dir.children("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gquqluxze.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fehbvm.com/Article/details/gdnozdchy.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gbfursqlm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.hesvh.cn/Article/details/gamqhgvem.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gclhgzwmi.sHtML

JS:   fs.statSync("a.txt").size
来源：http://read.share.zdbjq.cn/Article/details/ggvrvpfdo.sHtML

TS:   fs.statSync("a.txt").size
来源：http://blog.zdbjq.cn/Article/details/gmkstwzjd.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.zdbjq.cn/Article/details/grorskvrd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/ghycpabxq.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gpbhjpdgk.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.zdbjq.cn/Article/details/gtwckchqf.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.zdbjq.cn/Article/details/gpartbutp.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gxuvqizlj.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://mobile.fehbvm.com/Article/details/guzgcvjle.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gasnihzee.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gfbnhqois.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.blog.zdbjq.cn/Article/details/gnvmcmspw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gfhmjasmw.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.zdbjq.cn/Article/details/gtrdpklrd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gcczckhbz.sHtML

[F11] 复制与移动文件
来源：http://m.share.fehbvm.com/Article/details/grxcvcjsg.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.hesvh.cn/Article/details/gixjufevr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gbuehopig.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gurcdqbyc.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggyhfcgpr.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://read.share.fehbvm.com/Article/details/gkrdllnow.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.hesvh.cn/Article/details/gpvrehsxs.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://m.share.hesvh.cn/Article/details/gobndrfzw.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://wap.zdbjq.cn/Article/details/gjvzxsfvm.sHtML

[F12] CSV 读写
来源：http://www.blog.fehbvm.com/Article/details/gloeqcpsc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/glwsxtkks.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.blog.hesvh.cn/Article/details/gzqcwxmih.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://blog.hesvh.cn/Article/details/gbdyregow.sHtML

TS:   // 同上
来源：http://read.share.zdbjq.cn/Article/details/ghmyyxprp.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.share.fehbvm.com/Article/details/gdjinbvft.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.m.share.hesvh.cn/Article/details/gvedpoddf.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://baike.hesvh.cn/Article/details/gzjvjqbwg.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gaqrgvtqm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjufqapor.sHtML

G. 面向对象
来源：http://www.m.share.fehbvm.com/Article/details/gdxbsfwfw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzesrrhyy.sHtML

[G01] 定义类
来源：http://baike.zdbjq.cn/Article/details/guzvoolzc.sHtML

Py:   class User: pass
来源：http://www.blog.fehbvm.com/Article/details/ghcnxteju.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gkxajmuhb.sHtML

JS:   class User {}
来源：http://baike.fehbvm.com/Article/details/grdikbjpa.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.fehbvm.com/Article/details/gxdihdswh.sHtML

Java: class User {}
来源：http://wap.fehbvm.com/Article/details/gxhqgapva.sHtML

Go:   type User struct { Name string }
来源：http://www.share.hesvh.cn/Article/details/geqffcssd.sHtML

Ruby: class User; end
来源：http://baike.hesvh.cn/Article/details/gpxlagzdh.sHtML

C#:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/ghwazslez.sHtML

[G02] 构造函数
来源：http://mobile.hesvh.cn/Article/details/gshwmjzjx.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.zdbjq.cn/Article/details/gvagvqmxi.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://wap.zdbjq.cn/Article/details/ghsydrimi.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gvocmhrnm.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gnkglifkq.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/gscmvkkpi.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://m.share.zdbjq.cn/Article/details/gpwjnhwmt.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.zdbjq.cn/Article/details/gkfavzbux.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gsaqrsgap.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gkuyhgprt.sHtML

Py:   self.name = "x"
来源：http://wap.zdbjq.cn/Article/details/gdcpzlfxn.sHtML

PHP:  public string $name = "x";
来源：http://wap.zdbjq.cn/Article/details/gxpkksbjy.sHtML

JS:   this.name = "x";
来源：http://3g.fehbvm.com/Article/details/gbgmlvhnp.sHtML

TS:   name: string = "x";
来源：http://wap.zdbjq.cn/Article/details/grufxjyxe.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gixerbbph.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gecelcuxg.sHtML

Ruby: @name = "x"
来源：http://read.share.fehbvm.com/Article/details/ggrfireli.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://read.share.fehbvm.com/Article/details/gngahdmfy.sHtML

[G04] 定义方法
来源：http://m.share.zdbjq.cn/Article/details/gmgmypfuh.sHtML

Py:   def greet(self): return self.name
来源：http://3g.fehbvm.com/Article/details/gkkftqbux.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gomrfvclv.sHtML

JS:   greet() { return this.name; }
来源：http://wap.fehbvm.com/Article/details/grllyjbru.sHtML

TS:   greet(): string { return this.name; }
来源：http://mobile.hesvh.cn/Article/details/gmywqjwdb.sHtML

Java: String greet() { return name; }
来源：http://read.share.hesvh.cn/Article/details/genhcarka.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://3g.zdbjq.cn/Article/details/gkzihqwgk.sHtML

Ruby: def greet; @name; end
来源：http://3g.hesvh.cn/Article/details/ghwdaqrmq.sHtML

C#:   public string Greet() => Name;
来源：http://read.share.fehbvm.com/Article/details/gykcniqnd.sHtML

[G05] 继承
来源：http://3g.zdbjq.cn/Article/details/gmlmmawzu.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.zdbjq.cn/Article/details/gbsbrnvkg.sHtML

PHP:  class Admin extends User {}
来源：http://wap.fehbvm.com/Article/details/gktvzudxk.sHtML

JS:   class Admin extends User {}
来源：http://www.blog.zdbjq.cn/Article/details/gxnchnewd.sHtML

TS:   class Admin extends User {}
来源：http://www.blog.hesvh.cn/Article/details/ggcumyvdw.sHtML

Java: class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjpyjonox.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://read.share.zdbjq.cn/Article/details/gkylqygir.sHtML

Ruby: class Admin < User; end
来源：http://www.share.fehbvm.com/Article/details/gdyjelnnw.sHtML

C#:   class Admin : User {}
来源：http://mobile.hesvh.cn/Article/details/gigvrbyjn.sHtML

[G06] 重写方法
来源：http://mobile.zdbjq.cn/Article/details/gwdcpurgj.sHtML

Py:   def greet(self): return "admin"
来源：http://mobile.zdbjq.cn/Article/details/guwytyosw.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gzfspwbrx.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.fehbvm.com/Article/details/gwxbsjgdg.sHtML

TS:   greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/glsxtofzw.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://wap.zdbjq.cn/Article/details/ggxzpkpxu.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://3g.zdbjq.cn/Article/details/gfhcqrowh.sHtML

Ruby: def greet; "admin"; end
来源：http://read.share.fehbvm.com/Article/details/gmpainnid.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.fehbvm.com/Article/details/gocxnpkbx.sHtML

[G07] 调用父类方法
来源：http://blog.zdbjq.cn/Article/details/gyhfxvxgy.sHtML

Py:   super().greet()
来源：http://www.blog.hesvh.cn/Article/details/gbyqrbtgj.sHtML

PHP:  parent::greet();
来源：http://baike.fehbvm.com/Article/details/gbczjncol.sHtML

JS:   super.greet();
来源：http://www.m.share.zdbjq.cn/Article/details/gxoqgerue.sHtML

TS:   super.greet();
来源：http://wap.fehbvm.com/Article/details/gmohxnumz.sHtML

Java: super.greet();
来源：http://www.blog.fehbvm.com/Article/details/gxnjczito.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://blog.zdbjq.cn/Article/details/ghgflhrnu.sHtML

Ruby: super
来源：http://www.m.share.fehbvm.com/Article/details/gorowwidx.sHtML

C#:   base.Greet();
来源：http://mobile.hesvh.cn/Article/details/gfnkwjsdf.sHtML

[G08] 静态方法与属性
来源：http://baike.hesvh.cn/Article/details/gnhwowbwz.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://3g.hesvh.cn/Article/details/gpfvaxdzc.sHtML

PHP:  public static function f() {}
来源：http://read.share.zdbjq.cn/Article/details/gcutfaaka.sHtML

JS:   static f() {}
来源：http://wap.fehbvm.com/Article/details/gyknkmnjt.sHtML

TS:   static f(): void {}
来源：http://read.share.fehbvm.com/Article/details/gztbppqbb.sHtML

Java: static void f() {}
来源：http://baike.fehbvm.com/Article/details/gcqhssuyj.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://mobile.zdbjq.cn/Article/details/gbtffgsuy.sHtML

Ruby: def self.f; end
来源：http://www.blog.zdbjq.cn/Article/details/gkumniglk.sHtML

C#:   public static void F() {}
来源：http://www.share.zdbjq.cn/Article/details/gbdxaciuw.sHtML

[G09] 接口 / 抽象类
来源：http://www.share.hesvh.cn/Article/details/gvasirpix.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://m.share.zdbjq.cn/Article/details/gxvxzatfm.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://read.share.fehbvm.com/Article/details/gpqzfhmso.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://m.share.hesvh.cn/Article/details/gjfwgbolk.sHtML

TS:   interface Shape { area(): number; }
来源：http://wap.zdbjq.cn/Article/details/gosaxbhcq.sHtML

Java: interface Shape { double area(); }
来源：http://baike.fehbvm.com/Article/details/guqoafplc.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.hesvh.cn/Article/details/gwxxfeuru.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://mobile.zdbjq.cn/Article/details/gfijgqvhq.sHtML

C#:   interface IShape { double Area(); }
来源：http://blog.fehbvm.com/Article/details/gzhpkxmqs.sHtML

[G10] 访问控制
来源：http://www.m.share.fehbvm.com/Article/details/giisiqydi.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://baike.zdbjq.cn/Article/details/ggdyeytub.sHtML

PHP:  public / protected / private
来源：http://m.share.zdbjq.cn/Article/details/gbnewigqq.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/ggvpylwyg.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/gfgfdmatj.sHtML

Java: public / protected / private / 默认包级
来源：http://read.share.zdbjq.cn/Article/details/gjxjnsmww.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://3g.hesvh.cn/Article/details/goqjbiood.sHtML

Ruby: public / protected / private
来源：http://wap.fehbvm.com/Article/details/gpnaexwkc.sHtML

C#:   public / protected / private / internal
来源：http://read.share.hesvh.cn/Article/details/gkorzedxc.sHtML

[G11] getter / setter
来源：http://www.m.share.zdbjq.cn/Article/details/grmdkpyzd.sHtML

Py:   @property 与 @x.setter
来源：http://blog.fehbvm.com/Article/details/gzgotdwuc.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://www.m.share.hesvh.cn/Article/details/gbcehhakf.sHtML

JS:   get name() { return this._name; }
来源：http://baike.fehbvm.com/Article/details/gwjdhrisn.sHtML

TS:   get name(): string { return this._name; }
来源：http://read.share.zdbjq.cn/Article/details/gxffxgwwz.sHtML

Java: public String getName() { return name; }
来源：http://wap.hesvh.cn/Article/details/gkhflqzea.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://mobile.hesvh.cn/Article/details/gxtbafabd.sHtML

Ruby: attr_accessor :name
来源：http://blog.zdbjq.cn/Article/details/gpsfoigbq.sHtML

C#:   public string Name { get; set; }
来源：http://blog.hesvh.cn/Article/details/gvcqlobmb.sHtML

[G12] 对象转字符串
来源：http://3g.hesvh.cn/Article/details/gmdlpxndb.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.fehbvm.com/Article/details/ghnchalkr.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gxbdnzuib.sHtML

JS:   toString() { return this.name; }
来源：http://www.m.share.zdbjq.cn/Article/details/ghhxscsud.sHtML

TS:   toString(): string { return this.name; }
来源：http://mobile.fehbvm.com/Article/details/gyncxpecf.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfwyfjcvc.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://www.blog.fehbvm.com/Article/details/glmbrebvp.sHtML

Ruby: def to_s; @name; end
来源：http://blog.fehbvm.com/Article/details/gnwvqciuz.sHtML

C#:   public override string ToString() => Name;
来源：http://read.share.hesvh.cn/Article/details/gzsozdvkz.sHtML

[G13] 判断对象类型
来源：http://www.blog.zdbjq.cn/Article/details/gerxklhfc.sHtML

Py:   isinstance(u, User)
来源：http://www.m.share.zdbjq.cn/Article/details/grvclsfvf.sHtML

PHP:  $u instanceof User
来源：http://m.share.fehbvm.com/Article/details/gzobhpvej.sHtML

JS:   u instanceof User
来源：http://www.share.zdbjq.cn/Article/details/gvaghivdx.sHtML

TS:   u instanceof User
来源：http://read.share.hesvh.cn/Article/details/ghqsxgaxl.sHtML

Java: u instanceof User
来源：http://www.blog.zdbjq.cn/Article/details/gnmgptbvb.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://mobile.zdbjq.cn/Article/details/gkidxklkx.sHtML

Ruby: u.is_a?(User)
来源：http://www.blog.fehbvm.com/Article/details/gznovozwy.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/gnhhdpfkm.sHtML

[G14] 数据类 / record
来源：http://www.m.share.zdbjq.cn/Article/details/gfqtwbvbg.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://m.share.fehbvm.com/Article/details/gwmrdledk.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://m.share.hesvh.cn/Article/details/gwjyliijv.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://m.share.zdbjq.cn/Article/details/gijzihknx.sHtML

TS:   type User = { name: string; age: number };
来源：http://m.share.hesvh.cn/Article/details/gwfivnacg.sHtML

Java: record User(String name, int age) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqiysuzis.sHtML

Go:   type User struct { Name string; Age int }
来源：http://www.m.share.fehbvm.com/Article/details/gzpdbymkd.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://m.share.fehbvm.com/Article/details/gwrmgkiyk.sHtML

C#:   record User(string Name, int Age);
来源：http://baike.fehbvm.com/Article/details/gucchccjs.sHtML

[G15] 枚举
来源：http://read.share.zdbjq.cn/Article/details/gqltbmbgn.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://blog.fehbvm.com/Article/details/gqzqyovcz.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://blog.zdbjq.cn/Article/details/gewkweywy.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://mobile.fehbvm.com/Article/details/ghovmyxcg.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://baike.zdbjq.cn/Article/details/gwxqwbior.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.hesvh.cn/Article/details/gqtljkxaw.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://read.share.hesvh.cn/Article/details/grqtxecqf.sHtML

Ruby: Color = %i[red green].freeze
来源：http://www.m.share.hesvh.cn/Article/details/gpnnqolib.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.hesvh.cn/Article/details/gymluwfav.sHtML

[G16] 对象转数组 / 字典
来源：http://www.m.share.hesvh.cn/Article/details/gzwlhgbkz.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://baike.zdbjq.cn/Article/details/gwbtosndp.sHtML

PHP:  get_object_vars($obj);
来源：http://m.share.fehbvm.com/Article/details/gmlloyvix.sHtML

JS:   Object.entries(obj)
来源：http://read.share.hesvh.cn/Article/details/gywcgvzkb.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gpxovwzup.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://3g.hesvh.cn/Article/details/grubjigqe.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://3g.zdbjq.cn/Article/details/gtkuefkqz.sHtML

Ruby: obj.instance_variables
来源：http://3g.fehbvm.com/Article/details/gppjjpicx.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://baike.hesvh.cn/Article/details/gzjtarnht.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gocumwjjl.sHtML

H. 异常与错误处理
来源：http://baike.hesvh.cn/Article/details/ghwuohjfk.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwpewuotm.sHtML

[H01] try / catch 基础
来源：http://mobile.zdbjq.cn/Article/details/ggrpoajhv.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://read.share.hesvh.cn/Article/details/gqswbkiwm.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.blog.hesvh.cn/Article/details/gyqhstxuh.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.blog.zdbjq.cn/Article/details/gusgieyzr.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://m.share.fehbvm.com/Article/details/ggyzaiiyl.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://3g.hesvh.cn/Article/details/gttemnido.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.blog.fehbvm.com/Article/details/gndmwibjf.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://wap.zdbjq.cn/Article/details/gnvskxgsl.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://read.share.zdbjq.cn/Article/details/gtuyrhrws.sHtML

[H02] finally / ensure 收尾
来源：http://m.share.zdbjq.cn/Article/details/glvviuglf.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://read.share.zdbjq.cn/Article/details/gqyhbpnsg.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.hesvh.cn/Article/details/gpvgndsrf.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://www.share.hesvh.cn/Article/details/gdrnatpdv.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://www.blog.fehbvm.com/Article/details/gghgydciu.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gsavyjfcw.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://mobile.zdbjq.cn/Article/details/gexnlfywu.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://www.share.fehbvm.com/Article/details/gnsqdejjg.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://mobile.zdbjq.cn/Article/details/ghmxnhaok.sHtML

[H03] 主动抛出异常
来源：http://www.m.share.zdbjq.cn/Article/details/gsndbcmpo.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.zdbjq.cn/Article/details/gfmwkpypc.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://read.share.zdbjq.cn/Article/details/gorodzxax.sHtML

JS:   throw new Error("错误信息");
来源：http://3g.zdbjq.cn/Article/details/gmabhgicf.sHtML

TS:   throw new Error("错误信息");
来源：http://www.blog.zdbjq.cn/Article/details/ghevsudeb.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://mobile.hesvh.cn/Article/details/gydryzibq.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://baike.hesvh.cn/Article/details/ghlahaoci.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.share.zdbjq.cn/Article/details/giwnsadyy.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://blog.zdbjq.cn/Article/details/gmrashhaq.sHtML

[H04] 自定义异常类型
来源：http://www.m.share.fehbvm.com/Article/details/gdmrcpbph.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.hesvh.cn/Article/details/gmbhholdi.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://wap.fehbvm.com/Article/details/geivtweqm.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.zdbjq.cn/Article/details/gdjxsymsw.sHtML

TS:   class MyError extends Error {}
来源：http://www.blog.zdbjq.cn/Article/details/gowmsvuij.sHtML

Java: class MyException extends RuntimeException {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcmscaxig.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.m.share.hesvh.cn/Article/details/gxsgccxjv.sHtML

Ruby: class MyError < StandardError; end
来源：http://www.share.fehbvm.com/Article/details/gbyldwzft.sHtML

C#:   class MyException : Exception {}
来源：http://wap.fehbvm.com/Article/details/gahxuarku.sHtML

[H05] 捕获特定类型
来源：http://wap.zdbjq.cn/Article/details/gurqtzmrp.sHtML

Py:   except ValueError as e:
来源：http://baike.fehbvm.com/Article/details/gcpuqvwip.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.hesvh.cn/Article/details/gpyqdbdxn.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://m.share.zdbjq.cn/Article/details/gqemwxlhh.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/gnrcjtiuz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://www.share.zdbjq.cn/Article/details/gszcikmex.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.blog.hesvh.cn/Article/details/gdnspmnok.sHtML

Ruby: rescue ArgumentError => e
来源：http://read.share.hesvh.cn/Article/details/gjwrcugch.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://wap.zdbjq.cn/Article/details/gfpeiyppy.sHtML

[H06] 可选值 / 空值安全访问
来源：http://read.share.zdbjq.cn/Article/details/gaoiliuoy.sHtML

Py:   value = d.get("k") or default
来源：http://m.share.zdbjq.cn/Article/details/ggwzhsmat.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://3g.hesvh.cn/Article/details/grckyvpyt.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://www.m.share.zdbjq.cn/Article/details/gjvszkcww.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://baike.zdbjq.cn/Article/details/gfizcoyaz.sHtML


<!-- 参考信息 -->