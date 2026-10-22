代发 wailian999

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2pgplfepj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gxgjkvbh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2oaudusge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkvqipmt.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2oyeexfwg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2bwmvwmrg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2komvxenx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ngbkjwez.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ovmtgrzz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2aeyfmjaq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2zplzondl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tatpdfbr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zszrhipu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2twikuowh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2gjfuaccm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lgtthhpw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2qvgihkve.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lxffibix.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cxtevcos.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2mzscbkea.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2mcplbhek.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2hekrzcjc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tqxefuoz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2agmswbqj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ucfyjdyh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cbrhfybd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2lphpkwuh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ynuzsyhe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ztqkyzgd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nnicizpg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2mgloexpx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vzpvilja.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wjwruasn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2yxjgvlyp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2esuxpzwf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2bkjdgdqq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ctezhbav.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ewfbddch.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2lxirixfk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2euvnidgy.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wubzmugu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2xhqsmkep.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vqhencfl.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2stmekxvf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uzfztmii.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2devxtdoe.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2wgcwqtto.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ehyujrai.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tlyytnev.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2lrrhtnuo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2izdumlgu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2asiructw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bybtfmfe.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2exolojka.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2skqqfrfg.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2taidtnwb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cakdtnsc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bvmnutor.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2bhylkrdp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2jhhsvijg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2kewhmjvl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vetadyex.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gkpmbkvz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2ypyvbzlw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2xzdgnidy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2meofdfck.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2cpeykbub.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2ftkcicsg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2edglhdey.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2loooieii.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tudlahrk.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rzgafnvh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nzsqizzu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2dpmoahto.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ojalljll.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rdaujcpm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2tqjbehuj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ndxunfnq.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hrwmryxe.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zctmfixl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ltdcdoff.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eltsjohp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2rshlirde.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2paltmzeg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2pclwkjsf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2gcoxaxsn.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2neechhpx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rjfhkqsk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofjdrcdo.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2euukhhaw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2dsyfsasz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dpuecvvh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dgdhrtly.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wpkaeitt.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2jenlnbft.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hqwypvke.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2etaczszr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pbesjmwc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vfhlsvni.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vexxeedd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2curwiodc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2akfkxtwo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ifecqjes.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2wytoitxw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2azqdothk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2hzhdxchv.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2qwpsgnrb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ktxnvxuj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2cytemkkt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2bmjxjcvu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2wgfksndy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2wioypqcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gkkjozih.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2oxavaugk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nmamaxap.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2haaugavm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2pjtmfyeg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zfpnqaax.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2tuutosba.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2fulqzvgs.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zoksuoga.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ybtjhdkt.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2dckxkoee.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2vclztkeo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xwixcyfk.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2nljhjzav.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2nqnskaxg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkbnbioa.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2wvqxjymc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hzkpeftc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2wewltzwa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2cvyfvfvy.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2eujubmkt.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2elsbcttf.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2xrboglls.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2wamhtpwu.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2sjfckhny.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2zymgzgpk.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2vdlyjhef.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2enqgmwie.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2rugulsfu.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2jbgofkcy.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2emdlhifd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2kvqrxfgi.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbwicqqs.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2axguhigp.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dngctvlw.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2kqlndyxu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt2spvhaefs.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2fpgompzp.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2jqnivkgs.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2kzdhpqis.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt2jblacvjc.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2yxujwxhi.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2snzjnvfh.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ackjjliy.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2reinzmsh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt2xpmjsidu.html

Ruby: class Admin < User; end
来源：http://www.ydjk.org.cn/Article/details/gt2napolwwg.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt2fddfnnoq.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt2uwywkoap.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt2sizgboem.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2dfvpxgrz.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt2trbqnjar.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2xwuhoogv.html

Java: @Override String greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt2wrcumubn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt2vbbhiuqv.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt2vbhgjffe.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt2eotvfrli.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt2gryxrulq.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt2lrwjbvvk.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt2nxrmcqai.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2oueqgibf.html

TS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt2gpszofmx.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt2goflregk.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt2qxlobjbx.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt2sjzffccf.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt2onrfsxaw.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt2lhsnomku.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt2skiafeyg.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt2xykqxney.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt2hxhuzqhc.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt2goeuxlij.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt2mnekjawz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt2uoewptvx.html

Ruby: def self.f; end
来源：http://www.52xcode.cn/Article/details/gt2fhfqfpit.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt2lykdmudt.html

[G09] 接口 / 抽象类
来源：http://www.52xcode.cn/Article/details/gt2cmkglryf.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt2vbbwtbow.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt2ohvdylpx.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt2ogflzdhn.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt2zysysiqm.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dplytmld.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt2qpxuierb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt2jyfazyfh.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kucbfiwv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt2botpgnol.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt2jrpgxybj.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2dqdodhke.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt2xosgzjjg.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2eecjxyzt.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt2zhwokosp.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt2xdpcifrs.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt2brrxawrg.html

C#:   public / protected / private / internal
来源：http://www.ydjk.org.cn/Article/details/gt2nrzcjvcc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt2fhhmeqil.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt2yuzudfjl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2kcecdems.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2vkxpegcm.html

TS:   get name(): string { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt2ymeatemt.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2ivrekrhc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2qtngtnns.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt2ggdykuzq.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt2gyakezxi.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nndpylww.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2rezjqnem.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkbjcbeo.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xzbsewbh.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ymkqvibv.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2lpekftci.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2rekrjtsn.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt2voouhewg.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt2fjthkidu.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt2cwtqrwud.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt2lisoemlv.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt2cbnfwljd.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2gidpcera.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2hgnawbms.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt2ffvkhljr.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt2cngmxwti.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt2svqbuxvl.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt2psbpfcqe.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt2nawkuxrw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.ydjk.org.cn/Article/details/gt2abrarqvb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt2ttclczxe.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt2nrnliozh.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt2pbhpebnn.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt2clteieen.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt2cazvcozu.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt2bgdzfxsz.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt2imdnbpvf.html

[G15] 枚举
来源：http://www.52xcode.cn/Article/details/gt2gwqkpvgj.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt2vkvnmlef.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt2chvcnppk.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.52xcode.cn/Article/details/gt2fpvvhvho.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2eslpertz.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt2hzcxrqtg.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt2rfsfgyvr.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt2wslzeipu.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt2astliizp.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt2ymcerwge.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt2gawgnmom.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt2feyqpbzi.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ifqtvzkw.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt2ojocijho.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt2ssbfxqza.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt2tbnjezel.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt2hlnzkziz.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2liwerojd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2edkxyssf.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt2jmllrlkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gzumvcpy.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt2scqzsgcx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt2lzohqadm.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt2vxbrlcfb.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt2xidgdzsk.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt2dcpxeyrv.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt2zuzkxude.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt2evwqikas.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt2qotqmhnb.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt2hhwpvsao.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt2elucdhqu.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt2mrjtmili.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2xsqinaoy.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sieeifup.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2kugrogiw.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2wqnaghmd.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt2vwkdekza.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt2cynwmiqa.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt2ufcojvzy.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt2igjpptcy.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt2rymstuhz.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2izsfwgvb.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2bmqwefjn.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2lopojtqg.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt2ujjofaes.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt2jiztjtxm.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt2hjsddihq.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt2dhndgeev.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt2bwjgsjza.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt2nchzdrrm.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2pgpyisjj.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2amoyiwrl.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt2hnkyjfdb.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt2lwzlejrr.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt2bqppwoui.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt2mcqkchma.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt2qbxjigdk.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt2cwtkfohs.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt2ciphixov.html


<!-- 参考信息 -->