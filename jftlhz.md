代发 wailian999

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lqhheogv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hcjymair.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3bxzfftqc.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xefpaasc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3mypgfsrj.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3nleduffg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3pwzknykt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3cprmijdv.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkxhasgw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3arquclys.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3lfxjrrin.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3olopthcp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vzunlbkq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3apyvwnax.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3spqramac.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3bwafqqkk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kxpuihwd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3alwaqagf.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3przoknvo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ymplkirb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3krdcftzl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3hqfcprhe.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3arziptib.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3zdjukyus.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3tolygurh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3gqhbtgka.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3oldxzhoh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lwlzcyia.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3bwaqatsu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3crfymywh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3bzkjjzpy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sdjbwjop.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3nuoxjsje.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3ynxlelma.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jxxcepso.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qzuqamhh.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3duzqoabd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jmkbqrrt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3ouluodzn.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jprqiiwi.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eybjlpig.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3qyyerqzg.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hjetcmku.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3evfyaqrq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oacskdqz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eanettrv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3llfxrebd.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xbkgyvck.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3raxrqbla.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fqeeaceh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qemkxkeh.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wohebcgd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ybdqfdlq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3mbqbugwq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ovmepptc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3qenoanid.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3wgrtltzj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3zsevooad.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3kjhmnxfq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3majuehus.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3cukabfja.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zekoixtl.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ajdcuuek.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3uwciehdb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3sgxzxqaq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rexrjida.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3yqkltfuq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3pmjilzjg.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3mbdrhzvu.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ynpjfyzr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3lpmclffj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3petbsoyy.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3veafbvph.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dxzgheua.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3otsfwfol.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zzqzxxny.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3jvtfczoe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3mevqcjnc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3umepjcvw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hieakpjt.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lgfkfgfs.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bebdfnny.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3nvtgochy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kzeictnh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rtdbgtdd.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tvqaqpni.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3msfpdpkk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwjfqmfm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3dcvgnwkv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mderljuu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ydowepzn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xuobgzne.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3pxexdold.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zwhkoxml.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hcosgivn.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3hrzguvnq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3aucdgzuw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3xrmaottp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3mcfpaylh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3hapdbloq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3bxhcsioa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3uuylflqs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3bwhsgwox.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3vgbibylk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwwjmwel.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3lqahxeem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wfimkohb.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3rnikdies.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mufzknie.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3odzbzdkc.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3mdlpfwyk.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3zqyryhet.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3filflvvb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3maajhzmp.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3peeikjpp.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wgjplrrg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3lsodwbmn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3ybjiqwxy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jogtttka.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrjosqsq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3iaucunwr.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ghnsydov.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3hkcavqae.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3njdxhuqr.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jsqxduse.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3wnmzpzyn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ozqzsjzw.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3jdsfaqma.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3nnsibejs.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iimvzivl.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3tytmbqjw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3ysfkbuoq.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3tbymglgh.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3fpejsron.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3splpnqsk.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3owgeiare.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rtaefsbq.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3stiavoxn.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3abkfbxxs.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mbeeldaw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3jomarisf.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3vnnsvdor.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3sosminvz.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3tzcksxsi.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fewhwmhm.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ctljyhos.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yzyusziy.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hrbtsgii.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcpeduut.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3mqlwgxjx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ovoputhq.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3fogenxyo.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3qptbjfks.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ezxkrbng.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hnkidtfp.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3usqyctmy.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qwrnqlnx.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhvwutlp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3bbghusde.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3lvmkszbk.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3zwnowesu.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3zettxgch.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3tvrvfdga.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3opjeqcxi.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3enxrwxaj.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wjeggfzg.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3ddkepbmt.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3vhsfybst.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3whflulmp.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3gqcawzds.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3omeqpjim.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3foaxrsyr.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3kwdkajug.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3aelotzpj.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3rremglsd.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3hiwdzabr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3vroexnzq.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3cnpdnpfb.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3ziubyzrg.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ubwjphpv.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3dwkpjqgs.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3tjcmhbux.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ukeikbic.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3deaiaufc.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3egphjmhl.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3aaymcmag.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3aurulvzi.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3ahulqtue.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3nqrgyrkq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3drmbtfpt.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3yigrapwc.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3frtrtxkb.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3cywfvyjp.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3txapkmki.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3firyyzjz.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3umomqgtk.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3ukvducgc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3fsryjirv.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3vbwgxvan.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pihmmhem.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3rnfdkdmi.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jdxtkitr.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qhdljbcl.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3vsdgnpbw.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3vhnukmay.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3nngpjkgh.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3zfkmhgpb.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3vmdaztwf.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3asnhrdjp.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqsezbjj.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zqteogwh.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hdppxciz.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xbhghuqt.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3dofvwegs.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3hcavbmky.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3mgsfyyes.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3neiipmsz.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3agyxpqfy.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3nlwvnkso.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ziqkacqe.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3oorueexk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3gkuffsno.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3gixotlbb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3rqkjcbhg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3sngjsrjw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3vaeacuxl.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3wolxmmds.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3eiisfurz.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3quxvwusq.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gjejcnci.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3kuilejnc.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3pqescxwx.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ftbibkvm.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3sszpjyrm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3ciudgime.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3lpipagum.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3yuxhibes.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3snklalzu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3jdxugqgs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3mghssdzi.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3itoqdmfk.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3jwskbqwl.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3qyzjcbwx.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3kqzlsbci.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3cdpzcpyo.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3lzadutuk.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nhbtfzfz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3cmpqyzvx.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3fdwmvhld.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3izwsxing.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3jifmspdh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3titpqtru.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ngutslut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3srnwxevq.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3lffjymtp.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3meblikmt.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vtrgexki.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hejiuksa.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3nqvvzzpa.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3jbrgjrsb.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3roosutss.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3rousoftz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3sgtywrnj.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3oyttmcuo.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3ekhevwsq.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uvwwehvh.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sghxrvxj.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xtdkhkkz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mdqxaslu.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3nynlvoed.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3ickqxgud.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nzahtobi.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mjdazkki.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3xthqixvn.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3itsvhxfw.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wdcpcbna.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3iosvnraa.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rbnpksmo.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3rdilrhes.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3uuauqbvq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3spfcpcwx.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3zfmpkuka.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3jifxnoap.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3kkkrecyc.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3slcteasu.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3ajvtryob.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gyzkcijk.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3xeypmlvk.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3mfkurgwy.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3trtciypw.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3sxcvujjx.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3rppnslgc.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3ogujinam.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cdtguckh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jtuursdn.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkicywfk.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3gosnxzzv.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3hlcoezcf.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oylgrmhl.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3flceioyp.html


<!-- 参考信息 -->