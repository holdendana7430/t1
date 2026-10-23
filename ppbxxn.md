代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3szqpqxsk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3iwgpjyto.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3sqlpgmwv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kryfqagc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iekwwyvk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xeuzhase.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3puixfmqy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3koovnpyj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3lznoemhj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3znwkmztq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3vmolsrfm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3fipvumhc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3rgiilauw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ppnmvsnj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ibodkaar.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3kvbsmlji.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3odyfvocl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3vhihgcce.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jbvfstne.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3mtxybukm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fwcxdsur.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3zdhrvfjd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3yibilwgw.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jyjfcqrb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3whvilmcy.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3eqwtaloc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3kmfjvdda.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3yrxqtato.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bwagznyq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3akwdykvw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cghklbvp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kovjqybf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ktmwtcxk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vswieyvt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rdwleveo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ztllulph.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3flkyfrgl.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3rudetsnb.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lynrvmwt.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uxszcwlr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xheveqmc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xosmhtxh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qzqedoox.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3igvpaqmq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uozpmmok.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ndwzasri.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3ymuvrsdn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gvcyxkvh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3gpoyemqr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3whqckney.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ogcxznwy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3erqfluqo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3jtcpljwl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3imuhcmlo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3bhejxwwi.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3djgbqnnc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3xdamqzic.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3dcogmham.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3juinwrye.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pxyawjkw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ptestsaq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3dwxcatyo.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3eobfosie.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3byeoxgel.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3glrzdsfz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mgfwhfld.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mckxmwty.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3bbhogpqv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ccyairow.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zpwykqpd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3dshqguxp.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jrkdnrki.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3iibtvhha.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3vlothfgc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jjjdzuoq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lntuteaz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qrmukoov.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fuwpczvh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3idcnsphj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ocspzfyj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dchuupva.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3foeqnamq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3kofkfibk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ofhkunea.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nehbnnkm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qehrzmgo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3fbfnrcwt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3tdajcxnq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3efuqyiay.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jnwbujks.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3fddylhef.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ytutrptv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3rkrskphw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tzxqczko.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ivfpksjv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3yblbvkti.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3xlllpmzg.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vpnwzkkf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3piznroos.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3aubxavkp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gtqhqksw.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3dbnirotn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cawbsgut.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3glzwxczm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3eiwprkgj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxciebck.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3nwqkdwcw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3ahkocaby.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3fqwghetw.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3emezpisf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3fkhjojur.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gehaewov.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3eafguzsj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3wemnmfnk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3raucbock.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3khddanwe.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rqqudyut.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wajsatdz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3zlgghvfa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3gngqfawe.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vuefhdvv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3uxpnjnpp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ujdnweyd.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wxoyvvwk.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3fgnhxpse.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3dmolnawq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3hkqjgpgf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3anprvqso.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3adpsnpww.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3uslltiby.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3rljqvroa.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3bbppplxu.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uhmrnavz.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3oidmlwzw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ljlvmmax.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pmrwnufm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3qfhptrim.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3nkeytzyc.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3fkgcgetl.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3tepmcpyo.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3euluqxqg.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hrbsfnqt.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3powaalap.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gygbcjnf.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3gaitzkbc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3iqnhotax.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3fsnkfssg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3cbhtnfrw.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3uvtncdaz.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3clxobuom.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3okgvzuym.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mwwnllec.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gkrwenfj.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3bkminkwx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3uptifhmw.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3uomllzsh.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3ybleztln.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3jvmfhemh.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3lwjltkon.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ktehupez.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ilnmfwxj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3qqbsjhnl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3pzlsfcnt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3awbyiihd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3jprfipcp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3qalvdrkj.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3clgtbkmn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3eyhcackv.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3byytcteb.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3cspcflyp.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3wmxygssq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3suzzyjgc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xlqkwbjd.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3izldenaw.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3mmjeapyl.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3tathtmgr.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3xgnbyprf.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3hioipyrt.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.ydjk.org.cn/Article/details/gt3eajwkkwy.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukrtgmcz.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fgvvfmeg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3fbllstqj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3remtvxqf.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ggeonxyi.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3fpzmngjl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3esnpjkir.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3aexnrnmi.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3teymxswd.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3qcvfwzyw.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3ptrdmvoh.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3qyjplhsw.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pzaxllaj.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3jguxdvrn.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3tnlqedfh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3iprkqntf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nazpvyty.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3piyanjpa.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sjwaanmk.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxlwaqoq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3icjesugf.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3corfykcl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzlecvqw.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3ltftsogn.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3xtjeormz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3uoyebwmv.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3bvfhsvfz.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhcqqciq.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3kehfjvmt.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3hanbauwf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3pymsrbuc.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3nflmxvnn.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3nxyqrsfh.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3hahpkwhu.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3cyhilaap.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3gjipcult.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3mhdlxoaj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3yuhuxuzg.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3bwrzrmdj.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3anqhvdxl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3hqvuqsgk.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3yznnqqyw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3cwgpuvej.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3hzoemkeg.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3unuoacut.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3oibugbkx.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3slrzkkgu.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3zsqzzkkl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3kbcfqwid.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3jjvknguf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3eposrpwk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3qrtbwaag.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3ppxmfvay.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3dmywjzmx.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3aaiokbqn.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3tmtdqiwj.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3hrkwttcu.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3miqklyla.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3snslgsgy.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3novqhign.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3zevxehur.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3dyeiztxy.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3yadjqhqz.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3cqeunhph.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3trmukvhd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3bcszfhvw.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3zngcvvae.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3trmexzxt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmvqcerw.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3kxmahfes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xzalmkqs.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3upkqgruw.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3dfdbrijt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3kuwgwpsi.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3liocaohf.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3qlglwurh.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3dxkonard.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3qwypusqr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3gwdnvjtb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3omugbiky.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3tuqarumc.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ajwgwshz.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrfaemkq.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbnmqnha.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzzlfrho.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3noumdjti.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3eugffngr.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3npxpyutq.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3ebwzfsxk.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3bahpxgji.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3uheaovmx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3hzwyyggm.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vwbufkjn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3jjjsiuoq.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3otftxsqf.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3awlrrzjk.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3vofjfpsi.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mbwurfvy.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3dgqnjohh.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3bxvmzfqm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3hlikqaof.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vedyzoji.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3qnggttph.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3wzkxskug.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3ixtetwzt.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3asyslzxq.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3ujyevgms.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3dmcmbehj.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3imnpuvlo.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3sbucameg.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3uwtgegmf.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uulqjljl.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bniigmye.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3ercehxxr.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3zvctbaiw.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3ieijqwvn.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3uaoczwfe.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3ekgnlfik.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rdjnhgdg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3xwizezpo.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ltbxagry.html


<!-- 参考信息 -->