代发 wailian999

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3giirbfcr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3blozfyzd.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3txiwmuaj.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3fbelvsln.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3eatpuspr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3bwqredhe.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3xxqmorps.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3rogtmrkc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mcmgphfa.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lavzhnet.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mmbmqkpl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3lbeobrkm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3phydvikp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dckorgxv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jduutifs.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3zpcqormj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jhgzdehv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3dzrjzctg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fwjacgny.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kruathaf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3mfrukrme.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3qsueajnx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3nomdskcd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3uamlshbb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3xcczbtok.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xmaehbcz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vrpwwqzm.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pwyatkag.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tolagtjd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qwgpznge.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3zrymssng.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kelatufe.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhbulyjn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3upjkzooh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hkdvufjd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tqhzgxew.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sdloozpp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3djwkbabb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3plgabkwv.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzfpjvmq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kmmniqcn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lwbyyxng.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3srkkxxgy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dvaragmb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fqvtfjfo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3xccuybiu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qtxifoae.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ndqcqjid.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3yhrfolmj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3gaifuhzn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3bmuwqauo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3wpvueygk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gogklzfl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3alnplhwx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3gfhtbojn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ffzonwum.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3mmfksprb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qfwvhxgi.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dypivfjs.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nviicgtw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3dnlatvtc.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wqumvdiv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ugipjbtd.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3gshthnko.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qyxstvpj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3leqluwyj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3pypfnyxk.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eoxefoeo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3mpmdugmx.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3dbugwoej.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jqgckqwx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ivuttdyj.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3agfuwagm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ovybhysx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3jkvhyjvg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rvbusxas.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yxoacvha.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oxiyiilb.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3dmwbglls.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ckpjwzrh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3iqmfmjos.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tjlezkxd.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uamxymoa.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ibggbcoq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3wvpooplq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qskicgjo.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3miazmdrw.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3cmqzoafd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3sxuihogg.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zjkoynll.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3zggfyhin.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3fvdfipqa.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3ihdkjglc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3ffpsprbl.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ncmfrgkk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ndxkqjkc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ivlozfwg.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3svrnvrwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mehqoztq.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3bcoliwbe.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3tqcomfvz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hsxtjqkw.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3aaukiuvr.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3zvzkmzyp.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3kfbggpmm.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3lqxqeytd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3lponthqd.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ysxfksdw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3rzdcarff.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3xqygwbuq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3covtpaht.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjftvocb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3frgpcccc.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3gubfpllu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3dqttyras.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3qndrsayg.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3wqrnmgja.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zqemwdsp.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3ujdjltob.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3bfslibfs.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3qygfwfti.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt3voyglijc.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3ibriibkk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3hsmqmlkn.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3zsrqhlqg.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3xwxkctbd.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3ufgvwqzc.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3cxslvjze.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lddbiltf.html

JS:   greet() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3xjogrzpw.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3efsomkui.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ydvptgwb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3wyiilvbw.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3bjoozofu.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3ekfzbxrr.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3apnouwkj.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3hrrpvats.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3msmkdzdm.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3succjolu.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3eijrzrpz.html

Java: class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3sirrnqns.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3qieudecp.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3gkxakorl.html

C#:   class Admin : User {}
来源：http://www.ydjk.org.cn/Article/details/gt3qossjpgh.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3nzsfyjqq.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3oarskhqt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3ygehylpr.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3clcqbtbc.html

TS:   greet(): string { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3lhiwstng.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3czcycbjj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3jilxyjdu.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ozaugdxg.html

C#:   public override string Greet() => "admin";
来源：http://www.52xcode.cn/Article/details/gt3zdjpgvav.html

[G07] 调用父类方法
来源：http://www.52xcode.cn/Article/details/gt3qsrmawcn.html

Py:   super().greet()
来源：http://www.ydjk.org.cn/Article/details/gt3cijeiids.html

PHP:  parent::greet();
来源：http://www.ydjk.org.cn/Article/details/gt3stziaopu.html

JS:   super.greet();
来源：http://www.52xcode.cn/Article/details/gt3myqxhpje.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3tfvztpll.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3pphuaxed.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3lucussbl.html

Ruby: super
来源：http://www.52xcode.cn/Article/details/gt3qnlcccsj.html

C#:   base.Greet();
来源：http://www.52xcode.cn/Article/details/gt3exfzlbin.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3gagfbeky.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3zpwvqbif.html

PHP:  public static function f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3iszddlcx.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3rjuovwui.html

TS:   static f(): void {}
来源：http://www.ydjk.org.cn/Article/details/gt3ypvsgefs.html

Java: static void f() {}
来源：http://www.ydjk.org.cn/Article/details/gt3foeapkqc.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3fekcuony.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3fybrdjof.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3vptkynqe.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3ibltxqlw.html

Py:   from abc import ABC, abstractmethod
来源：http://www.52xcode.cn/Article/details/gt3sdrfdctk.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.52xcode.cn/Article/details/gt3wezweunn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3ryvcdres.html

TS:   interface Shape { area(): number; }
来源：http://www.52xcode.cn/Article/details/gt3nobuqvhi.html

Java: interface Shape { double area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3cdstklih.html

Go:   type Shape interface { Area() float64 }
来源：http://www.ydjk.org.cn/Article/details/gt3qmhpnhbr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3tgtrwdmx.html

C#:   interface IShape { double Area(); }
来源：http://www.52xcode.cn/Article/details/gt3kmmrutjk.html

[G10] 访问控制
来源：http://www.ydjk.org.cn/Article/details/gt3pnoyjthp.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3qldohglh.html

PHP:  public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3blijsafa.html

JS:   #private 字段；其余公开
来源：http://www.52xcode.cn/Article/details/gt3ktxxuefm.html

TS:   public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3pugqpzdo.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3ikqbjvii.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.52xcode.cn/Article/details/gt3mbbnpial.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3gsoexdry.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3skwxtadw.html

[G11] getter / setter
来源：http://www.ydjk.org.cn/Article/details/gt3vasiqweh.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3msvsssmz.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3gofzkgbk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ctdwrqiy.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vnpmalrg.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3xewmxvue.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3uqppsaos.html

Ruby: attr_accessor :name
来源：http://www.52xcode.cn/Article/details/gt3sicbrqry.html

C#:   public string Name { get; set; }
来源：http://www.52xcode.cn/Article/details/gt3sdapgzhz.html

[G12] 对象转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qmqxdwjh.html

Py:   def __str__(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt3apuiyobe.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3beeynrlh.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3heowojpb.html

TS:   toString(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3pmmlfzlg.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3ubrccwku.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ghjqwnpf.html

Ruby: def to_s; @name; end
来源：http://www.52xcode.cn/Article/details/gt3fyodspip.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3ldnihmkn.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3fkduuxlj.html

Py:   isinstance(u, User)
来源：http://www.ydjk.org.cn/Article/details/gt3dvhsiono.html

PHP:  $u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3lcpyltxg.html

JS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3tjjpktzx.html

TS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3vxiaskqp.html

Java: u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3asnmejep.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3fitremav.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3wgtjxqag.html

C#:   u is User
来源：http://www.ydjk.org.cn/Article/details/gt3gzbqjfno.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3mfoarkcl.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3cjjwvqyo.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3esduxwkl.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.52xcode.cn/Article/details/gt3qdnighcz.html

TS:   type User = { name: string; age: number };
来源：http://www.52xcode.cn/Article/details/gt3lzlakoox.html

Java: record User(String name, int age) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ynhitjdi.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3jwvfjrtr.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3onnojfwn.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3kxkhdqkt.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bdwsrjjy.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.52xcode.cn/Article/details/gt3cwyqeafr.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bkihdepy.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3hzjpxspj.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3vlfjcdbu.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3qvmunkbi.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.ydjk.org.cn/Article/details/gt3uefuyfnu.html

Ruby: Color = %i[red green].freeze
来源：http://www.ydjk.org.cn/Article/details/gt3bqzapguq.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3rzghzqwm.html

[G16] 对象转数组 / 字典
来源：http://www.52xcode.cn/Article/details/gt3ivrktuvd.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3raqmhhim.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3dhirjidf.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3uaoykyth.html

TS:   Object.entries(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zansvqdi.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.52xcode.cn/Article/details/gt3xozolqwm.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3vrunhnhx.html

Ruby: obj.instance_variables
来源：http://www.52xcode.cn/Article/details/gt3qmpbufbu.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ibmibzcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhbcngmb.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3sfstaqic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jhpkdowr.html

[H01] try / catch 基础
来源：http://www.ydjk.org.cn/Article/details/gt3mjiyuoey.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.ydjk.org.cn/Article/details/gt3lzprvdsr.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3rixbxhkz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3admfwfgy.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3orideqmy.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3eunnesom.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.52xcode.cn/Article/details/gt3mieucscr.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.52xcode.cn/Article/details/gt3mwzuvrpg.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3prslgqzw.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3oxcefmkz.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3qipbawdf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzcmcdav.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3exbilkip.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3vpsyjtjp.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3dojljelg.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3tylgssvk.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3uswquygk.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3wlgerbmr.html

[H03] 主动抛出异常
来源：http://www.ydjk.org.cn/Article/details/gt3uiuubulh.html

Py:   raise ValueError("错误信息")
来源：http://www.ydjk.org.cn/Article/details/gt3sjhjknkx.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3mpqsqkba.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3zixjetdo.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3odvpeggl.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3itnhocen.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3cidiygmz.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3ysnuqrow.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.52xcode.cn/Article/details/gt3wosythnn.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3fbcnvteo.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3cdvwnfho.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.ydjk.org.cn/Article/details/gt3ezbdugdh.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3zlregsaf.html

TS:   class MyError extends Error {}
来源：http://www.52xcode.cn/Article/details/gt3gvbvkesu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3colcfxtc.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.52xcode.cn/Article/details/gt3nytbfpgx.html

Ruby: class MyError < StandardError; end
来源：http://www.ydjk.org.cn/Article/details/gt3bziivwci.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3oflqakou.html

[H05] 捕获特定类型
来源：http://www.ydjk.org.cn/Article/details/gt3adcsqnbl.html

Py:   except ValueError as e:
来源：http://www.52xcode.cn/Article/details/gt3puqekans.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.ydjk.org.cn/Article/details/gt3owyaagsq.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3njlizvho.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rkpirzny.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aktxcleu.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3qtpkzfhq.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3okizhjtv.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ftfjtwjl.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3faluikor.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3clzcregk.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xaxcfxqp.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3ekgecvnd.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3knigwaxg.html

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://www.ydjk.org.cn/Article/details/gt3collbays.html

Go:   if v, ok := m["k"]; ok { }
来源：http://www.ydjk.org.cn/Article/details/gt3zgfdauxg.html

Ruby: d&.dig(:a, :b)
来源：http://www.52xcode.cn/Article/details/gt3ptvheliw.html

C#:   obj?.A?.B ?? default
来源：http://www.52xcode.cn/Article/details/gt3rxmlgsth.html


<!-- 参考信息 -->