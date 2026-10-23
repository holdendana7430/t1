代发 wailian999

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3otmrbhhc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3zocmmbld.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3eyksmlwz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3eugxovwp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qcbsnvcu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wqduebvm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3rvhcabkb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ybdqbvjq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3hetjziuq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3mputafqu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3joebdpjy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3cqcadchg.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3vybknpcc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3sqkrsgqv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3smehxbsk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tmdxvvhe.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3bdfgfazg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3yzewrsch.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3uhyctnic.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3eyovoszw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gcmzxrsu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ejlxulth.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jtfynfme.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3axzyubkr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3bfbojjgf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3dcstxccf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ikrowcqd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3wlfcyqem.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qmyfummo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3rxfatyhd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rsiaasso.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3shxubezg.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fbvlpjsb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3obzbvitw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lrxhasdx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bitfpcmp.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lvizcein.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3ebyolcpp.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ieodfgcx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mchwzgst.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bqxfpnfj.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3frzxqycs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kafpsiae.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mczwtogt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oynrzsqo.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kogwuiyl.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3dwqacutw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3yzekcear.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3qmvqsmpa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wuqdmktk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ncrdpxcz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3fgllddwr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3sqclkfle.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3apwnzlzm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3affysqbg.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vpoleaqj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3rezsaiwj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ewtaosbt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xmvjnhsy.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3pefrsqkk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3iclmjges.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ebrranxh.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3nasfkbui.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nocspguh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3hyysdgia.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oglsftre.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hflytiep.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qsrvnahi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ibttowfk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3aybuzpca.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ziotyytt.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3swmggodx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3brjwcvno.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3djtsjuds.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hmknumrl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ylfemxyl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cjznyskk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zwobermr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3rntcjzwt.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xmcqstcl.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hxreorco.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lhmnkljj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3shompmlw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mbwiihgm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3slpcgzzr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3umdomtav.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqggubqj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jbiqpspn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3pcfklcja.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3csutrbsp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3mvcjfmcj.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3jtytfahs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3dhshlwxt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3wbrfyywb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ihmcbfiw.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ryiljksd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3sygnojhp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3dbpaqexp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3xmokpptv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3bednrggf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uflrqoqj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3bhglbpsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tmprkyjo.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ckonkfii.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3tdzmvdjt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3hezsdulj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3xtpqntwx.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3uvphauhq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3yvdxjkqc.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3asgojvxe.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3nejnsepa.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3ymuzhjuq.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3wqwaxpfn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3nbfxcsmg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yjjzwuvg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3mxpxhqyv.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkhyfndh.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3jkakvdje.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3leiaqise.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3crbrpbwh.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3pxdjkxfu.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3zojslemg.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3iqsdlfba.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3jyasvzuv.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sdzkjjph.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pdgnjobh.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3cquhpqgo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3gezmxrks.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt3kvrxujxy.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt3hgruynnt.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3twqcjzyz.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jlvczgpd.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3oedqvuyh.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3cjxpyldd.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3tthaojjh.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldmvvgxu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3ozvknrgn.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3rzcgzbon.html

C#:   public string Greet() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3vkapikju.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt3yzabxzev.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt3zxkodhqs.html

PHP:  class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfxnbpgr.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tridonps.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hxugfuvz.html

Java: class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3uhmompgw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.ydjk.org.cn/Article/details/gt3udlliihe.html

Ruby: class Admin < User; end
来源：http://www.52xcode.cn/Article/details/gt3jwyhqcos.html

C#:   class Admin : User {}
来源：http://www.52xcode.cn/Article/details/gt3ailiiifo.html

[G06] 重写方法
来源：http://www.ydjk.org.cn/Article/details/gt3oljszlzl.html

Py:   def greet(self): return "admin"
来源：http://www.ydjk.org.cn/Article/details/gt3umaioxec.html

PHP:  public function greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3icqwjtrp.html

JS:   greet() { return "admin"; }
来源：http://www.52xcode.cn/Article/details/gt3khokfcyo.html

TS:   greet(): string { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3dyqvactq.html

Java: @Override String greet() { return "admin"; }
来源：http://www.ydjk.org.cn/Article/details/gt3lpwoahhy.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://www.ydjk.org.cn/Article/details/gt3gsbijubh.html

Ruby: def greet; "admin"; end
来源：http://www.ydjk.org.cn/Article/details/gt3ezkozbzt.html

C#:   public override string Greet() => "admin";
来源：http://www.ydjk.org.cn/Article/details/gt3snpzjmqj.html

[G07] 调用父类方法
来源：http://www.ydjk.org.cn/Article/details/gt3yrlwnkjt.html

Py:   super().greet()
来源：http://www.52xcode.cn/Article/details/gt3rtumrofu.html

PHP:  parent::greet();
来源：http://www.52xcode.cn/Article/details/gt3ywrfygje.html

JS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3wpeecnmx.html

TS:   super.greet();
来源：http://www.ydjk.org.cn/Article/details/gt3byxuzhef.html

Java: super.greet();
来源：http://www.52xcode.cn/Article/details/gt3hwstzpyo.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://www.52xcode.cn/Article/details/gt3ovaicrtc.html

Ruby: super
来源：http://www.ydjk.org.cn/Article/details/gt3kshjzfrs.html

C#:   base.Greet();
来源：http://www.ydjk.org.cn/Article/details/gt3edfylytv.html

[G08] 静态方法与属性
来源：http://www.ydjk.org.cn/Article/details/gt3oswgsymc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://www.ydjk.org.cn/Article/details/gt3gcfanmuf.html

PHP:  public static function f() {}
来源：http://www.52xcode.cn/Article/details/gt3omdybhzi.html

JS:   static f() {}
来源：http://www.52xcode.cn/Article/details/gt3steubjam.html

TS:   static f(): void {}
来源：http://www.52xcode.cn/Article/details/gt3modsvgxt.html

Java: static void f() {}
来源：http://www.52xcode.cn/Article/details/gt3nlqamrzn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://www.52xcode.cn/Article/details/gt3xmblmenx.html

Ruby: def self.f; end
来源：http://www.ydjk.org.cn/Article/details/gt3xxqvewiz.html

C#:   public static void F() {}
来源：http://www.ydjk.org.cn/Article/details/gt3bzplipsy.html

[G09] 接口 / 抽象类
来源：http://www.ydjk.org.cn/Article/details/gt3retxzuvj.html

Py:   from abc import ABC, abstractmethod
来源：http://www.ydjk.org.cn/Article/details/gt3myqpthmi.html

PHP:  interface Shape { public function area(): float; }
来源：http://www.ydjk.org.cn/Article/details/gt3ldibtxcg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://www.52xcode.cn/Article/details/gt3jdxiplqq.html

TS:   interface Shape { area(): number; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbacuaqm.html

Java: interface Shape { double area(); }
来源：http://www.52xcode.cn/Article/details/gt3eiwqswdw.html

Go:   type Shape interface { Area() float64 }
来源：http://www.52xcode.cn/Article/details/gt3skmpwrgk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://www.52xcode.cn/Article/details/gt3fadxnrrk.html

C#:   interface IShape { double Area(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lmqnywjv.html

[G10] 访问控制
来源：http://www.52xcode.cn/Article/details/gt3aapwumve.html

Py:   约定 _protected / __private（不强制）
来源：http://www.ydjk.org.cn/Article/details/gt3yqcddqnt.html

PHP:  public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3agecflaz.html

JS:   #private 字段；其余公开
来源：http://www.ydjk.org.cn/Article/details/gt3gvnmiqte.html

TS:   public / protected / private
来源：http://www.ydjk.org.cn/Article/details/gt3fngkmjhe.html

Java: public / protected / private / 默认包级
来源：http://www.52xcode.cn/Article/details/gt3zjfxcuar.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://www.ydjk.org.cn/Article/details/gt3zzmrnpax.html

Ruby: public / protected / private
来源：http://www.52xcode.cn/Article/details/gt3vqjwohxc.html

C#:   public / protected / private / internal
来源：http://www.52xcode.cn/Article/details/gt3tdupuddc.html

[G11] getter / setter
来源：http://www.52xcode.cn/Article/details/gt3mkviytsc.html

Py:   @property 与 @x.setter
来源：http://www.52xcode.cn/Article/details/gt3pjhhzets.html

PHP:  public function getName(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt3pcetpnxk.html

JS:   get name() { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmxrsjul.html

TS:   get name(): string { return this._name; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlfppdwl.html

Java: public String getName() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3tctyqjlm.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://www.52xcode.cn/Article/details/gt3oanlurwu.html

Ruby: attr_accessor :name
来源：http://www.ydjk.org.cn/Article/details/gt3wykpjdbl.html

C#:   public string Name { get; set; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndctxucp.html

[G12] 对象转字符串
来源：http://www.52xcode.cn/Article/details/gt3etnfjxoy.html

Py:   def __str__(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3jcunocde.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3zqcpuwtq.html

JS:   toString() { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyfyrmjl.html

TS:   toString(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3lesfqhxt.html

Java: @Override public String toString() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3qduavfkx.html

Go:   func (u User) String() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ktvenbqn.html

Ruby: def to_s; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt3jwoasqfv.html

C#:   public override string ToString() => Name;
来源：http://www.ydjk.org.cn/Article/details/gt3phscvmkj.html

[G13] 判断对象类型
来源：http://www.ydjk.org.cn/Article/details/gt3wsqxqtri.html

Py:   isinstance(u, User)
来源：http://www.52xcode.cn/Article/details/gt3ixxyyqah.html

PHP:  $u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3neqgyikn.html

JS:   u instanceof User
来源：http://www.52xcode.cn/Article/details/gt3rkfrwnfn.html

TS:   u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3ndrdinoj.html

Java: u instanceof User
来源：http://www.ydjk.org.cn/Article/details/gt3moxqgoou.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://www.ydjk.org.cn/Article/details/gt3itybizks.html

Ruby: u.is_a?(User)
来源：http://www.ydjk.org.cn/Article/details/gt3qyizkbpt.html

C#:   u is User
来源：http://www.52xcode.cn/Article/details/gt3nckjkngv.html

[G14] 数据类 / record
来源：http://www.52xcode.cn/Article/details/gt3fvzdvamn.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://www.52xcode.cn/Article/details/gt3zzyetjph.html

PHP:  // 用 readonly 属性模拟
来源：http://www.ydjk.org.cn/Article/details/gt3ixbsnxbz.html

JS:   // 无内置：普通类或对象字面量
来源：http://www.ydjk.org.cn/Article/details/gt3gubkmiex.html

TS:   type User = { name: string; age: number };
来源：http://www.ydjk.org.cn/Article/details/gt3ofscbvob.html

Java: record User(String name, int age) {}
来源：http://www.52xcode.cn/Article/details/gt3regzctyt.html

Go:   type User struct { Name string; Age int }
来源：http://www.ydjk.org.cn/Article/details/gt3mwkzfuhm.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://www.52xcode.cn/Article/details/gt3qnajkiby.html

C#:   record User(string Name, int Age);
来源：http://www.52xcode.cn/Article/details/gt3xdilmidc.html

[G15] 枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ilvgryno.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://www.ydjk.org.cn/Article/details/gt3wzhkpgma.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://www.ydjk.org.cn/Article/details/gt3cujaopon.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://www.ydjk.org.cn/Article/details/gt3biebhozn.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dlziskcp.html

Java: enum Color { RED, GREEN }
来源：http://www.ydjk.org.cn/Article/details/gt3ouvwjzym.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://www.52xcode.cn/Article/details/gt3nuhppisy.html

Ruby: Color = %i[red green].freeze
来源：http://www.52xcode.cn/Article/details/gt3paudlofx.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://www.52xcode.cn/Article/details/gt3gwnfgccy.html

[G16] 对象转数组 / 字典
来源：http://www.ydjk.org.cn/Article/details/gt3hbqghiyf.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://www.52xcode.cn/Article/details/gt3uysfseto.html

PHP:  get_object_vars($obj);
来源：http://www.ydjk.org.cn/Article/details/gt3biyoedwa.html

JS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jkkqcnxd.html

TS:   Object.entries(obj)
来源：http://www.52xcode.cn/Article/details/gt3jpcgmplz.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://www.ydjk.org.cn/Article/details/gt3zrphjwyo.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://www.ydjk.org.cn/Article/details/gt3rirtvkvq.html

Ruby: obj.instance_variables
来源：http://www.ydjk.org.cn/Article/details/gt3hfgbqetn.html

C#:   // 用反射或 System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3tvqyvjea.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fyrzendr.html

H. 异常与错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3pweugkji.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3loymtbge.html

[H01] try / catch 基础
来源：http://www.52xcode.cn/Article/details/gt3kmehtfap.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://www.52xcode.cn/Article/details/gt3tqvzmprv.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://www.52xcode.cn/Article/details/gt3ihafmhpz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://www.ydjk.org.cn/Article/details/gt3hqmypjak.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://www.52xcode.cn/Article/details/gt3raxtsjyw.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://www.ydjk.org.cn/Article/details/gt3ikwgbtrw.html

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://www.ydjk.org.cn/Article/details/gt3xbkjrjmn.html

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://www.ydjk.org.cn/Article/details/gt3xxuvqmve.html

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://www.52xcode.cn/Article/details/gt3twjjdfid.html

[H02] finally / ensure 收尾
来源：http://www.ydjk.org.cn/Article/details/gt3eagzthlb.html

Py:   try: f()⏎finally: cleanup()
来源：http://www.ydjk.org.cn/Article/details/gt3fqwfbzuf.html

PHP:  try { f(); } finally { cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nmxgieav.html

JS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3usmvfitn.html

TS:   try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3tkuoxvhz.html

Java: try { f(); } finally { cleanup(); }
来源：http://www.52xcode.cn/Article/details/gt3mlhbcnkn.html

Go:   defer cleanup()             // 函数返回时执行
来源：http://www.ydjk.org.cn/Article/details/gt3inhunfly.html

Ruby: begin; f; ensure; cleanup; end
来源：http://www.ydjk.org.cn/Article/details/gt3loaoluqc.html

C#:   try { F(); } finally { Cleanup(); }
来源：http://www.ydjk.org.cn/Article/details/gt3pngxwvyb.html

[H03] 主动抛出异常
来源：http://www.52xcode.cn/Article/details/gt3mjhghgvk.html

Py:   raise ValueError("错误信息")
来源：http://www.52xcode.cn/Article/details/gt3svlyxluf.html

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3nuxjhxzo.html

JS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gjquteun.html

TS:   throw new Error("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3lnvnbnzi.html

Java: throw new IllegalArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3gyfexnhv.html

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://www.ydjk.org.cn/Article/details/gt3hpxhwgoa.html

Ruby: raise ArgumentError, "错误信息"
来源：http://www.ydjk.org.cn/Article/details/gt3qemrbxod.html

C#:   throw new ArgumentException("错误信息");
来源：http://www.ydjk.org.cn/Article/details/gt3icsmxhmx.html

[H04] 自定义异常类型
来源：http://www.ydjk.org.cn/Article/details/gt3ratsdnyj.html

Py:   class MyError(Exception): pass
来源：http://www.ydjk.org.cn/Article/details/gt3ftmbvmbj.html

PHP:  class MyError extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3nnhtprqg.html

JS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3powulhza.html

TS:   class MyError extends Error {}
来源：http://www.ydjk.org.cn/Article/details/gt3gfqkcqhu.html

Java: class MyException extends RuntimeException {}
来源：http://www.52xcode.cn/Article/details/gt3fejhdxqv.html

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://www.ydjk.org.cn/Article/details/gt3jpchqwxq.html

Ruby: class MyError < StandardError; end
来源：http://www.52xcode.cn/Article/details/gt3gwmqymyj.html

C#:   class MyException : Exception {}
来源：http://www.ydjk.org.cn/Article/details/gt3yhigrgeh.html

[H05] 捕获特定类型
来源：http://www.52xcode.cn/Article/details/gt3rkyeyemy.html

Py:   except ValueError as e:
来源：http://www.ydjk.org.cn/Article/details/gt3dafiomeh.html

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://www.52xcode.cn/Article/details/gt3nfgraoon.html

JS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tjcsrtxa.html

TS:   if (e instanceof TypeError) {}
来源：http://www.ydjk.org.cn/Article/details/gt3farenubq.html

Java: catch (IOException | SQLException e) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zatcjjto.html

Go:   errors.Is(err, os.ErrNotExist)
来源：http://www.52xcode.cn/Article/details/gt3ryicwuwn.html

Ruby: rescue ArgumentError => e
来源：http://www.ydjk.org.cn/Article/details/gt3cyvftypp.html

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://www.52xcode.cn/Article/details/gt3sjsmrhzz.html

[H06] 可选值 / 空值安全访问
来源：http://www.ydjk.org.cn/Article/details/gt3bbmctlyc.html

Py:   value = d.get("k") or default
来源：http://www.ydjk.org.cn/Article/details/gt3bptkumnq.html

PHP:  $v = $d["k"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3uyxlrjsz.html

JS:   obj?.a?.b;  d ?? default
来源：http://www.ydjk.org.cn/Article/details/gt3gwepqsjc.html

TS:   obj?.a?.b;  d ?? default
来源：http://www.52xcode.cn/Article/details/gt3jyrxhtnj.html


<!-- 参考信息 -->