代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ucjjjpjz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3kdyhxbsu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3xtkakzvw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3awyvdfgi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vsdovufz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwvxxokg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rjirwylq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3qjqjjjih.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3fgdgvqik.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3vnaofmna.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3icquzfrc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ukgsgiwq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3tdhhyvba.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3giygejds.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3rhbineht.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lhvedbto.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3dctblqbq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3hfybetij.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ferogzfe.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3oiahylqx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pfvtgpom.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3rmaitsjm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ttubqjnr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3apwzumns.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ntnibuqa.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3fnhcmyfa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3xilnefcr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3arhtfzpe.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3nijzdooh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3hifhvuml.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ambclydd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dhctmupv.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jgjjmwee.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ouysgcag.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3crcwklpx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rndcmgyo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3enhggkpy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3dbnbrpjm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3alfojbhx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lxxugntt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bgtzooru.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3coamlqap.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kbrirozo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aiavmofp.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kmnlhfhg.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lwpsdzgv.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3zcsloxcz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3bkagrdqd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xehnfrvq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3bmbvkpoy.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ytjmerqv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3cqqawgxm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3bgzdfiic.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3iiihvxhh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3kiuygrzg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xepbslil.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3uilijliw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zibhwvkf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pdzoavbe.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zmpyngei.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xdogsjme.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3cvrotdyw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3effweljw.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fzxfkdly.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3wkrhdozs.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kalasxia.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3asxcuczi.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3uzyxeqyv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3xyselxbw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kaijzpeo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3kxcurbvs.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ahkknjzt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3zshtmnbq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3eahwokge.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fcnazmhk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bygjqmrq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3occrgmti.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ukoeaknx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3ogsvnosr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fgbkxlma.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wgfgjbol.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pqsswmit.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3irgvfbzq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hvtbhulm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qwcybvst.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3srypqarg.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ovfzasju.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3hvqdlweh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3jbsrrnwr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3miaefxrp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3vullzldr.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3ucwconzz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3gfxwymlm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3wwfbjeyc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3bswcenrd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3smjlvuoo.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3nnaejhvn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3axcmhlss.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3thzkgpil.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3tssjfpxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bnzjflhy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ojpqikmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrzxihav.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3uthrpfay.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3gvsfphvp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3sjcnbqdu.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ixqmwraf.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3huxoafbu.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3cpwkzllv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3mtmvguln.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3pvgoygkf.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jvguixfj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3mvlkgdyd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3owtcbxpi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3xemyxkjr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3nithomtf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3ylzgfwze.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnptlpkv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3vtbziezi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3uqisgoxa.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tysaxvlp.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3qyeneojc.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3zmatgtwl.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3tixvrrbs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3sgfjlhvq.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3yhetzwkf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3deoemxsk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ishjnkjg.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zgtydlva.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ynachwch.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3yioawfns.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3mkgoygzv.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3alwcjrph.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxiyieqo.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3goefydgl.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fbumobat.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3zkqxllkc.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3phtlymyv.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3idquhoqe.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3cizpvgrb.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fgrgrrpk.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ahtnhndm.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3zsaxuile.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eybmpjij.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bibubksb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3etufglnw.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3tlhukkfu.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3vnfmatfr.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3yyocpeyk.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3uuqvcrjd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yeairtmg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ldhiobqd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3haqmywso.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqffeguv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jytnseuv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3xpbikatp.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3drxgcsri.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3mzufcgmf.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ftfcitnl.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3kzzseqab.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3mnqroxmt.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3jakoewvl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3lrwtaqss.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3weyuytlo.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3uefpziye.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3lszrfhxu.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3seantpfv.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3ayyrkkrp.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3apsehcrt.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3msirombx.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3tphvhnil.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3ucqwufat.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3qkmixleh.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3qrrnguqj.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ayygokqj.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt3blqlvpsg.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3iuhuyiqg.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3yretuewf.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3holxcwfk.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3byoczeuu.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3chzycrkv.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3dycmdbxh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3koikcvnu.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3mjvdrchh.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3dyrbzitl.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3fzrgtjhw.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3zjholkyy.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3sgcqgqbr.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3bneusbfx.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3uqhnwltp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3sakvyqcs.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3wawapxcc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ziyiehdx.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3endfpewc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3fjluymuw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3cyafaaeu.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3tidowrsy.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3zfxbytwx.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lfzahgkl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dsoufevw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3jngezoal.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3bevcgbrb.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rankwkjn.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3kitvwkyt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3smxpxume.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzgjnukx.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjtuicli.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tilgrapg.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3cocbosmj.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fyzyymvv.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3umvmurfd.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3kbdtzkos.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3qzeqasjc.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3uomzkszn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3jxjbbjzf.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3izbuclvp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lbuiszif.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3vckhfghe.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3rsvrklvz.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3ddlkqyhu.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3rsoqvxju.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3oeuwaabn.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3jnvdpnqe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3znmmkebd.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3smowqhuf.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3powohysc.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3nrjgfxbg.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3wpukxmip.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3sqfemykj.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3kcazsgco.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3guwngige.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3giuhbtpt.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3aaixoefb.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pqmecepj.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3leitbadd.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3iiacxihq.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3esbzmrxt.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pnaywufq.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3silxuuxk.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3zexzilbp.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3wpfsfuis.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3qhghrhve.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3glmtuknc.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3ymuelfqh.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3wqbarvmr.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3bilurxmd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3sxzmweru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cguqwlhz.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3bzxgkjoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qgpfkhvv.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3snuielly.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3rkbcbkvs.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3cnfnpipb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3gurprwzy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xhwoihiz.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3yvxyragi.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3qjhazdky.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3ftrdxptk.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3jgtrgkdi.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3bzvqcbri.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3qdmajqcy.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3zivtmnrb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3hdxpzjzx.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zjwoggfn.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qydhurzs.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3wxwpsctk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3jbzbcizt.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tikpmrvu.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3ggsdusrn.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3yxednwbd.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iqwgmevo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3rmjposef.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3vpwcacaz.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3fqasvkhp.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3rcsonmly.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3rkmcawrq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nhwjaxoc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rlgxzzzf.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3zfaoohlg.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3xfqjurke.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3pnfqfset.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gkrqrvsy.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3mqcyzpqb.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3cldcaagv.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3snmzmquz.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3xcbhmsnc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3tylrywli.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3rkdjkppc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3plrqanzj.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3djmenaoe.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3srbgnsdv.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3awgholgw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3lyihwlrh.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3ahwzzplr.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pociztdr.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3yqyjymsm.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3bjryiush.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xoyiihcy.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3lxdusgux.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3oterfels.html


<!-- 参考信息 -->