代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzqoydjs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3miaikntd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fopeyzyq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3byvtpuwv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3lhgclpxg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3witqscqe.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3iyniflte.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3owclnojh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3itzacksn.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mzhpvkma.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3lwelhmtx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mkuhrvld.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3uuiheroj.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3crnhohhu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jatciear.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3jaznnidt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ukosxgbl.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3gkzvwhnz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3beihacps.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3nsurzbnk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3iwlbygwr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hywzvtkn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3xumklter.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3eyykclnh.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rlbynfpj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3gdesczns.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fufhwkiy.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kjkkyaxl.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hcdxkfxo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qexppbqh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3uickxtqd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3riumcvvi.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3iunumgco.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3lyntrwly.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtejnext.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xwfswpuc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wwwdvmmi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jqaxergp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ppduwaef.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lvuxboom.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jumkfxfz.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ydqnhdvu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3bxfjrcwy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ivteflzj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3pxohiyxe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3hkuefdzj.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3nkhlzvyf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lrcbaixn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ndmczqih.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3ggrqjsai.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cmpovvea.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3nfkqylxz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3iesrwzgx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3gqekqnsy.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3lxxpkahc.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rvucdqfe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3uofmcbrg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3favcdoml.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3adcqdrdc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3lozmafce.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3rbirqygn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lvnkltso.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rhoznicc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vhpcbzjd.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3znzuvfgw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vdjmqjzf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3irmlodoa.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uoqrpwjz.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3vraazpoz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3dgsqwgzp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hxamgbiw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bjlmqrgb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vytfglej.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wbytdgtw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3avhlfuqt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bciylqid.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cpaddptf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nivtgozs.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3vxebitkx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zrqobxmy.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3meddhfml.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lwcfrrhc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ycrxfhbv.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nmwbdpar.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ledkruhc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qifohfwx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3lzlubvou.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3aiyifivs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3qlgqnlfi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3rimynlcl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vknhnqxr.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3zndtkpxj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3irvvxder.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3aynmcqyt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3lvidyaeo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3wjdtxeek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3elqwnjws.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3priuqcob.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gsmkibjc.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3lpezyhig.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3xfgxkwkd.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwqmsujj.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3myjtnwoy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3carykamv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ccpckqcc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3ujqlohga.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3fiogotvg.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jzxknulk.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3vpgabuvq.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3yqkdkspu.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dpjpajse.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3uxysnxbq.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zhqtdcsm.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3xspmrnvm.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3ngdnqmoq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3szedvjne.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fcqxneqe.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3opknuafs.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3npqqwuew.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3vkmqithe.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kockpnrn.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3myqcmmld.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ajqpaefk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3jctxgbfw.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3dxhxmxrm.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3frlkuiim.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3kwefcmzh.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jycuwnqe.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3risspzxe.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3xtkmsyec.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmuenibh.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3uogpiudv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3xuxjqkcu.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tisyeagr.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3qxmyplli.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3zkhykien.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3isvhejvd.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ewtudxih.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3qisrfsgi.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3skhvcbsz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3yvaxwkyw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.52xcode.cn/Article/details/gt3fppgkhyz.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3omhlddhn.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3gojiyrhi.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3hmxikpkx.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3ituquqob.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3mlvdbgjg.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3kxlrpvfa.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vosebyoy.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofaieilp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3vibinicq.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3gtnlwvsz.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3koyjfspx.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3shtsziqs.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3tbnpzqju.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3wvxlgxnd.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3yazljtpp.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3mfqdftjh.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3zmlkoguc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3kotwqdxr.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3pqkidxjj.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3ecahxmne.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3lynikyfj.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3sfgzzfvl.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3sewbtgdz.html

JS:   static f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3havazxzl.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3faqaqzmy.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qkwcdwog.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3sbqmwiwi.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3zstiswwd.html

C#:   public static void F() {}
来源：http://www.52xcode.cn/Article/details/gt3cbjmrmtm.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3kguajpnd.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3vnwgprku.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3mtqrfjgv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3bgodujvw.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3uyrvtnls.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbkaltfk.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3tzhohono.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3mbmzsgzw.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3wcbjxhsg.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3vvtfoylx.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3yqfxcxdc.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3syzehknt.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3gmoldpdj.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3eoxucccn.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3iaolcvrw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3iykpfawx.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3htgszdar.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3bvbdgvbb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3ducjbgrc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3rtsatqpw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3jkwooyxo.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3sczdlrkf.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3nqirlbvj.html

Java: public String getName() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbrrozzc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3gksirwuh.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3ihwdijrw.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3jjzidwaw.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ovmwzftf.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3ewiprqse.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3jckmgnqm.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cwfuasqz.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pazoewvb.html

Java: @Override public String toString() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cmfmsaaa.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3symgtwlu.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3zgohflev.html

C#:   public override string ToString() => Name;
来源：http://www.52xcode.cn/Article/details/gt3jzfqpqqt.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3aaesojql.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3zqmibuck.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pfvpmeux.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3dkjxaviw.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3dlgiixlp.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3iphoqgca.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3wikdshkq.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3kgvqnaao.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3xxosbxyo.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3ioxzmiax.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3xpobvhdb.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ahdehcpi.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3tzoslyzh.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3bbjitzac.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3feaciwfw.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3mxdexnix.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3rpwvluns.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3pufbqjjd.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3wruwpgns.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3xzhpjasx.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.52xcode.cn/Article/details/gt3nihfibws.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3lpgiyios.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3iouflnxc.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3lmdomnhz.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3arivtpjp.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3fagisfqf.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gotlrwwx.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3sewavtyl.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.ydjk.org.cn/Article/details/gt3cnzracwb.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3zpaejruw.html

JS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pbtbeadd.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ejkkscuq.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3wqzxyesd.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3vkbiwrvk.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3ibufhujd.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ojthfoqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jjqkxjwg.html

H. 异常与错误处理
来源：http://www.52xcode.cn/Article/details/gt3emdxkkqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qklzxacf.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3qkqpdlue.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3jpcyuthz.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3duedxnvw.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3sfcjrmhl.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3tfgppqnu.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.52xcode.cn/Article/details/gt3nqvdlqkj.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3cisoflya.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3nlcdwnuu.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.ydjk.org.cn/Article/details/gt3vptzlhmv.html

[H02] finally / ensure 收尾
来源：http://www.52xcode.cn/Article/details/gt3qqrwyspx.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.52xcode.cn/Article/details/gt3kurqlirt.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hujhjfxu.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3husiqvzg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3qdlvbbcg.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3bffoggfr.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3hgsztzqp.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3tntxkven.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tjupbtaa.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3wegfsqql.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3hggakxmx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3krcdyksq.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zklmwcpx.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3qslqdfpv.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3mnglvgtt.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3jvgavvgt.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3qoxeupae.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3eocjjzrw.html

[H04] 自定义异常类型
来源：http://www.52xcode.cn/Article/details/gt3rizjyami.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3fadxjxic.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpgwjgqm.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3fnqdsonl.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxdxqlsn.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3uirnheie.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3smrjnpyu.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3pczdodeq.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3ahrxvbpl.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3cltunapw.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3nixrbvik.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3ypknfkdf.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3khfptztr.html

TS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3ofwsujta.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3efkmnjfe.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.ydjk.org.cn/Article/details/gt3dmcfepsf.html

Ruby: rescue ArgumentError => e
来源：http://www.52xcode.cn/Article/details/gt3dfyaurir.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3xxtgrozi.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3nkaxesel.html

Py:   value = d.get("k") or default
来源：http://www.52xcode.cn/Article/details/gt3eajgoxgz.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3gliqzrse.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3rpzfbsie.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3gnuylvhl.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3ujfntbfq.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.52xcode.cn/Article/details/gt3hewkljgd.html

Ruby: d&.dig(:a, :b)
来源：http://www.ydjk.org.cn/Article/details/gt3cnokwzby.html

C#:   obj?.A?.B ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3lgurqnks.html


<!-- 参考信息 -->