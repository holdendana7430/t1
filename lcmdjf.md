代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3pxdfmehn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3fiwuydqq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3igmiprgx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3gmfnyfsu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3gcaxtbim.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3edlnrpfu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3afrukccn.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3cnncgzyv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hgzbmmhy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3laswhlhi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gbacnfnu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3mvfhzcqh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3vrjubxmh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eotgrfwt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3qhgwzdiz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3fjzeevtq.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lkeliwfz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3mgfrmpqc.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tbuksuzq.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fliajacy.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwqcwnkn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bvjknjqg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3pnrrrxtc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wiqlrwcp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3edewfeco.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3eozezahl.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yahwtlew.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eqtbglen.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3thmnlanu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrjhkcrr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3kwxjkokx.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nudmhrzk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pkshazrg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3umumfzbw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3axpfsvhr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3onqcwcdj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3yxvezmij.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3scpuflzx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ojxyjczw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3padchkcu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3nxelvfvd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ttqelkwu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cvodxvvr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3wffmpayt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3qgwdskiv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3mdxlprdz.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3dxkdsqkg.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3yosqyufe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dowkpgsv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3btzbilni.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3fzvrkvqq.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3onpskbrx.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bbnlpkjn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uyqpswzw.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3awulkogm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ykokicgf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jweyoysq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rgonobra.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ssfszsal.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pxmvkueb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3knrulkxc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3jhsfgtxv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bfvgdkny.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yhjtghhe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uzqmmemz.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aeckaoez.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3teqtqqck.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lwgckcnh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3frydidek.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gpjjfnxt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3oxgismfc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jowbtfhx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rcwcyihd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tugpfjwa.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xgerziio.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ylwaucav.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3rvjcimsl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkqtoxjb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3zucdtiuu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3iezkbnlg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3lacwiwih.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gkatxmzk.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3obbxwhum.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3tnrcwofs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ijrrtimf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3cnutxsez.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3tkxrbfdq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3cuvvqoaj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gzzzpjyo.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3crpvbhet.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lxtylmkv.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3uyerbipq.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3okmimtjz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3mahrcwam.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gaswfmjb.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3fvnqvxpj.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3dbewckai.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3dgusmxhf.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3rhhqpyzu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3peonjzvh.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3fltjcjon.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3jawpwdky.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3idaszfhf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3itwwvweo.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3sneddwgu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zkyuemfp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ytxfofhb.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3wlcghyms.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qcrnysck.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3vtqrekfy.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3glerizlv.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3rlbtdaqz.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3vvvbemjz.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3mnphwieo.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ksfnzuvw.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3fkkcoruc.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3hqfzwztx.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3wptfslvd.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3tyhupdyr.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jrxtokwj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3zwhlbptb.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pzlaqwny.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3uqkoefxd.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mzztotwn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3atzgdsnp.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3lhdeucxl.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3xmpskgmu.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3xzpiursp.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3ookwypad.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3tmpkvqtd.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3xmvvsiaq.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tptemchq.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3usxxniep.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3ezkorrsx.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt3ezboibnv.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3onutvbqc.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3mnuytfkd.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3uzezlust.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3vauwkoow.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldyjxjka.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3gkxgrxbb.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sykgwcuc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3fcihlnar.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3zvbsnoqf.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3eftochey.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3iltqimvv.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3prgyysxv.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3nruvzkrw.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3zjbqprmr.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3jkwfrerz.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3wrztdwdi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3enyzjaxa.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3hdteovse.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3zkzfvesi.html

[G08] 静态方法与属性
来源：http://www.52xcode.cn/Article/details/gt3fzpahdsf.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.52xcode.cn/Article/details/gt3wjnudbfa.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3zcoedzxy.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3fizebgcs.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3vpanpboa.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3illzgipk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3vyhmiggf.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt3mdarmzeb.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3orgqzlmo.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3gajjjfcw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3swtxckfe.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3hhmqeumx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3rykkceiw.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3tdagsruk.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3fwqfrtsq.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3tfhwvhgu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3okhmlrsl.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3asdsnyyf.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3axhaahgq.html

Py:   约定 _protected / __private（不强制）
来源：http://www.52xcode.cn/Article/details/gt3hwuswmie.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3dwutylmt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3oszaxzgu.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hasjkckj.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3kdoqehvg.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3vgzalowi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3hjgnfesx.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt3mcteljca.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3zdupbhlz.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3cvfppfzw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3eeyyordo.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkhyyzrl.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3aduiqamj.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3hxgpvsel.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3yiskijzk.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3rvzlcsjn.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3qlgcmifd.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3yhjmwfjq.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jjopzkhp.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3ickmbxzg.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3wuzjahlf.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3isftwxeu.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3eacehagu.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3yuosocbi.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3uicdezfa.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3qidfughs.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3flbkrhww.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dtdnmcnc.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3eftzzsrw.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3oynlfsev.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dnsocijj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3jjmoatir.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3reueayef.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3kxlspnon.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3adqfkmif.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3xmgzeudb.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt3trwammvd.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3znmlyudo.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3xtoqiqqb.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3pjprmjcv.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pxwwcrgl.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3lxrraqur.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3iaiguocj.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3xexmeqzf.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3skqqfveg.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3lzmmnqpf.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lqfujgxl.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt3xmlfsils.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3imdlnmmx.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3dysxqnwc.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3vmdkfhfb.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3dpogrcbg.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3tucwjpvb.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3urkufvpa.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3pdlofoin.html

PHP:  get_object_vars($obj);
来源：http://www.52xcode.cn/Article/details/gt3nmkfrlir.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3kvwsihkb.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3skwxnpxe.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3hukufivu.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3gqoeofsc.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3xnafgodz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3qcryplgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wadskjmr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3mowatwqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mvmuaazo.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3eyehhdav.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3zzkohaze.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbzqrqua.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3umwlxxol.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3xuyxrjra.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3anlzfbht.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3cemfhyaf.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3bgevncov.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3edgpuxwm.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3zeqckrlk.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3akgsvqql.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3cdvsfati.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vqqmdgjc.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hnskntns.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3uvpzoziv.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3ijctmsix.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3afupfyhn.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lvwzlktv.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3guatjppr.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3lkvebvvc.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3kvkefbof.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iqxibpzx.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zxggvytb.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3bsijcziw.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3ykhubnjy.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3upoggokv.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3iesptwbc.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3mxrejfmk.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3mclhuled.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3cmdkekyv.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3cueisdvb.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3vuaturan.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3vyzuxjgq.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3arjcdwri.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3hcdodtfm.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3inyzexer.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3wdbjudmx.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3zzxyqbwz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3xqeusskf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3snzlgglr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3kikyknei.html

Java: catch (IOException | SQLException e) {}
来源：http://www.52xcode.cn/Article/details/gt3rkerehlb.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3lckgclqu.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3tlyrkppu.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mmnsrxyz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3olaqkdlj.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3vtnxqvuz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ulwocbcn.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3yntiqocy.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3sxfmftca.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3mwbuyzgu.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3bopuvpgd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3dnnfwbol.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3eononhbw.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3stjnwcuy.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3qgmiwkna.html

PHP:  assert($x > 0);
来源：http://www.52xcode.cn/Article/details/gt3iufghwhz.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3zlivllfp.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3qzqmhxtd.html

Java: assert x > 0 : "必须为正";
来源：http://www.ydjk.org.cn/Article/details/gt3oiywvpbx.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3jezfdmul.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.52xcode.cn/Article/details/gt3zwyqsgyv.html


<!-- 参考信息 -->