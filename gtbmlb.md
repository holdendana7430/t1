代发 wailian999

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xpevdfnx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3nvqvybdl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3szkdvsfh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3excatxms.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3uquvawcr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yoprbsxc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3tznmmmqy.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3bibdhzry.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vyszwaaq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3nuvcriqn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3otofygoq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3figregyx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3otxjbmtm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qsvxlddx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3ujaanxym.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3dafiobrg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3notnvzjo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3lxeaenvw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pikzmfqc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbtnoefn.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zblmesar.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jrwdyiom.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lecegcoi.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fanvunyq.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zjzkhqzu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vscvlrmu.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tldvpopk.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oqkwayom.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dtfduzsp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qzpttumk.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3dzlxpbij.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xnwumprq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3spzwxsfm.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rthvgrgk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3hdxwmpfx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3ebrjqtfh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3vbfhacnr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cfxuwkme.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pztqvwps.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3jxdhbvgw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3skxpwrku.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3btybbwdj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3jelodtqt.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3lfazdzbh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3phttseae.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3raagyxgb.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rkpadwdl.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mnhsariv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vppbpinf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3cugwwcsy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xblnkyeg.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3gadgzcdr.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3gadqocsh.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kadonbtg.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zhfowgvi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3lzqxemdp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3pvkytczz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3inyrfphh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3sjbgvted.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ndjjakem.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3iqedsglz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3izokblqx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3orovngwb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3swvvgdaq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nqotatkl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3twapgjdf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3vdgskcfg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jswylker.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qktavyiu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dzigvrlv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qrifondf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vhuugmop.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tinpfmww.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3pszuwzmy.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lyhozsxn.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yhnmqkts.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3wgqmrwxi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hqjsatmc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3uhauylro.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3ftaxikzv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3rwleqvzk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vfkflkff.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3fshdwfwe.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ohdyvxwr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3rnnzltos.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3hdihwhgu.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3hidpnavs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3gqqgacnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rwxmywxe.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3iahmptje.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tysrwuhi.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3fxalambh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ikxpukpg.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qlhxdwml.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uybsjqzx.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3emjvgtsw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3uewiiiwg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3xyndsaep.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3hneltogc.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcsxgmtj.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3wvmahpif.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3lnhwkrvk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oliorgdv.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3tlngnjyw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rwxezfnc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lracocki.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3wbdktpcn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ugguebbu.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3qsqprhil.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3ppbajuny.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3uhhmtxli.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3pexeiwoa.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3nfjvcakh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3lgfdxllf.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3ozdubiqk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3utamfejz.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3fejfisdi.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3wfeevqte.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt3jlsflprn.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3gaavhczh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3corhhdok.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3atybjmev.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3urzgjxqn.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mzgtukde.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ldneiyam.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3sbzxwnou.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3cwduwury.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3ofveeefr.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3tuizbrcx.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cveouuqy.html

JS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3ffbziswm.html

TS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xyjvqiuu.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xkjlhdfm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3thgwzcjv.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3kfbgstmf.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3pfidqjcg.html

[G06] 重写方法
来源：http://www.52xcode.cn/Article/details/gt3hcvxigbu.html

Py:   def greet(self): return "admin"
来源：http://www.52xcode.cn/Article/details/gt3pitggohd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rnnastyb.html

JS:   greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jrljryvd.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3jpztqmik.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3mznizlrc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3aapphqja.html

Ruby: def greet; "admin"; end
来源：http://www.52xcode.cn/Article/details/gt3dybxigfc.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3rnxizvip.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3ilsmwreu.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3nbsitvpw.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3zxgqvciv.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3setvjjnv.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3suqgwswl.html

Java: super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3urcbhqab.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.ydjk.org.cn/Article/details/gt3grhhttia.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3eivjuoyd.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3jmlaxfiz.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3twkhgajk.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3pesfeczm.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3zyipbrsq.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3qijksegz.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3isksamtq.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3xzmiikdc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.ydjk.org.cn/Article/details/gt3kfojuhtc.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3mibocrmr.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgabwfnl.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3yhzqeade.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3uofmbxqa.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3camydfxo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3nvfgxlqe.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3zwipywrb.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qionfaqd.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3gerbmlav.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.ydjk.org.cn/Article/details/gt3rrklqiie.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3katltbbh.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3urxqwkvb.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3spuftpjj.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3ffaaxfzz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3orzlthja.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3micfyimg.html

Java: public / protected / private / 默认包级
来源：http://www.ydjk.org.cn/Article/details/gt3dzwxzmvt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3qhcbmtfi.html

Ruby: public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3pxcxohle.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3btytancb.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3soldrqyf.html

Py:   @property 与 @x.setter
来源：http://www.ydjk.org.cn/Article/details/gt3dvafegwq.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3hxppuaic.html

JS:   get name() { return this._name; }
来源：http://www.52xcode.cn/Article/details/gt3nzxpncgq.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3dfndlnho.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3desjrjwr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3dlhaygek.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3qybtinnx.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3evuyscrl.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3xkuosber.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3asymmkkc.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjjbxmnn.html

JS:   toString() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3zunkbzia.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3buyltddc.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3mgulerzf.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3tkytvxvz.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3jvmvmezc.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3kffobfdq.html

[G13] 判断对象类型
来源：http://www.52xcode.cn/Article/details/gt3monctbve.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3kvnjooph.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rewjoqfr.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3eqizsrxn.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3pcwewihi.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3rwaglnje.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.52xcode.cn/Article/details/gt3xzpqposx.html

Ruby: u.is_a?(User)
来源：http://www.52xcode.cn/Article/details/gt3hsigfscb.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3yecoyohz.html

[G14] 数据类 / record
来源：http://www.ydjk.org.cn/Article/details/gt3dpinzhiw.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3gxxmmjks.html

PHP:  // 用 readonly 属性模拟
来源：http://www.52xcode.cn/Article/details/gt3qyvpbngm.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3pnlglehx.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3oonyqhzz.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3rfohimfd.html

Go:   type User struct { Name string; Age int }
来源：http://www.52xcode.cn/Article/details/gt3xzqnzzgp.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.ydjk.org.cn/Article/details/gt3jqraeund.html

C#:   record User(string Name, int Age);
来源：http://www.ydjk.org.cn/Article/details/gt3pvwuqhak.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uuynlouu.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3wyphyjbp.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ysndafqn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3wuhtbscu.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3ppzdljvv.html

Java: enum Color { RED, GREEN }
来源：http://www.52xcode.cn/Article/details/gt3moynzslp.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3snefzfkb.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3qdpqxgqy.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3lpkntndz.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3hatkyykh.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3apbnzwwh.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3ovhjlzhd.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jwetydys.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3vumyozlx.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3ncygfbue.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.52xcode.cn/Article/details/gt3ixktfqaq.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3osyurvgi.html

C#:   // 用反射或 System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3svsygvhy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcsaltvn.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wpsderoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xdbqzofb.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3axwlgyhx.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3hijuzflg.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qaszonyg.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3fldycgsv.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3ojdhvahb.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3oohffkoo.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3otamkgbu.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3jjjwtxbt.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3radmldjs.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3wmphnysi.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3hcrialon.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3gbyuhusb.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3xejrpjkg.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3skazcbec.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ncwvhjfo.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.52xcode.cn/Article/details/gt3yfjmtwnd.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.52xcode.cn/Article/details/gt3whxzhpzc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3nrckzqzi.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3zwjmhakd.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3kwomaumu.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3tbkckgmt.html

JS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3ppuxehgl.html

TS:   throw new Error("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3pmtqszum.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3rmrkrqfb.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.52xcode.cn/Article/details/gt3drtnjacs.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.52xcode.cn/Article/details/gt3hnvtazlo.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3xmsabpxp.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3fkcmjvff.html

Py:   class MyError(Exception): pass
来源：http://www.52xcode.cn/Article/details/gt3zcvjiyks.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3smipuijz.html

JS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3xhlyckke.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcjzjtkr.html

Java: class MyException extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlklzrbx.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3qudcmfcy.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3cvzgugmm.html

C#:   class MyException : Exception {}
来源：http://www.52xcode.cn/Article/details/gt3kwqhrimc.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3tanqhmux.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3ljsftawz.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3yafnnliu.html

JS:   if (e instanceof TypeError) {}
来源：http://www.52xcode.cn/Article/details/gt3dwjijieh.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3suduchnq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ervkancw.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3nmxxhihw.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3paihczdl.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fplsexfz.html

[H06] 可选值 / 空值安全访问
来源：http://www.52xcode.cn/Article/details/gt3orocgzjt.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3kerwkldf.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lfvutmyd.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3anucqcvk.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3bezjupuk.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.52xcode.cn/Article/details/gt3qvslcexs.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3jeqdmkzs.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3mxztfrdg.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3naaocird.html

[H07] 断言
来源：http://www.ydjk.org.cn/Article/details/gt3ocqenymi.html

Py:   assert x > 0, "必须为正"
来源：http://www.52xcode.cn/Article/details/gt3rplbtdfs.html

PHP:  assert($x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3revlpkfl.html

JS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ptemytvr.html

TS:   console.assert(x > 0);
来源：http://www.ydjk.org.cn/Article/details/gt3kmwyhawk.html

Java: assert x > 0 : "必须为正";
来源：http://www.52xcode.cn/Article/details/gt3egtbmkgd.html

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://www.52xcode.cn/Article/details/gt3vbkilrlv.html

Ruby: raise "必须为正" unless x > 0
来源：http://www.ydjk.org.cn/Article/details/gt3gkhkzdwa.html


<!-- 参考信息 -->