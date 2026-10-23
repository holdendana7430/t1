代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zeivyard.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nemuzkgk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ykpazgrl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3zyvwihpk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3kyemiido.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3icpidyeg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xowiflph.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3fqzxdayx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bsozntlh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fhlqpzou.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nlpizald.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pwqjfslx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gamttrtr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3leomdbgw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kvgavgpj.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3qefjobug.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3wjfldzus.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3fzpikxdm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3kawamsen.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3owkdmols.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3psypanmf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3ipxhzcjv.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3uuahbznt.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3jytntqni.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qugvjsjv.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3iqmzorpu.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oaqtlirp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zhhtiqhc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3csrtlwkq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fydznehh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3obtngkel.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3clfllmfg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zkunkdme.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ooginuos.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eppayouq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3veiogogs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dhzeaftr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kddadibx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pnribubc.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jjsmmzvb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mlfefgwa.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ekqjdbwy.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3dwqlukdc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qwixupny.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3bdhirrhi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nhjhiulk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cwjitsat.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3vclzbtqt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ewuhbzwe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3qwlbdtsw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3dhvianpt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vdwyelbb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3klkwlgtn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3zsdgenui.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3vqqpwoah.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wnuizkbv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fjevxvow.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3frocvpfp.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3htxzcvib.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zsggfyxp.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wouyrvix.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cswgyrgf.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ttrwulqh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zrpaeanl.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yswmyvvn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jwswzvwm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3orkhwvee.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ycqbqyhf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3naddufby.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3cwwydnbr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zujfiaff.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3fjdwvwhs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wvejbrlt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qvzxttdy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3jtpyhqjb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ifseiseg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vlahpzmj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mjhwmenn.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3csbnsmfs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zriupmhl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aftgcuac.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wzvjxzox.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwvruswl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qexkwfiq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3rytudern.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dqlpuyoz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3icrmwyci.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3srelkrny.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3rongcfcl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3uztvmojn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3ptiwbtsu.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3sxpnmolw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ggtetpzz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3sahhejjx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3plwbceeo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3gnmddhvk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojozsffj.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3nnpahunu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqrhtdwy.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3qeasvqvr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3nqbzjybm.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3msoyadua.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uewftypx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3aawzhbzl.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3fbopdnbl.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3rkcbyihw.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ouguodng.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3eiptafbc.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vlcdmdmg.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3hsoecjli.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzqvjniv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wfzevaxz.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3hqxgjath.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3eendpmck.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3zqwnzreg.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3nngeqamk.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3hjmzujxv.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3dnbqhxrw.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3imipozjp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3bqnczats.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ymczbxdb.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3tylpvslu.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ndmatkyd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3oqgshjhi.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3uszqnhyb.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3chfacmhz.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ingizjkj.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3dmfflpio.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3sqvioxcb.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3rbspvbsy.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zspguswz.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3aekxtuab.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3waevabpk.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3nwzzlvhn.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3zwvzuvbm.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3iemuqakn.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3auqwries.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3fqkaawqj.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3soitsboi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tbxmubve.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3teafonzs.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3nyxcjqrt.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3oeghzaqs.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgblpvxr.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3gdybnbzp.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3tynujqbr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3aexugaso.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3qovecskn.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncgskdai.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3yfhtmazv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3cktwocjv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3pglfadgu.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3gxeyukbo.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3frizkdqg.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3ezatbkxf.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3bejkrozu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3xatoipae.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mbuxatyk.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wrejhnsj.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3hmcpvdkd.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3ihivgarl.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3njtqbela.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3skwvxkjw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3bcepbfwc.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3hrvywutm.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3pwahzgsf.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3zvdnogmp.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddvyrbhw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3vzduvevj.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3zttgctkg.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3jrlfuelt.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3jvvslyfo.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3zgqhtvrz.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3aokaiwqn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ptcgktlf.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3wmhnodot.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3weagscrg.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3jnlefjgh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3gdycpixq.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3dsevgzol.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3tnpfiuos.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3hfpggvog.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3msiqefqf.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ikflacub.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3wqxvvili.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3udokbibz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3vzudqrka.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3brjufwep.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3igckfspe.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3ofmzykyz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3jgdoyevo.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgdtjcxe.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3hkhiiidp.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3cusshoci.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xunjnznq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3fzrcfuzk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3glxzgnom.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3ycinabgd.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mpakcuhp.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3fqxfsbiz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zayszavi.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cvnhlvpi.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hrlxafdu.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3knsdrxdu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gweeieeh.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3cmwwtzdj.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3mrfxeita.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3qjatqupx.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3gnkibdis.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3kocypoyl.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3bterosan.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3upknvoen.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3ocbzaywc.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3ahnishus.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3udbqwlgb.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3xtstwbtg.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3uvgdvxzs.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3qmqjmkrh.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3dgflcgol.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3ibqmgatn.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3adqxufqn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3cgnfkcek.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3wlqxywjl.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3iiknnsjf.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3ilvlggvs.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt3pfibnavm.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3jxgxkfyd.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bgzkgxfl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3vbgcbdpz.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3guxqlspb.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3sjzjqfgs.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3qjjebuch.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3lkgbzglq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ugsxuzae.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3pgerplnz.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3entcioyk.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3moabvzad.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3sflgqeqy.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3skmybrzy.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3jgchhyvj.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3pppvwasa.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3egvmmtbu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3uvcfdjbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lktjcecd.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3hktldzzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3revywcse.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3bjuylrdd.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3edpspxqn.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3vgjbxjtk.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3wrpwjlxe.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3brkcqori.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3hifqjcoz.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3dwcbxxhi.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3ijwwnanz.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3thxikpyw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3fexfgljk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3hhohbxkk.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3mfoqvkzv.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3lxkvhzeq.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wzfsspuv.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gmmapimb.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3vifigoxp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3fjqiqwhu.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tpniavxh.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3afidxihc.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3ykmglcls.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3lugsmxvv.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3uaulpmcr.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3wdgvxdwt.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ihqhxtef.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3boupjvfp.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3ghlmgbiu.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3ubgyhjyp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3sqtjblmz.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hllqraas.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3lnbetgnl.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwcrbdww.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3uwxcfkur.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3rrdvymed.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3zisptdff.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3lohkgsqd.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3fovelrst.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3qbawksop.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3xdvjrxgs.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ysuuwowl.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vupoqexw.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3vbkiirvj.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aapadfxd.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3luqlclww.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3kgtrmrka.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3acuayveg.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3egenvrbh.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3kggvguae.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3geiqhuhg.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ftxqhylm.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3avhwbhqi.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3gzbfbykw.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3iwygylbw.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3tdozlqau.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3kgefbtqb.html


<!-- 参考信息 -->