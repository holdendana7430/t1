代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gqegnuzij.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.zdbjq.cn/Article/details/ggspusdkm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.hesvh.cn/Article/details/gxvooobfc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.hesvh.cn/Article/details/gwmrhesdt.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gtyascvai.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gglyjtedi.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.hesvh.cn/Article/details/gsrfdxatd.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gjgpzsxuv.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/ghtceclts.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fehbvm.com/Article/details/grxnywomk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/grqgbzjkg.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fehbvm.com/Article/details/gltcotouy.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.hesvh.cn/Article/details/gnajuqywb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gmrdijxuk.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.fehbvm.com/Article/details/gwgycporb.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/gztkjsvbw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.share.fehbvm.com/Article/details/gjhrsjhvr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.zdbjq.cn/Article/details/gllkndeji.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gpwmdkuzo.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.hesvh.cn/Article/details/geyuwmcqc.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gijizxwim.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://baike.zdbjq.cn/Article/details/gqjcxqlfz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://blog.hesvh.cn/Article/details/gtmecodsk.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gujwfzjsj.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.fehbvm.com/Article/details/giookjmub.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.zdbjq.cn/Article/details/gcexhmzws.sHtML

PHP:  file_exists("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gaalomlqh.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/geaoxmepm.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/gwwyvutqd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/ggzlvmpjl.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gwyusudep.sHtML

Ruby: File.exist?("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzslyrqpn.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gygdudial.sHtML

[F06] 删除文件
来源：http://mobile.zdbjq.cn/Article/details/gfglgzhge.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ghoyzboug.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gxomklbkb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkojscdxq.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcvkgynae.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gmewailzy.sHtML

Go:   os.Remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gtxvbxymk.sHtML

Ruby: File.delete("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gkrrqvifi.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gtcdnloaq.sHtML

[F07] 创建目录（含多级）
来源：http://www.blog.zdbjq.cn/Article/details/grcfnnlzc.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.blog.fehbvm.com/Article/details/gymqyfrvt.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.hesvh.cn/Article/details/grdmiryvv.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.zdbjq.cn/Article/details/gioetditp.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gufpnetgw.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://m.share.hesvh.cn/Article/details/gxfhjfktz.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.fehbvm.com/Article/details/gnmfjbwxn.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gpuwsgrvv.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.blog.zdbjq.cn/Article/details/gvuinszsi.sHtML

[F08] 遍历目录
来源：http://wap.zdbjq.cn/Article/details/giodgnyof.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.zdbjq.cn/Article/details/gcwqqatay.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gcqsibpob.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gliextiqx.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.hesvh.cn/Article/details/gawccoasi.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gcwvdojmp.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gljvgsfka.sHtML

Ruby: Dir.children("dir")
来源：http://3g.fehbvm.com/Article/details/gzjeahxis.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.m.share.fehbvm.com/Article/details/gyhfvzxsh.sHtML

[F09] 获取文件大小
来源：http://read.share.hesvh.cn/Article/details/gcgqdymxp.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwfgvwwex.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gkunpujuk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/gxyfmhupa.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gngppkhib.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/gjqodexaa.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.zdbjq.cn/Article/details/gszmiybue.sHtML

Ruby: File.size("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gnacnmpqm.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fehbvm.com/Article/details/goaecsrvb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fehbvm.com/Article/details/gukmugdcx.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gapedlypl.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fehbvm.com/Article/details/gxlrclpir.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gelgqhisn.sHtML

TS:   path.extname("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/grgtpurzy.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.hesvh.cn/Article/details/gendthxpq.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gqdkyjxgl.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gbsarsgrp.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmcyzgtuh.sHtML

[F11] 复制与移动文件
来源：http://www.m.share.fehbvm.com/Article/details/gerwhcduk.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gmkhexpcr.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.hesvh.cn/Article/details/golvnydzr.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.fehbvm.com/Article/details/goqvstiks.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gryfoymxa.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gqcsscarr.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.zdbjq.cn/Article/details/grsubgdba.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.hesvh.cn/Article/details/gtlncdqbi.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gekcfskvt.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gmexecldw.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.hesvh.cn/Article/details/gkjtsavbk.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gbnlhfsnd.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.zdbjq.cn/Article/details/govsvieoh.sHtML

TS:   // 同上
来源：http://baike.fehbvm.com/Article/details/gsykgvmzs.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/ggnghnqii.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.fehbvm.com/Article/details/ghkakiicr.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.hesvh.cn/Article/details/guhyxbanf.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.zdbjq.cn/Article/details/gfbbfdhmk.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkjvrhxdh.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gkxtsmzwi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggjtazbfi.sHtML

[G01] 定义类
来源：http://baike.fehbvm.com/Article/details/gtrbeomhn.sHtML

Py:   class User: pass
来源：http://wap.hesvh.cn/Article/details/grdfvcmjp.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gkakpijur.sHtML

JS:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gtcxjqclc.sHtML

TS:   class User { name: string = ""; }
来源：http://baike.fehbvm.com/Article/details/gucheqkpp.sHtML

Java: class User {}
来源：http://m.share.zdbjq.cn/Article/details/gmrzsvguj.sHtML

Go:   type User struct { Name string }
来源：http://wap.fehbvm.com/Article/details/gunnvdujf.sHtML

Ruby: class User; end
来源：http://blog.zdbjq.cn/Article/details/gkvqleqgw.sHtML

C#:   class User {}
来源：http://read.share.fehbvm.com/Article/details/ghvtmsixd.sHtML

[G02] 构造函数
来源：http://wap.zdbjq.cn/Article/details/gysouxgbh.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fehbvm.com/Article/details/giwrawiip.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://www.share.fehbvm.com/Article/details/grnekqmqt.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gjtsppstw.sHtML

TS:   constructor(public name: string) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghksfusrs.sHtML

Java: User(String name) { this.name = name; }
来源：http://mobile.hesvh.cn/Article/details/ggbovbmca.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.m.share.zdbjq.cn/Article/details/gvutjxndc.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://m.share.zdbjq.cn/Article/details/gntsppatw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://m.share.fehbvm.com/Article/details/gdwjxhqhi.sHtML

[G03] 实例属性
来源：http://m.share.fehbvm.com/Article/details/gzfzcfqzk.sHtML

Py:   self.name = "x"
来源：http://3g.fehbvm.com/Article/details/gfzelthzz.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gzfzsbziv.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gfizxstam.sHtML

TS:   name: string = "x";
来源：http://blog.zdbjq.cn/Article/details/gtdzueoey.sHtML

Java: private String name;
来源：http://wap.zdbjq.cn/Article/details/gyyyfmczt.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.zdbjq.cn/Article/details/gwhglkwex.sHtML

Ruby: @name = "x"
来源：http://www.m.share.fehbvm.com/Article/details/gplrqyqqa.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.m.share.fehbvm.com/Article/details/gsrempkyx.sHtML

[G04] 定义方法
来源：http://baike.fehbvm.com/Article/details/gljnrozup.sHtML

Py:   def greet(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gyetcyppl.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://blog.hesvh.cn/Article/details/gglhetpme.sHtML

JS:   greet() { return this.name; }
来源：http://wap.zdbjq.cn/Article/details/gcjgduwci.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.fehbvm.com/Article/details/gjmwuvtuh.sHtML

Java: String greet() { return name; }
来源：http://3g.hesvh.cn/Article/details/ghjcjylvw.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.blog.zdbjq.cn/Article/details/ggwojkmec.sHtML

Ruby: def greet; @name; end
来源：http://www.m.share.hesvh.cn/Article/details/gevdgtpmo.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.hesvh.cn/Article/details/gjenztuvu.sHtML

[G05] 继承
来源：http://mobile.zdbjq.cn/Article/details/ghdqjzfdh.sHtML

Py:   class Admin(User): pass
来源：http://m.share.zdbjq.cn/Article/details/gkjxghicl.sHtML

PHP:  class Admin extends User {}
来源：http://baike.hesvh.cn/Article/details/gzqmoyvnk.sHtML

JS:   class Admin extends User {}
来源：http://blog.zdbjq.cn/Article/details/gznjbzdoh.sHtML

TS:   class Admin extends User {}
来源：http://baike.zdbjq.cn/Article/details/gkylxpeoh.sHtML

Java: class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gjylbssvr.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.fehbvm.com/Article/details/gvwnchtvr.sHtML

Ruby: class Admin < User; end
来源：http://www.m.share.hesvh.cn/Article/details/gvulgqjve.sHtML

C#:   class Admin : User {}
来源：http://read.share.hesvh.cn/Article/details/gbhuchoee.sHtML

[G06] 重写方法
来源：http://www.share.hesvh.cn/Article/details/gmdnkkrzc.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.zdbjq.cn/Article/details/gpkpcsznk.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://read.share.zdbjq.cn/Article/details/gydeqncyb.sHtML

JS:   greet() { return "admin"; }
来源：http://mobile.fehbvm.com/Article/details/gzzeqjlza.sHtML

TS:   greet(): string { return "admin"; }
来源：http://wap.fehbvm.com/Article/details/gpsazrvtx.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://blog.fehbvm.com/Article/details/gwbzogeac.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://read.share.zdbjq.cn/Article/details/gmbxiehrj.sHtML

Ruby: def greet; "admin"; end
来源：http://www.blog.zdbjq.cn/Article/details/gnyqwrsnm.sHtML

C#:   public override string Greet() => "admin";
来源：http://read.share.hesvh.cn/Article/details/gcmdqvzoa.sHtML

[G07] 调用父类方法
来源：http://baike.fehbvm.com/Article/details/ggxexxkmd.sHtML

Py:   super().greet()
来源：http://baike.fehbvm.com/Article/details/gsprgalss.sHtML

PHP:  parent::greet();
来源：http://www.blog.zdbjq.cn/Article/details/gshtoqyhc.sHtML

JS:   super.greet();
来源：http://baike.hesvh.cn/Article/details/gqrqgajfw.sHtML

TS:   super.greet();
来源：http://www.share.fehbvm.com/Article/details/gkdwftbkc.sHtML

Java: super.greet();
来源：http://m.share.fehbvm.com/Article/details/gqeslmrar.sHtML

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://3g.fehbvm.com/Article/details/gpddijjgl.sHtML

Ruby: super
来源：http://3g.fehbvm.com/Article/details/gssptudaj.sHtML

C#:   base.Greet();
来源：http://3g.hesvh.cn/Article/details/gajyqmujk.sHtML

[G08] 静态方法与属性
来源：http://m.share.hesvh.cn/Article/details/gaigtcufn.sHtML

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://read.share.hesvh.cn/Article/details/gxpvioygg.sHtML

PHP:  public static function f() {}
来源：http://wap.hesvh.cn/Article/details/gszuqhive.sHtML

JS:   static f() {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqmulqygw.sHtML

TS:   static f(): void {}
来源：http://blog.zdbjq.cn/Article/details/gjnedkpuz.sHtML

Java: static void f() {}
来源：http://mobile.zdbjq.cn/Article/details/gwfcswjsw.sHtML

Go:   // 无 static：用包级函数，按包名调用
来源：http://blog.fehbvm.com/Article/details/gkimddaqw.sHtML

Ruby: def self.f; end
来源：http://baike.hesvh.cn/Article/details/gsssuzhud.sHtML

C#:   public static void F() {}
来源：http://www.m.share.hesvh.cn/Article/details/gzwpjmkjf.sHtML

[G09] 接口 / 抽象类
来源：http://3g.zdbjq.cn/Article/details/gwzyxkgxk.sHtML

Py:   from abc import ABC, abstractmethod
来源：http://www.m.share.fehbvm.com/Article/details/gdhyuuznl.sHtML

PHP:  interface Shape { public function area(): float; }
来源：http://mobile.hesvh.cn/Article/details/gwtvvsfwp.sHtML

JS:   // 无接口：靠约定或 JSDoc
来源：http://blog.zdbjq.cn/Article/details/guithpufq.sHtML

TS:   interface Shape { area(): number; }
来源：http://blog.fehbvm.com/Article/details/gfleyitnx.sHtML

Java: interface Shape { double area(); }
来源：http://m.share.fehbvm.com/Article/details/geqzsfozw.sHtML

Go:   type Shape interface { Area() float64 }
来源：http://mobile.zdbjq.cn/Article/details/gklxlhqae.sHtML

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://read.share.zdbjq.cn/Article/details/gxjjgdcpn.sHtML

C#:   interface IShape { double Area(); }
来源：http://3g.fehbvm.com/Article/details/gpqoumfzj.sHtML

[G10] 访问控制
来源：http://m.share.zdbjq.cn/Article/details/gtdnrckbt.sHtML

Py:   约定 _protected / __private（不强制）
来源：http://mobile.hesvh.cn/Article/details/gqlhvmucu.sHtML

PHP:  public / protected / private
来源：http://wap.fehbvm.com/Article/details/gieaddbat.sHtML

JS:   #private 字段；其余公开
来源：http://www.m.share.fehbvm.com/Article/details/grrbicvyf.sHtML

TS:   public / protected / private
来源：http://www.share.fehbvm.com/Article/details/ggjbjtjel.sHtML

Java: public / protected / private / 默认包级
来源：http://mobile.fehbvm.com/Article/details/gletpipbh.sHtML

Go:   首字母大写可导出，小写仅包内可见
来源：http://baike.hesvh.cn/Article/details/gmdqtxtkm.sHtML

Ruby: public / protected / private
来源：http://read.share.zdbjq.cn/Article/details/gishoswgg.sHtML

C#:   public / protected / private / internal
来源：http://m.share.zdbjq.cn/Article/details/gltgusnvi.sHtML

[G11] getter / setter
来源：http://3g.hesvh.cn/Article/details/goxvpokot.sHtML

Py:   @property 与 @x.setter
来源：http://read.share.zdbjq.cn/Article/details/gjtqfubad.sHtML

PHP:  public function getName(): string { return $this->name; }
来源：http://blog.zdbjq.cn/Article/details/ghrfovgjo.sHtML

JS:   get name() { return this._name; }
来源：http://m.share.hesvh.cn/Article/details/gvdbmmkxw.sHtML

TS:   get name(): string { return this._name; }
来源：http://wap.zdbjq.cn/Article/details/gaqmoaxha.sHtML

Java: public String getName() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/guoyemuxk.sHtML

Go:   func (u User) GetName() string { return u.Name }
来源：http://read.share.zdbjq.cn/Article/details/gbwuielbf.sHtML

Ruby: attr_accessor :name
来源：http://www.blog.zdbjq.cn/Article/details/giqmdfoxd.sHtML

C#:   public string Name { get; set; }
来源：http://read.share.fehbvm.com/Article/details/gcfgvwitx.sHtML

[G12] 对象转字符串
来源：http://wap.hesvh.cn/Article/details/gznrosmam.sHtML

Py:   def __str__(self): return self.name
来源：http://mobile.zdbjq.cn/Article/details/gfmomyimo.sHtML

PHP:  public function __toString(): string { return $this->name; }
来源：http://wap.hesvh.cn/Article/details/gjivkkrvd.sHtML

JS:   toString() { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gtcbmyedh.sHtML

TS:   toString(): string { return this.name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdqhkewmm.sHtML

Java: @Override public String toString() { return name; }
来源：http://www.blog.hesvh.cn/Article/details/gztnagkou.sHtML

Go:   func (u User) String() string { return u.Name }
来源：http://m.share.fehbvm.com/Article/details/gdoglklgq.sHtML

Ruby: def to_s; @name; end
来源：http://www.m.share.fehbvm.com/Article/details/gjtyihfrr.sHtML

C#:   public override string ToString() => Name;
来源：http://www.m.share.zdbjq.cn/Article/details/ghdzperwi.sHtML

[G13] 判断对象类型
来源：http://blog.hesvh.cn/Article/details/gdwngkpjs.sHtML

Py:   isinstance(u, User)
来源：http://wap.hesvh.cn/Article/details/ghvcmsfax.sHtML

PHP:  $u instanceof User
来源：http://mobile.fehbvm.com/Article/details/gttobeamo.sHtML

JS:   u instanceof User
来源：http://www.m.share.fehbvm.com/Article/details/gaaaldyrr.sHtML

TS:   u instanceof User
来源：http://blog.fehbvm.com/Article/details/gntqvxtyu.sHtML

Java: u instanceof User
来源：http://blog.zdbjq.cn/Article/details/gbjkvcywd.sHtML

Go:   u, ok := v.(User)            // 类型断言
来源：http://blog.zdbjq.cn/Article/details/gywywzxfz.sHtML

Ruby: u.is_a?(User)
来源：http://m.share.hesvh.cn/Article/details/gqeejqvzl.sHtML

C#:   u is User
来源：http://read.share.fehbvm.com/Article/details/guctzpdbh.sHtML

[G14] 数据类 / record
来源：http://mobile.fehbvm.com/Article/details/gcdhxvmxi.sHtML

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.m.share.fehbvm.com/Article/details/gamkjapka.sHtML

PHP:  // 用 readonly 属性模拟
来源：http://read.share.zdbjq.cn/Article/details/gwfemnvkx.sHtML

JS:   // 无内置：普通类或对象字面量
来源：http://read.share.hesvh.cn/Article/details/gosdrqaym.sHtML

TS:   type User = { name: string; age: number };
来源：http://read.share.zdbjq.cn/Article/details/gdreeysvo.sHtML

Java: record User(String name, int age) {}
来源：http://m.share.fehbvm.com/Article/details/goorqlfxw.sHtML

Go:   type User struct { Name string; Age int }
来源：http://m.share.zdbjq.cn/Article/details/gsvzjxlwg.sHtML

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://blog.fehbvm.com/Article/details/glmloebol.sHtML

C#:   record User(string Name, int Age);
来源：http://read.share.fehbvm.com/Article/details/ggsuhhsvs.sHtML

[G15] 枚举
来源：http://www.blog.fehbvm.com/Article/details/ghfupmddl.sHtML

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://3g.zdbjq.cn/Article/details/gdptgybao.sHtML

PHP:  enum Color: string { case Red = "red"; }
来源：http://m.share.zdbjq.cn/Article/details/gocojahvm.sHtML

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.m.share.zdbjq.cn/Article/details/gzraljtmo.sHtML

TS:   enum Color { Red = 1, Green = 2 }
来源：http://mobile.zdbjq.cn/Article/details/gzgdtjafz.sHtML

Java: enum Color { RED, GREEN }
来源：http://baike.zdbjq.cn/Article/details/gougswwof.sHtML

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.blog.hesvh.cn/Article/details/goerrloto.sHtML

Ruby: Color = %i[red green].freeze
来源：http://baike.zdbjq.cn/Article/details/gugdnfnqt.sHtML

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.share.fehbvm.com/Article/details/gqyaokoli.sHtML

[G16] 对象转数组 / 字典
来源：http://blog.zdbjq.cn/Article/details/gnapqppxb.sHtML

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.m.share.zdbjq.cn/Article/details/gszlgikvi.sHtML

PHP:  get_object_vars($obj);
来源：http://mobile.fehbvm.com/Article/details/gfdqetsfv.sHtML

JS:   Object.entries(obj)
来源：http://baike.hesvh.cn/Article/details/gevpnzcmc.sHtML

TS:   Object.entries(obj)
来源：http://www.m.share.hesvh.cn/Article/details/glpbfilpt.sHtML

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://mobile.zdbjq.cn/Article/details/gijcsqlph.sHtML

Go:   // 手写转换，或用 mapstructure 库
来源：http://read.share.zdbjq.cn/Article/details/gcuqwffzj.sHtML

Ruby: obj.instance_variables
来源：http://m.share.zdbjq.cn/Article/details/gvzfhmprb.sHtML

C#:   // 用反射或 System.Text.Json
来源：http://3g.zdbjq.cn/Article/details/ggfwyzbxq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyvlemmht.sHtML

H. 异常与错误处理
来源：http://www.m.share.fehbvm.com/Article/details/grcyjdmbd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gnmbiqacy.sHtML

[H01] try / catch 基础
来源：http://3g.zdbjq.cn/Article/details/guowjjxci.sHtML

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.blog.zdbjq.cn/Article/details/gqjvwlhgj.sHtML

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.share.hesvh.cn/Article/details/gbaznvjny.sHtML

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://wap.zdbjq.cn/Article/details/gxpoqnlxc.sHtML

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.m.share.fehbvm.com/Article/details/gfnbeaino.sHtML

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://wap.zdbjq.cn/Article/details/gphowsuae.sHtML

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://blog.zdbjq.cn/Article/details/gxnbbdlki.sHtML

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.share.hesvh.cn/Article/details/ggiihbhlv.sHtML

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://3g.zdbjq.cn/Article/details/gbxsitgpk.sHtML

[H02] finally / ensure 收尾
来源：http://3g.fehbvm.com/Article/details/gmrnldtti.sHtML

Py:   try: f()⏎finally: cleanup()
来源：http://m.share.fehbvm.com/Article/details/gsmfknlrh.sHtML

PHP:  try { f(); } finally { cleanup(); }
来源：http://mobile.fehbvm.com/Article/details/gveihjcis.sHtML

JS:   try { f(); } finally { cleanup(); }
来源：http://read.share.fehbvm.com/Article/details/gbtqchlry.sHtML

TS:   try { f(); } finally { cleanup(); }
来源：http://blog.zdbjq.cn/Article/details/gvagclulr.sHtML

Java: try { f(); } finally { cleanup(); }
来源：http://wap.fehbvm.com/Article/details/gccmwjbwa.sHtML

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.m.share.zdbjq.cn/Article/details/gmzpongxy.sHtML

Ruby: begin; f; ensure; cleanup; end
来源：http://wap.zdbjq.cn/Article/details/gsblwclho.sHtML

C#:   try { F(); } finally { Cleanup(); }
来源：http://blog.fehbvm.com/Article/details/grtvajzfw.sHtML

[H03] 主动抛出异常
来源：http://wap.hesvh.cn/Article/details/gkftibomi.sHtML

Py:   raise ValueError("错误信息")
来源：http://read.share.hesvh.cn/Article/details/gbmwwwkkv.sHtML

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://baike.hesvh.cn/Article/details/gyiqwlrpi.sHtML

JS:   throw new Error("错误信息");
来源：http://www.blog.hesvh.cn/Article/details/gkzzwwqwj.sHtML

TS:   throw new Error("错误信息");
来源：http://3g.hesvh.cn/Article/details/gybepdhva.sHtML

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.share.fehbvm.com/Article/details/gerblmewj.sHtML

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.m.share.hesvh.cn/Article/details/gejuyxmng.sHtML

Ruby: raise ArgumentError, "错误信息"
来源：http://www.m.share.zdbjq.cn/Article/details/gcwpilrkb.sHtML

C#:   throw new ArgumentException("错误信息");
来源：http://read.share.hesvh.cn/Article/details/gykgrvldw.sHtML

[H04] 自定义异常类型
来源：http://blog.hesvh.cn/Article/details/gunsxiklg.sHtML

Py:   class MyError(Exception): pass
来源：http://m.share.fehbvm.com/Article/details/gpcdpjbhw.sHtML

PHP:  class MyError extends RuntimeException {}
来源：http://3g.fehbvm.com/Article/details/gfgnzwoen.sHtML

JS:   class MyError extends Error {}
来源：http://m.share.hesvh.cn/Article/details/gnjpjtwjr.sHtML

TS:   class MyError extends Error {}
来源：http://www.m.share.zdbjq.cn/Article/details/ggxobvgpl.sHtML

Java: class MyException extends RuntimeException {}
来源：http://wap.zdbjq.cn/Article/details/gbmhgrctp.sHtML

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://m.share.fehbvm.com/Article/details/gvzfhjtbo.sHtML

Ruby: class MyError < StandardError; end
来源：http://wap.fehbvm.com/Article/details/gpoacmzjx.sHtML

C#:   class MyException : Exception {}
来源：http://mobile.zdbjq.cn/Article/details/gnfnziuzd.sHtML

[H05] 捕获特定类型
来源：http://m.share.fehbvm.com/Article/details/gsqsdoxmz.sHtML

Py:   except ValueError as e:
来源：http://baike.hesvh.cn/Article/details/gmqhuoplm.sHtML

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://wap.zdbjq.cn/Article/details/gtdbtdybm.sHtML

JS:   if (e instanceof TypeError) {}
来源：http://read.share.zdbjq.cn/Article/details/gbgxwdban.sHtML

TS:   if (e instanceof TypeError) {}
来源：http://blog.fehbvm.com/Article/details/glmecihtz.sHtML

Java: catch (IOException | SQLException e) {}
来源：http://m.share.zdbjq.cn/Article/details/gcdlguyzo.sHtML

Go:   errors.Is(err, os.ErrNotExist)
来源：http://3g.zdbjq.cn/Article/details/gmxalkkfg.sHtML

Ruby: rescue ArgumentError => e
来源：http://www.m.share.zdbjq.cn/Article/details/gyqrgrmpl.sHtML

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://blog.hesvh.cn/Article/details/gxrqbxplr.sHtML

[H06] 可选值 / 空值安全访问
来源：http://www.share.hesvh.cn/Article/details/gfbkcllni.sHtML

Py:   value = d.get("k") or default
来源：http://baike.hesvh.cn/Article/details/gccuemiuu.sHtML

PHP:  $v = $d["k"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gkrzntzad.sHtML

JS:   obj?.a?.b;  d ?? default
来源：http://blog.fehbvm.com/Article/details/ghjwqshdl.sHtML

TS:   obj?.a?.b;  d ?? default
来源：http://m.share.zdbjq.cn/Article/details/gnxaubujx.sHtML

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.m.share.hesvh.cn/Article/details/gyfwfsdrd.sHtML

Go:   if v, ok := m["k"]; ok { }
来源：http://www.blog.fehbvm.com/Article/details/giepvhubv.sHtML

Ruby: d&.dig(:a, :b)
来源：http://www.share.hesvh.cn/Article/details/guvzjhgew.sHtML

C#:   obj?.A?.B ?? default
来源：http://blog.zdbjq.cn/Article/details/gvgkgclqk.sHtML


<!-- 参考信息 -->